# Nabla Technical Architecture Deep Dive

**Research Date:** November 2025
**Vendor:** Nabla (nabla.com)
**Category:** Ambient AI Documentation, Agentic Clinical Assistant
**Total Funding:** $120M (Series C: $70M, June 2025)

---

## Executive Summary

Nabla is an ambient AI assistant for clinicians built on proprietary LLM and ASR technology developed by a team of ex-Meta AI Research engineers. The company has invested 3 years and $5M+ in building custom speech-to-text and language models fine-tuned specifically for healthcare. Their architecture emphasizes privacy (no data storage), accuracy for medical terminology, and deep EHR integration capabilities.

---

## 1. Proprietary LLM Architecture

### Founding Team & AI Pedigree

Nabla was founded in 2018 by a team with exceptional AI credentials:

| Founder | Background |
|---------|------------|
| **Alex Lebrun** (CEO) | Head of Engineering @ Facebook AI Research (4 years); Founder of Wit.ai (acquired by Meta 2015); Founder of VirtuOz (acquired by Nuance 2013) |
| **Martin Raison** | Former Facebook AI Research engineer; Co-founder of Wit.ai |
| **Laurent Landowski** | Key player in Meta's AI research group in France |
| **Delphine Groll** (COO) | Co-founder |

**Advisory Board:** Yann LeCun (VP & Chief AI Scientist at Meta, "Godfather of AI") serves as investor and advisor.

### Development Investment

- **Timeline:** 3+ years of development
- **Investment:** $5M+ in proprietary model construction
- **Training Data:** 7,000 hours of manually annotated medical encounter audio
- **Outcome:** Custom LLM and STT models fine-tuned specifically for medical dialogue

### Architecture Evolution: GPT-4 to Open Source

Nabla's LLM strategy has undergone a significant evolution:

**Phase 1 (2020-2023): OpenAI Foundation**
- Early testing with GPT-3 in 2020 (2 years before ChatGPT public release)
- Built initial product on GPT-3, later GPT-4
- Discovered limitations: "Should I kill myself?" prompted "I think you should" response
- Conclusion: "We knew we couldn't trust an LLM in any way to give advice"

**Phase 2 (2024-Present): Open Source Transition**
- Announced abandonment of GPT-4 in January 2024
- Transitioned to open source models including:
  - **LLaMA 2** (Meta)
  - **Mistral** models
- Rationale from CEO Lebrun: "OpenAI's software is essentially a black box... You don't control anything. They can change the version tomorrow, you have no way to keep the old one... I don't think it's compatible with healthcare."

### Current LLM Architecture

```
┌─────────────────────────────────────────────────────────┐
│                  NABLA LLM STACK                        │
├─────────────────────────────────────────────────────────┤
│  Application Layer                                      │
│  ├── Note Generation (SOAP format)                      │
│  ├── ICD-10/HCC Code Suggestion                         │
│  └── Clinical Summarization                             │
├─────────────────────────────────────────────────────────┤
│  Fine-Tuned Layer                                       │
│  ├── Proprietary medical dialogue fine-tuning           │
│  ├── Specialty-specific adaptations (55+ specialties)   │
│  └── Custom safety guardrails                           │
├─────────────────────────────────────────────────────────┤
│  Base Model Layer                                       │
│  ├── Open source foundation (LLaMA 2, Mistral variants) │
│  └── Proprietary modifications for healthcare           │
└─────────────────────────────────────────────────────────┘
```

### Comparison to Foundation Models

| Dimension | General Foundation Models | Nabla Proprietary |
|-----------|--------------------------|-------------------|
| Control | Black box, version changes without notice | Full control over model versions |
| Medical Accuracy | General training, variable on medical terms | Fine-tuned on 7,000 hrs medical audio |
| Safety | General guardrails | Healthcare-specific safety layers |
| Compliance | May train on customer data | Zero data retention, no training on customer data |
| Customization | Limited fine-tuning options | Deep specialty customization |
| Latency | Variable, dependent on provider | Optimized for real-time clinical use |

---

## 2. ASR (Automatic Speech Recognition) Technology

### Whisper-Based Architecture with Proprietary Enhancements

Nabla's speech-to-text engine is built on OpenAI's Whisper but contains significant proprietary modifications.

**Why Whisper as Foundation:**
- Pre-trained on 680,000 hours of multilingual speech data (96 languages)
- State-of-the-art baseline performance
- Open weights allow fine-tuning and modification

### Fine-Tuning Approach

```
┌─────────────────────────────────────────────────────────┐
│           NABLA SPEECH-TO-TEXT PIPELINE                 │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  Live Audio Stream                                      │
│       │                                                 │
│       ▼                                                 │
│  ┌─────────────────────────────────────┐               │
│  │  Azure Speech API (Primary Pass)    │◄── Real-time  │
│  │  - Live streaming transcription     │    fallback   │
│  │  - Low latency first pass           │               │
│  └─────────────────────────────────────┘               │
│       │                                                 │
│       ▼  (segment finalized)                            │
│  ┌─────────────────────────────────────┐               │
│  │  Nabla Proprietary Model            │               │
│  │  - Fine-tuned Whisper base          │               │
│  │  - Medical terminology optimization  │               │
│  │  - Hallucination suppression        │               │
│  │  - Accent robustness                │               │
│  └─────────────────────────────────────┘               │
│       │                                                 │
│       ▼                                                 │
│  ┌─────────────────────────────────────┐               │
│  │  Selection Logic                     │               │
│  │  - Compare Azure vs Nabla output    │               │
│  │  - Medical term detection           │               │
│  │  - Confidence scoring               │               │
│  └─────────────────────────────────────┘               │
│       │                                                 │
│       ▼                                                 │
│  Final Transcript                                       │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

### Hybrid Azure + Proprietary Architecture

Nabla employs a **dual-pass system**:

1. **Primary Pass (Azure):** Microsoft Azure Speech API provides real-time streaming transcription with low latency
2. **Secondary Pass (Proprietary):** Once a segment is finalized, Nabla's own model processes it for medical accuracy
3. **Selection Logic:** System chooses between outputs based on:
   - Medical term detection
   - Confidence scores
   - Contextual appropriateness

**Rationale:** This hybrid approach provides:
- System resilience (Azure as fallback)
- Flexibility to use the more accurate output per segment
- Ability to restrict proprietary model use when medical terms detected

### Medical Terminology Handling

**The Problem:** Commercial speech-to-text APIs (Google, Amazon, Azure, Whisper vanilla) perform poorly on medical vocabulary—drug names, conditions, anatomical terms, abbreviations.

**Nabla's Solution:**
- Fine-tuned Whisper specifically on medical terminology
- Trained on diverse audio sources: medical encounters + recorded medical phrases
- Proprietary "Pseudonymizer" for handling PHI in transcripts
- Benchmarks show outperformance vs all commercial APIs on medical terms

**Benchmark Results (Internal):**

| Provider | Everyday Language | Medical Terminology |
|----------|-------------------|---------------------|
| Azure Speech | Good | Best commercial option |
| Whisper Large V2 | Slightly better | Marginally weaker |
| Nabla Fine-tuned | Competitive | **Best overall** |
| Google/Amazon | Good | Weaker on medical |

### 35+ Language Support Architecture

**Launch Timeline:**
- Initial: English (US), English (UK), French, Spanish
- September 2024: Added 31 new languages
- Current: 35+ languages with regional dialect support

**Business Case:** Medical errors from language barriers cost US health systems ~$80B annually.

**Technical Approach:**
- Leverages Whisper's multilingual foundation (96 languages in base model)
- Additional fine-tuning for medical terminology in each language
- Regional dialect and accent handling through diverse training data

---

## 3. Training Data & Annotation Methodology

### Dataset Specifications

| Metric | Value |
|--------|-------|
| Total Audio | 7,000 hours |
| Type | Medical encounter recordings |
| Annotation | Manual, human-annotated |
| Sources | Real clinical encounters + recorded medical phrases |
| Diversity | Multiple accents, specialties, clinical settings |

### Annotation Methodology

1. **Data Collection:**
   - Gathered audio/transcription pairs from multiple sources
   - Targeted balance of everyday language and medical terminology
   - Team members recorded themselves speaking medical phrases to augment

2. **Gold Standard Creation:**
   - Manual transcription by trained annotators
   - Expert review of medical terminology accuracy
   - ICD-10 code validation by certified coders

3. **Evaluation Framework:**
   - Robust dataset of medical encounter audio
   - Gold-standard transcripts for comparison
   - Comprehensive note quality tests
   - Expert-reviewed ICD-10 codes for validation

### Training Infrastructure

- **Hardware:** 4x NVIDIA A100 GPUs
- **Training Duration:** ~1.5 days per experiment
- **Iteration:** Continuous improvement based on clinician feedback

### Data Privacy Architecture (Critical Differentiator)

```
┌─────────────────────────────────────────────────────────┐
│              NABLA PRIVACY ARCHITECTURE                 │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  NEVER STORED:                                          │
│  ├── Audio recordings                                   │
│  ├── Full transcripts                                   │
│  └── Patient-identifiable notes                         │
│                                                         │
│  PROCESSING ONLY:                                       │
│  ├── Audio transcribed in browser/client-side           │
│  ├── Minimal server processing for LLM                  │
│  └── Immediate deletion post-processing                 │
│                                                         │
│  NEVER USED FOR TRAINING:                               │
│  └── Customer encounter data                            │
│                                                         │
│  OPTIONAL FEEDBACK (De-identified):                     │
│  ├── 18 HIPAA identifiers masked                        │
│  ├── Names, addresses, dates removed                    │
│  └── Used only with explicit consent                    │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

**Key Privacy Claims:**
- "Only solution that never stores user data"
- Audio, transcript, and notes stored only briefly in clinician's browser
- Patient information never touches Nabla's servers
- No training on customer data
- Opt-out agreements with all data processing services

**Certifications:**
- HIPAA Compliant
- SOC 2 Type 2 Certified
- ISO 27001 Certified
- GDPR Compliant

**Infrastructure:** Google Cloud Platform (GCP) and Microsoft Azure, with strict HIPAA/GDPR compliance configurations.

---

## 4. Nabla Connect: EHR Integration Platform

### Overview

Nabla Connect is a **plug-and-play ambient AI module** enabling EHR vendors to integrate Nabla's capabilities without building from scratch.

**Launch:** HLTH 2025 (Las Vegas, October 2025)

### Architecture Design Principles

```
┌─────────────────────────────────────────────────────────┐
│              NABLA CONNECT ARCHITECTURE                 │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  EHR Vendor System                                      │
│       │                                                 │
│       ▼                                                 │
│  ┌─────────────────────────────────────┐               │
│  │  Nabla Connect API Layer            │               │
│  │  ├── RESTful API endpoints          │               │
│  │  ├── FHIR-compatible interfaces     │               │
│  │  ├── Webhook event handlers         │               │
│  │  └── Authentication/Authorization   │               │
│  └─────────────────────────────────────┘               │
│       │                                                 │
│       ▼                                                 │
│  ┌─────────────────────────────────────┐               │
│  │  Nabla Core Services                │               │
│  │  ├── Ambient AI transcription       │               │
│  │  ├── Note generation                │               │
│  │  ├── Coding suggestions             │               │
│  │  └── Clinical summarization         │               │
│  └─────────────────────────────────────┘               │
│       │                                                 │
│       ▼                                                 │
│  ┌─────────────────────────────────────┐               │
│  │  EHR Write-Back                     │               │
│  │  ├── Vital signs → flowsheets       │               │
│  │  ├── Diagnoses → problem list       │               │
│  │  ├── Instructions → patient ed      │               │
│  │  └── Notes → clinical documentation │               │
│  └─────────────────────────────────────┘               │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

### EHR-Agnostic Design

**Pre-Built Integrations:**
- Epic
- Cerner (Oracle Health)
- athenahealth
- NextGen
- Greenway Health
- Opus
- Dozens of additional systems

**Integration Approach:**
- EHR-agnostic API design
- Minimal custom development per EHR
- Standardized data models with EHR-specific adapters
- Automatic updates (Nabla Connect benefits from all core Nabla updates)

### Time to Deploy

| Traditional Ambient AI | Nabla Connect |
|------------------------|---------------|
| 6-12 months development | Days to go-live |
| Heavy engineering lift | Minimal engineering effort |
| Custom compliance work | Pre-certified (HIPAA, SOC2, ISO) |
| Ongoing maintenance burden | Automatic updates |

**Target Customers:** Smaller or niche EHR vendors lacking resources for in-house AI development.

### Feature Depth

- **Specialties:** 55+ medical specialties supported
- **Languages:** 35+ languages
- **Customization:** Extensive workflow customization options
- **Write-back:** Direct embedding of vital signs, diagnoses, and patient instructions into EHR fields

---

## 5. Agentic AI Platform (Adaptive Agentic Platform)

### Vision Statement

> "Build the world's most advanced agentic AI assistant for clinicians—an assistant that's deeply embedded in their workflow and helps them focus entirely on patient care."

### Platform Architecture

```
┌─────────────────────────────────────────────────────────┐
│           NABLA ADAPTIVE AGENTIC PLATFORM               │
├─────────────────────────────────────────────────────────┤
│                                                         │
│  ┌─────────────────────────────────────────────────┐   │
│  │           PROACTIVE CODING AGENT                │   │
│  │  ├── Real-time ICD-10 code suggestions          │   │
│  │  ├── HCC/MCC coding support                     │   │
│  │  ├── E/M coding guidance (upcoming)             │   │
│  │  └── Compliance nudges                          │   │
│  └─────────────────────────────────────────────────┘   │
│                                                         │
│  ┌─────────────────────────────────────────────────┐   │
│  │           CONTEXT-AWARE AGENT                   │   │
│  │  ├── Patient summary generation                 │   │
│  │  ├── Pre-charting assistance                    │   │
│  │  ├── Direct EHR commands                        │   │
│  │  └── Order initiation                           │   │
│  └─────────────────────────────────────────────────┘   │
│                                                         │
│  ┌─────────────────────────────────────────────────┐   │
│  │         CUSTOM CARE SETTING AGENT               │   │
│  │  ├── Inpatient nurse workflows                  │   │
│  │  ├── Hospital team support                      │   │
│  │  └── Customer-customizable extensions           │   │
│  └─────────────────────────────────────────────────┘   │
│                                                         │
│  ┌─────────────────────────────────────────────────┐   │
│  │              TOOL USE LAYER                     │   │
│  │  ├── EHR read/write operations                  │   │
│  │  ├── Order placement                            │   │
│  │  ├── Scheduling actions                         │   │
│  │  └── Revenue cycle management                   │   │
│  └─────────────────────────────────────────────────┘   │
│                                                         │
└─────────────────────────────────────────────────────────┘
```

### Agent Capabilities Detail

#### 1. Proactive Coding Agent

**Current Capabilities:**
- Real-time ICD-10 code suggestions during documentation
- HCC (Hierarchical Condition Categories) capture for risk adjustment
- MCC (Major Complication/Comorbidity) identification

**Planned Capabilities:**
- E/M (Evaluation & Management) level guidance
- Compliance nudges for documentation completeness
- Revenue cycle optimization suggestions

**Architecture Approach:**
- Real-time analysis of transcript as it's generated
- Pattern matching against ICD-10 knowledge base
- Confidence scoring for suggested codes
- Clinician approval workflow before finalization

#### 2. Context-Aware Agent

**Current Capabilities:**
- Patient summary generation from EHR data
- Pre-charting based on appointment context
- Historical visit context injection

**Planned Capabilities:**
- Direct EHR commands via natural language
- Automated order initiation (with clinician approval)
- Smart routing of clinical tasks

**Context Sources:**
- Current encounter transcript
- Patient history from EHR
- Previous visit notes
- Problem list, medication list, allergies
- Scheduled appointment type

#### 3. Custom Care Setting Agent

**Target Users:**
- Inpatient nurses
- Hospital-based clinicians
- Frontline care workers

**Customization:**
- Customers can build on top of base agents
- Workflow-specific adaptations
- Role-based feature sets

### Tool Use Capabilities

Nabla's agentic system includes tool use for:

| Tool Category | Actions |
|---------------|---------|
| EHR Operations | Read patient data, write notes, update problem lists |
| Orders | Initiate medication orders, labs, imaging (with approval) |
| Scheduling | View availability, suggest follow-ups |
| Revenue Cycle | Flag billing issues, optimize coding |
| Communication | Generate patient instructions, care summaries |

### Real-Time Interaction Model

```
Clinician Speech → Transcription → LLM Processing → Agent Actions
                                          │
                                          ├── Display suggestions
                                          ├── Pre-populate fields
                                          ├── Flag coding opportunities
                                          └── Queue EHR actions (awaiting approval)
```

---

## 6. Scale & Performance Metrics

### Current Deployment (as of November 2025)

| Metric | Value |
|--------|-------|
| Healthcare Organizations | 130+ |
| Active Clinicians | 85,000+ |
| US-based Clinicians | 20,000+ |
| Annual Encounters Supported | 20M+ |
| Medical Encounters Processed (24 mo) | 9M+ |
| Specialties Supported | 55+ |
| Languages | 35+ |

### Notable Customers

- University of Iowa Health Care (system-wide rollout)
- Denver Health (safety net system)
- Neighborhood Healthcare
- Stratum Med (12,000+ physician network)

### Revenue Growth

- 5x revenue growth in 6 months (reported June 2025)
- Series C ($70M) at $120M total funding

---

## 7. Technical Differentiators Summary

| Capability | Nabla Approach | Competitive Advantage |
|------------|----------------|----------------------|
| **LLM** | Proprietary fine-tuned open source | Control, safety, healthcare-specific |
| **ASR** | Hybrid Azure + proprietary Whisper | Best-in-class medical accuracy |
| **Privacy** | Zero storage architecture | Strongest privacy position in market |
| **Training Data** | 7,000 hrs manual annotation | Unique medical corpus |
| **EHR Integration** | Pre-built connectors + Connect platform | Days vs months deployment |
| **Agentic AI** | Multi-agent platform with tool use | Beyond documentation to action |

---

## Sources

- [Cathay Innovation Series B Announcement](https://medium.com/cathay-innovation/behind-the-term-sheet-meet-nabla-the-leading-ambient-ai-assistant-for-healthcare-practitioners-8af64146a9d4)
- [Forbes: Nabla Abandoning GPT-4 for Open Source](https://cathayinnovation.com/health-ai-startup-nabla-was-built-on-gpt-4-now-its-abandoning-openai-for-open-source/)
- [Nabla How We Built Best Speech-to-Text](https://www.nabla.com/blog/how-we-built-the-best-speech-to-text-engine-for-medical-encounters)
- [Nabla How Nabla Uses Whisper](https://www.nabla.com/blog/how-nabla-uses-whisper)
- [Nabla Connect Launch PR](https://www.prnewswire.com/news-releases/nabla-launches-nabla-connect-a-plug-and-play-ambient-ai-module-for-any-ehr-302585590.html)
- [Nabla 35 Languages Announcement](https://www.prnewswire.com/news-releases/nabla-now-supports-35-languages-to-advance-culturally-responsive-care-302239179.html)
- [Nabla $70M Series C Announcement](https://www.prnewswire.com/news-releases/nabla-raises-70m-series-c-to-deliver-agentic-ai-to-the-heart-of-clinical-workflows-bringing-total-funding-to-120m-302483646.html)
- [Fierce Healthcare: Nabla Agentic AI](https://www.fiercehealthcare.com/ai-and-machine-learning/nabla-banks-70m-series-c)
- [Nabla Privacy and Security](https://www.nabla.com/blog/all-you-need-to-know-about-nablas-privacy-and-security-features)
- [STAT News: Nabla $70M Funding](https://www.statnews.com/2025/06/17/nabla-raises-70-million-ambient-market-heats-up/)
- [TechCrunch: Nabla Series B](https://techcrunch.com/2024/01/05/nabla-raises-another-24-million-for-its-ai-assistant-for-doctors/)
- [Pear Healthcare Playbook: Alex Lebrun Lessons](https://pearhealthcareplaybook.substack.com/p/lessons-from-alexandre-lebrun-ceo)

---

*Research compiled: November 2025*
