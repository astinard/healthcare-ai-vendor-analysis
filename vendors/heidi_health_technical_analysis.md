# Heidi Health Technical Analysis

**Company:** Heidi Health (formerly Oscer)
**Headquarters:** Melbourne, Australia
**Founded:** 2019
**Analysis Date:** November 2025

---

## Executive Summary

Heidi Health is an Australian health technology company developing AI-powered medical scribe software. The platform transcribes patient consultations and generates clinical documentation using large language models (LLMs) and speech recognition. As of 2025, Heidi processes 2+ million patient interactions weekly across 100+ countries and supports 110+ languages.

**Funding:** ~USD $100 million total (Series B: $65M in October 2025, valuation $465M)
**Investors:** Point72 Private Investments, Blackbird Ventures, Headline, Local Globe

---

## 1. LLM Approach

### Model Architecture

| Aspect | Details |
|--------|---------|
| **Base Models** | Uses Large Language Models (LLMs) - specific models not publicly disclosed |
| **Customization** | Custom-trained/fine-tuned models for medical terminology |
| **Processing** | Data processed through customized LLMs stored in privately hosted servers |

### Australian English Optimization

- **Custom Model:** Heidi utilizes a custom model specifically engineered to handle regional dialects and medical terminology variations
- **Multi-Accent Support:** Real-time transcription trained to accurately detect multiple speakers and various accents
- **Regional Dialects:** Adaptive voice recognition handles regional dialects and medical terms with precision
- **Market-Leading Accuracy:** Claims "market-leading word error rates" regardless of regional differences

### Medical Terminology

- **Domain Training:** Models specifically trained on medical vocabulary and clinical terminology
- **Specialty Support:** Supports documentation across wide range of specialties (cardiology, paediatrics, surgery, allied health)
- **Veterinary Support:** Captures veterinary drug names (generic and brand) accurately
- **Clinical Coding:** Automatically suggests ICD-10-CM and CPT codes drawn from documentation

### Accuracy Claims

| Metric | Claim | Source |
|--------|-------|--------|
| **Documentation Time Reduction** | 51% reduction | Large-scale clinical rollout data |
| **Note-Taking Reduction** | From 17 min to 4 min per patient | Hawke's Bay Hospital trial (NZ) |
| **Quality Assurance** | Medical team reviews and refines AI outputs | Company statement |
| **KLAS Recognition** | 2025 KLAS Research spotlight cited improved note accuracy | Independent research |

**Limitations Noted:**
- AI transcription can make mistakes (accent variations, microphone positioning)
- Some mobile app reliability issues reported (crashes, freezing during dictation)

---

## 2. ASR Technology

### Speech Recognition Approach

| Feature | Details |
|---------|---------|
| **Technology** | Ambient AI / ambient listening technology |
| **Mode** | Real-time transcription with offline capability |
| **Speaker Detection** | Multi-speaker clinical environment optimization |
| **Audio Storage** | No audio recordings stored (transcription only) |

### Australian Accent Handling

- **Accent Adaptation:** Trained to accurately detect various accents including Australian/NZ
- **Regional Dialect Support:** Custom model engineered for regional dialect variations
- **Adaptive Learning:** Voice recognition technology "rapidly adapts to different clinician styles"
- **Multicultural Support:** Designed for multicultural and multilingual clinical environments

### Background Noise Handling

- **Clinical Optimization:** Ambient capture optimized for multi-speaker clinical environments
- **Medical Vocabulary:** Specifically tuned for medical terminology in noisy settings
- **Mobile Support:** Works on iOS, Android, and desktop clients

### Real-Time vs Batch Processing

| Mode | Capability |
|------|------------|
| **Real-Time** | Primary mode - ambient listening during consultations |
| **Dictation** | Clinicians can dictate during or after encounters |
| **Offline Mode** | Transcription continues without internet; syncs when reconnected |
| **Post-Consult** | Notes can be generated after the consultation |

### Technical Specifications

- **Languages:** 110+ languages supported
- **Deployment:** Cloud-native SaaS with web and mobile clients (iOS/Android/web)
- **Client:** Lightweight client for ambient capture (mobile/desktop)
- **Latency:** Throughput and latency scale with subscription tier and enterprise architecture

---

## 3. EHR Integrations

### Australian Clinical Software

| System | Integration Status | Details |
|--------|-------------------|---------|
| **Best Practice (Bp Premier)** | Full Integration | Native integration via Setup menu; one-click push to patient records |
| **MedicalDirector Clinical** | Full Integration | "Smart Scribe" - built into SmartBar, no separate install needed |
| **Genie Solutions** | Planned/Requested | Dr. Kelly confirmed plans for integration |
| **Gentu (Magentus)** | Full Integration | Cloud-based PM software with seamless Heidi access |
| **Cliniko** | Full Integration | Two-way sync; appointment pull and note push (AU only, Together plan) |
| **MediRecords** | Full Integration | Deep integration announced; embedded Heidi capability |

### Best Practice Integration Details

- **Setup:** Enable via Best Practice Setup menu → Integrations menu in Heidi
- **Workflow:** Push notes/documents directly to patient's medical record
- **Availability:** Notes instantly available for final edits and saving
- **Market:** Best Practice is leading AU GP software

### MedicalDirector Integration ("Smart Scribe")

- **Architecture:** Heidi built directly into MedicalDirector Clinical (not external overlay)
- **Access:** Available in SmartBar - nothing new to install
- **Pricing:** Free for Heidi Together and Enterprise Plans
- **Real-Time:** Generate structured notes and push with one click

### Hospital Systems

| System | Integration Status |
|--------|-------------------|
| **Epic Systems** | Integrated |
| **Athenahealth** | Integrated |
| **Gentu by Magentus** | Integrated |
| **Veradigm** | Integrated |

### Notable Australian Deployments

- **ForHealth** (Australia)
- **Victorian Virtual Emergency Department** (via MediRecords integration)
- **Queensland Health** (via MediRecords)
- **Health New Zealand** - 16 emergency departments, 1,000+ clinician licenses

---

## 4. Medicare Integration

### MBS/Medicare Support

| Feature | Status |
|---------|--------|
| **Pre-built Templates** | Medicare claims templates available |
| **MBS Item Numbers** | Not explicitly confirmed in public documentation |
| **Bulk Billing Workflows** | Templates for billing workflows |
| **PBS Integration** | Not confirmed |

### Billing & Coding Features

- **ICD-10-CM Codes:** Automatically suggested from documentation
- **CPT Codes:** Ranked by relevance and flagged for review
- **Medicare Claims Templates:** Pre-built templates shared by clinicians
- **Mental Health Care Plans:** Templates available
- **Insurance Forms:** Pre-built templates

### Australian Healthcare Forms

- Templates for:
  - Medicare claims
  - Mental health care plans
  - Insurance forms
  - Referral letters
  - Patient summaries

**Note:** Direct Medicare API integration (Services Australia) not publicly confirmed. Integration appears to be via template-based workflow support rather than direct MBS claiming.

---

## 5. Infrastructure

### Cloud Provider

| Aspect | Details |
|--------|---------|
| **Architecture** | Cloud-native SaaS |
| **Providers** | AWS and GCP (per job listings) |
| **Deployment** | Multi-region with local data processing |

### Data Residency (Australian Servers)

| Aspect | Status |
|--------|--------|
| **Australian Storage** | Yes - data stored in servers located in Australia |
| **Onshore Processing** | Yes - information processed onshore |
| **Offshore Services** | When necessary for performance, with compliance measures |
| **Pseudonymization** | Applied for offshore processing |
| **Local Storage** | Compliant local storage solutions used |

### Data Processing Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    Heidi Health Platform                      │
├─────────────────────────────────────────────────────────────┤
│  Client Layer                                                │
│  ├── Web Application                                         │
│  ├── iOS Mobile App                                          │
│  ├── Android Mobile App                                      │
│  └── Desktop Client (ambient capture)                        │
├─────────────────────────────────────────────────────────────┤
│  Processing Layer                                            │
│  ├── Real-time ASR Engine (custom medical model)             │
│  ├── LLM Processing (customized models)                      │
│  └── Document Generation Engine                              │
├─────────────────────────────────────────────────────────────┤
│  Storage Layer                                               │
│  ├── Australian Data Centers (primary)                       │
│  ├── Encrypted at rest and in transit                        │
│  └── No audio storage (transcripts only)                     │
├─────────────────────────────────────────────────────────────┤
│  Integration Layer                                           │
│  ├── EHR Connectors (BP, MD, Cliniko, Epic, etc.)           │
│  └── API Gateway                                             │
└─────────────────────────────────────────────────────────────┘
```

### Latency for AU Users

- **Local Processing:** Data processed onshore in Australia
- **Offline Capability:** Transcription continues without internet connection
- **Sync:** Automatic sync when connection restored
- **Enterprise Scaling:** Latency scales with subscription tier and cloud provisioning

### Uptime/Reliability

| Certification | Status |
|--------------|--------|
| **SOC2 Type 2** | Certified |
| **ISO27001** | Certified |
| **HIPAA** | Compliant |
| **GDPR** | Compliant |
| **Australian Privacy Principles** | Compliant |
| **NHS DCB0129/DTAC/DSPT** | Compliant |
| **PIPEDA** | Compliant |

### Security Features

- **Encryption:** At rest and in transit
- **Audio Policy:** No audio recordings stored
- **Data Deletion:** Permanent deletion when requested
- **Auto-Redaction:** Automatically removes identifiable details from transcripts
- **Incident Response:** Strict protocol per ISO27001/SOC2

---

## 6. Scale & Performance Metrics

| Metric | Value |
|--------|-------|
| **Weekly Patient Interactions** | 2+ million |
| **Countries** | 100+ |
| **Languages** | 110+ |
| **Hours Returned to Clinicians** | 18+ million (in 18 months) |
| **Patient Visits Supported** | 73+ million total |

---

## 7. Competitive Position (Australian Market)

### Key Differentiators

1. **Australian Origin:** Founded in Melbourne, deep AU market understanding
2. **Australian Data Residency:** Data stored and processed in Australia
3. **Comprehensive AU EHR Integration:** Best Practice, MedicalDirector, Cliniko, MediRecords
4. **Offline Capability:** Critical for regional/rural Australian practices
5. **Multi-Accent Support:** Australian, NZ, and international accents

### Competitive Landscape

| Competitor | Notes |
|------------|-------|
| **Lyrebird Health** | AU competitor; Best Practice integration partner (Feb 2024) |
| **Nuance (Microsoft)** | Global leader; DAX Copilot |
| **Abridge** | US-focused |
| **Nabla** | European origin |

---

## 8. Technical Gaps & Unknowns

| Area | Gap |
|------|-----|
| **Specific LLM Models** | Not disclosed (GPT, Claude, or proprietary) |
| **ASR Engine** | Custom model details not public |
| **Direct Medicare API** | Integration with Services Australia not confirmed |
| **Genie Solutions** | Full integration pending |
| **Hospital EMR** | Deep integration with Australian hospital systems (Cerner, etc.) unclear |
| **PBS Integration** | Not confirmed |

---

## Sources

- [Heidi Health Wikipedia](https://en.wikipedia.org/wiki/Heidi_Health)
- [Heidi Health Official Site](https://www.heidihealth.com/en-au)
- [Best Practice Integration](https://bestpracticesoftware.com/partner-network/our-partners/heidi-health/)
- [Cliniko Integration](https://www.cliniko.com/connected-apps/heidi/)
- [MedicalDirector Integration](https://www.heidihealth.com/au/blog/medicaldirector-integration)
- [Health NZ Emergency Department Rollout](https://www.nzherald.co.nz/business/health-nz-to-roll-out-heidi-ai-scribe-in-16-emergency-departments-but-whats-the-story-with-errors-and-privacy/premium/)
- [Medical Republic - AI Scribe Wars](https://www.medicalrepublic.com.au/ai-scribe-wars-heating-up/111273)
- [Heidi Compliance FAQs](https://www.heidihealth.com/blog/heidi-compliance-lightning-faqs)
- [Heidi Safety Page](https://www.heidihealth.com/en-au/safety)
- [MediRecords Partnership](https://www.hospitalhealth.com.au/content/technology/news/partnership-to-streamline-clinical-documentation-641417954)

---

*Analysis compiled November 2025*
