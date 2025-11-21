# Commure + Augmedix: Technical Architecture Deep Dive

## Executive Summary

Commure (merged with Athelas in a $6B deal) acquired Augmedix (July 2024, $139M) to create one of the largest AI software providers in healthcare. The combined entity powers **20+ million clinician appointments annually** across **150+ hospital systems** with **350,000+ clinicians** and integrations with **60+ EHRs**.

---

## 1. MULTI-MODEL STRATEGY

### Foundation Models Used

| Model Type | Provider | Use Case |
|------------|----------|----------|
| **MedLM** | Google Cloud | Medically-tuned note generation, specialty expansion |
| **Med-PaLM 2** | Google Cloud | Clinical reasoning (piloted) |
| **Google Cloud Speech-to-Text** | Google Cloud | Real-time ASR transcription |
| **Specialty Fine-Tuned LLMs** | Proprietary | Specialty-specific note formatting |

**Key Partnership Details:**
- Augmedix has been piloting Google Cloud's **Med-PaLM 2** and integrating **MedLM** into their tech stack
- Uses **Vertex AI** for fine-tuning models with proprietary training data from **70,000 notes generated weekly** across 30+ specialties
- MedLM integration announced January 2024 for Augmedix Go product

### Model Routing Approach

**Multi-Pass Architecture:**
```
Audio Input → ASR (Google Speech-to-Text)
           → NLP Pipeline (Multiple Passes)
           → Foundational LLM (MedLM/Med-PaLM 2)
           → Specialty Fine-Tuned LLM
           → Structured Note Output
```

The system uses **foundational and specialty-specific fine-tuned LLMs** that make **multiple passes** to generate natural-sounding notes. Additional NLP models generate structured data for note review and analytical purposes.

### Specialty-Specific Models

**Currently Supported (35+ Specialties):**
- **Emergency Department**: Bespoke app with ED-specific AI
- **Oncology**: AI fine-tuned for cancer care workflows
- **Primary Care**: High-volume ambulatory documentation
- **Orthopedics**: Procedure-heavy documentation
- **Hospitalist**: Inpatient rounding workflows

**Fine-Tuning Approach:**
- Training data from existing Augmedix production (70K notes/week)
- Specialty-specific vocabulary and note templates
- MedLM enables rapid expansion to new subspecialties
- Custom models for complex clinical workflows and noisy environments (ED)

### Cost Optimization

**Tiered Product Strategy:**
| Tier | Automation Level | Human Support | Cost Profile |
|------|-----------------|---------------|--------------|
| **Go** | Pure AI | None | Lowest |
| **Assist/Notes** | AI + QA | MDS review within 1 hour | Medium |
| **Live** | AI + Real-time | Dedicated specialist | Highest |

**Efficiency Gains:**
- Google Cloud MedLM reduces compute costs for specialty expansion
- Hybrid model offloads simple cases to pure AI
- Human reviewers handle exceptions and complex cases

---

## 2. KNOWLEDGE GRAPH / PATIENT 360 ARCHITECTURE

### Data Platform Design

**FHIR-Native Foundation:**
- Commure launched as a **FHIR-native open platform** for healthcare developers (2020)
- HL7 FHIR server built on open principles
- Supports FHIR DSTU2, STU3, R4 standards
- Compliant with 21st Century Cures Act requirements

**Platform Components:**
```
┌─────────────────────────────────────────────────────────┐
│                  Commure Platform                        │
├─────────────────────────────────────────────────────────┤
│  • HL7 FHIR Server (R4)                                 │
│  • Event Service Bus                                    │
│  • API Gateway                                          │
│  • Flexible Data Store                                  │
│  • Terminology Services                                 │
│  • Healthcare-specific UI Components                    │
│  • REST APIs & SDKs                                     │
└─────────────────────────────────────────────────────────┘
```

### Patient 360 / PatientKeeper

**PatientKeeper Co-Pilot Features:**
- AI surfaces most important patient information
- **12-hour summaries** highlight significant changes, treatments, key data
- Chat interface for natural language queries against patient record
- Longitudinal view across encounters without EHR navigation

**Context Integration:**
- Pre-visit information pulled from scheduling systems
- Historical context from prior encounters
- Patient conversations flow through unified system
- Coding model has complete clinical picture due to shared architecture

### Ontology Mapping

**Standard Terminology Support (via FHIR/Industry Standards):**
| Standard | Use Case |
|----------|----------|
| SNOMED CT | Clinical findings, diagnoses |
| LOINC | Laboratory observations |
| RxNorm | Medication normalization |
| ICD-10 | Diagnosis coding |
| CPT | Procedure coding |

*Note: Specific implementation details of ontology mapping are not publicly disclosed. Commure's FHIR platform inherently supports UMLS-integrated terminologies.*

### Memory Across Encounters

**Contextual Persistence:**
- Previous visit summaries available for current encounter
- Medication lists carried forward with drug interaction checks
- Ambient system maintains conversation context for multi-hour appointments
- AI can reference "last EKG" or historical medication changes

---

## 3. AGENTIC ARCHITECTURE

### Commure Agents Overview

**June 2025 Launch:** Commure launched "Commure Agents" - AI assistants fully integrated into the EHR that automate entire workflows.

**Architecture Principles:**
- Full EHR integration (read/write capabilities)
- Embedded in clinical workflow (not separate app)
- "Lights out" automation for administrative tasks
- 24/7 autonomous operation capability

### Agent Types & Capabilities

| Agent | Function | Automation Level |
|-------|----------|-----------------|
| **Referral Management** | Automate specialist referrals, follow-ups | Full |
| **Prior Authorization** | Submit/track insurance approvals real-time | Full |
| **Discharge Planning** | Generate personalized discharge instructions | Full |
| **Revenue Cycle Optimization** | Identify inefficiencies, suggest improvements | Advisory |
| **Claims Processing** | Submit, track, reconcile insurance claims | Full |
| **Denials Autopilot** | Identify errors in rejected claims, resubmit | Full |

### Tool Use (EHR Read/Write)

**EHR Integration Capabilities:**
```
READ Operations:
├── Provider schedules (FHIR API)
├── Patient encounter data
├── Historical notes and labs
├── Medication lists
├── Insurance information
└── Prior authorization status

WRITE Operations:
├── Clinical notes (by section: HPI/ROS/PE/AP)
├── Orders (medications, labs, imaging)
├── Referral letters
├── Discharge instructions
├── AVS (After Visit Summary)
├── CPT/ICD-10 codes
└── Quality measures
```

**Specific Integrations:**
- **Epic**: Deep integration, embedded in workflow
- **Cerner/Oracle Health**: FHIR R4 APIs
- **MEDITECH Expanse**: Direct embedding in Expanse Now mobile app
- **athenahealth**: FHIR APIs for scheduling + note upload

### Planning and Orchestration

**Workflow Orchestration:**
```
Patient Visit → Ambient Capture
             → Real-time Transcription
             → Note Draft Generation
             → Coding Suggestion
             → Order Generation
             → EHR Filing
             → Billing Workflow Trigger
```

**Practice Management OS:**
- Cloud-based operating system
- AI agents for patient outreach, scheduling, engagement
- Task orchestration across disparate EHRs
- Unified architecture connecting fragmented systems

### Guardrails Architecture

**Multi-Layer Safety:**

1. **Model-Level Guardrails:**
   - LLMs fine-tuned for healthcare (not general web access)
   - Reduced hallucination rates with medical context
   - Better conversation/information contextualization

2. **Workflow Guardrails:**
   - Code edits flag incompatible combinations
   - High-complexity visits routed for additional review
   - Clinician sign-off required for all AI-proposed codes
   - "Autonomous" does not bypass clinician approval

3. **Clinical Decision Support:**
   - Evidence-based guideline surfacing
   - Drug interaction alerts
   - Medication safety checks (QT prolongation, etc.)
   - Pre-order safety cues

---

## 4. SAFETY & GOVERNANCE

### Compliance Certifications

| Certification | Status | Coverage |
|--------------|--------|----------|
| **HIPAA** | Certified | Full platform |
| **HITRUST CSF** | Certified | Enterprise security |
| **SOC 2** | Certified | Data handling |

### PHI/PII Controls

**Technical Safeguards:**
- End-to-end encryption for audio/video streams
- Robust user consent policies
- Enterprise-grade security meeting health system expectations
- FHIR-based access controls

**Administrative Controls:**
- Data retention policies
- Patient consent workflows
- Compliance and security workstream
- Role-based access management

### Audit Trail Implementation

**HIPAA Audit Trail Requirements Met:**
- Who accessed patient records
- What actions were taken
- When they occurred
- Device/location information
- 6-year retention requirement compliance

**Platform Logging:**
- Commure Ambient AI saves visit details for future reference and audits
- Complete documentation of AI-generated content vs. clinician edits
- Transparency in AI decision-making for clinical inferences

### Red-Teaming Program

**Publicly Disclosed Information:** Limited

**Inferred Safety Practices:**
- Forward-deployed engineering model allows continuous monitoring
- Pilot programs (e.g., HCA 4-site ED pilot) test before full deployment
- Clinician champions provide qualitative and quantitative feedback
- Weekly QA initially, transitioning to monthly for stable deployments

### Prompt Injection Defenses

**Not Publicly Disclosed**

**Industry Context:** Healthcare AI systems require technical safeguards per HIPAA §164.312 including:
- Access controls accounting for prompt injection risks
- Audit logging for all PHI access
- Input validation for natural language interfaces

---

## 5. HUMAN + AI HYBRID MODEL

### Legacy Augmedix Human Scribe Model

**Original Model (Founded 2012):**
- Remote human scribes observing visits via audio/video
- Real-time documentation during patient encounter
- Full clinical workflow support
- Dedicated scribe per clinician relationship

**Workforce Scale:**
- 1,001-5,000 employees (many as Medical Documentation Specialists)
- Serving 20+ major health systems
- Hundreds of sites of care

### Transition to AI

**Evolution Timeline:**
```
2012: Founded with human scribe model
2021: Notebuilder platform with AI-assisted transcription
2023: Augmedix Go launched (pure AI option)
2024: Google Cloud MedLM integration
2024: Commure acquisition, agentic AI integration
2025: Full Commure Agents platform
```

**Current Hybrid Architecture:**
```
┌────────────────────────────────────────────────────────┐
│                 Audio/Video Stream                      │
└────────────────────────────────────────────────────────┘
                          │
                          ▼
┌────────────────────────────────────────────────────────┐
│              ASR (Google Speech-to-Text)                │
└────────────────────────────────────────────────────────┘
                          │
                          ▼
┌────────────────────────────────────────────────────────┐
│       NLP + LLM Pipeline (MedLM, Fine-tuned models)     │
│       - Multiple passes for natural note generation     │
│       - Specialty-specific formatting                   │
│       - Structured data extraction                      │
└────────────────────────────────────────────────────────┘
                          │
           ┌──────────────┼──────────────┐
           ▼              ▼              ▼
      [Go Path]    [Assist Path]   [Live Path]
      Pure AI      AI + 1hr QA     Real-time MDS
           │              │              │
           ▼              ▼              ▼
┌────────────────────────────────────────────────────────┐
│              Clinician Review & Sign-off                │
└────────────────────────────────────────────────────────┘
                          │
                          ▼
┌────────────────────────────────────────────────────────┐
│                    EHR Integration                      │
└────────────────────────────────────────────────────────┘
```

### Quality Assurance Approach

**Medical Documentation Specialist (MDS) Role:**
- More than scribe or transcriptionist
- Tech-enabled specialist functioning as care team member
- Uses Notebuilder Platform for QA
- Ensures fidelity, comprehensive content, relevant context

**QA Workflow:**
| Service Tier | QA Process | Turnaround |
|--------------|------------|------------|
| **Go** | Clinician self-review | Immediate |
| **Assist/Notes** | MDS quality review + finalization | < 1 hour |
| **Live** | Real-time MDS supervision + editing | Real-time |

**Ongoing QA Protocol:**
- Weekly QA initially for new deployments
- Transition to monthly for stable deployments
- Small ops team (1-3 FTEs per dozens of clinicians)
- Manage exceptions, onboarding, performance metrics
- Feedback loops for continuous improvement

### When Humans Are Involved

**Always:**
- Clinician review and sign-off (all AI outputs)
- Code review for autonomous coding suggestions
- High-complexity visit routing

**Assist/Notes Tier:**
- MDS reviews all AI-generated drafts
- Editing, coding, orders, data entry support
- Referral letter preparation

**Live Tier:**
- Dedicated MDS observes entire visit
- Real-time supervision of AI engine
- Immediate correction for complex cases
- Gets to know each clinician's preferences

**Exception Handling:**
- Complex specialty cases
- Noisy environments (ED)
- Multi-speaker conversations
- Non-English encounters (60+ language support)

---

## 6. TECHNICAL INFRASTRUCTURE

### Cloud Platform

**Google Cloud Partnership:**
- MedLM on Vertex AI for medical LLM capabilities
- Google Cloud Speech-to-Text for ASR
- HIPAA-compliant cloud infrastructure

**Platform Architecture:**
- Cloud-based Practice Management OS
- Multi-tenant architecture serving 150+ health systems
- Real-time processing for 20M+ appointments/year

### Scale Metrics

| Metric | Value |
|--------|-------|
| Annual appointments powered | 20M+ |
| Clinicians using platform | 350,000+ |
| EHR integrations | 60+ |
| Annual claims processed | $10B+ |
| Patient interactions | 100M+ |
| Supported specialties | 35+ |
| Supported languages | 60+ |

### Performance Outcomes

**Documentation Efficiency:**
- 80% reduction in documentation time
- Average 43 seconds to close clinical note
- 2 hours saved per physician per day
- 20-50% reduction in documentation time (varies by specialty)

**Revenue Cycle Impact:**
- 25%+ reduction in claim denials
- 19% drop in denials (Ambient facilities vs. non-Ambient)
- 31% reduction in documentation errors
- 5-15% coding capture uplift

---

## Sources

### Primary Sources
- [Commure Official Website](https://www.commure.com/)
- [Augmedix Official Website](https://www.augmedix.com/)
- [Commure-Augmedix Acquisition Announcement](https://www.commure.com/blog/commure-and-athelas-sign-deal-to-acquire-augmedix)
- [Commure Agents Launch](https://www.commure.com/press-releases/commure-launches-commure-agents---ai-assistants-that-fully-automate-physician-workflows)
- [HCA Healthcare Partnership](https://www.commure.com/press-releases/hca-and-commure-announce-largest-ai-deployment-in-healthcare)

### Google Cloud Partnership
- [Augmedix-Google Cloud MedLM Partnership](https://www.prnewswire.com/news-releases/augmedix-partners-with-google-cloud-to-bring-medically-tuned-ai-technology-to-ambient-documentation-302014271.html)
- [Google MedLM Introduction](https://cloud.google.com/blog/topics/healthcare-life-sciences/introducing-medlm-for-the-healthcare-industry)
- [Fierce Healthcare - MedLM Launch](https://www.fiercehealthcare.com/ai-and-machine-learning/google-unveils-medlm-generative-ai-models-healthcare-hca-augmedix-and)

### Technical Architecture
- [Augmedix Notebuilder Platform](https://www.augmedix.com/resources/news/augmedixs-proprietary-notebuilder-tool-leverages-intelligent-automation-technology-to-efficently-deliver-accurate-and-timely-medical-notes/)
- [Augmedix Google Cloud ASR Partnership](https://augmedix.com/resources/news/augmedix-announces-partnership-with-google-cloud-to-harness-automated-speech-recognition-technology/)
- [Commure FHIR Platform Launch](https://hitconsultant.net/2020/02/10/commure-launches-fhir-native-open-platform-for-healthcare-developers/)
- [Augmedix Product Overview](https://www.augmedix.com/product-overview)

### Industry Analysis
- [Healthcare Dive - Acquisition Coverage](https://www.healthcaredive.com/news/commure-acquire-augmedix-ai-documentation/721978/)
- [Fierce Healthcare - Commure Agents](https://www.fiercehealthcare.com/ai-and-machine-learning/fresh-200m-raise-commure-rolls-out-ai-agents-automate-physician-workflow)
- [Athelas-Commure Merger](https://www.athelas.com/tbh/athelas-commure-merging-to-create-a-6b-healthcare-infrastructure-company)

---

## Research Gaps & Limitations

**Information Not Publicly Available:**
1. **Specific LLM Providers**: Beyond Google Cloud MedLM, other LLM vendors (OpenAI, Anthropic) not confirmed
2. **Graph Database**: Whether Neo4j, Neptune, or other graph DB is used for Patient 360
3. **Red-Teaming Details**: Formal adversarial testing program specifics
4. **Prompt Injection Defenses**: Technical implementation details
5. **Model Routing Logic**: Specific criteria for routing between models
6. **Fine-Tuning Dataset Composition**: Detailed training data methodology

**Recommendations for Further Research:**
- Direct vendor engagement for technical deep dives
- Security whitepapers or trust documentation
- Academic publications from Augmedix/Commure engineering teams
- Customer case studies with technical implementation details

---

*Research compiled: November 2025*
*Confidence Level: High for publicly disclosed information; Moderate for inferred architecture details*
