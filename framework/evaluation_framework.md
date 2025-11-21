# Healthcare AI Vendor Analysis Framework (2025)

## Purpose
Comprehensive evaluation framework for clinical AI solutions (ambient documentation, CDS, CDI, coding) for enterprise health system procurement decisions.

---

## 1. Company Profile

| Field | Description |
|-------|-------------|
| Company Name | |
| Founded | |
| HQ Location | |
| Valuation / Funding Stage | Series A/B/C, total raised |
| Employees | Total headcount |
| Clinical Team Size | MDs, RNs on staff |
| Key Investors | Strategic partners (health systems, EHR vendors, cloud) |
| Revenue Model | Per-provider/month, per-encounter, enterprise license |
| Target Market | SMB, mid-market, enterprise, academic |

---

## 2. Foundation Model & AI Stack

| Field | Description |
|-------|-------------|
| **Primary LLM** | GPT-4o, Claude 3.5, Gemini, proprietary, open-source |
| **Multi-Model Strategy** | Single model vs. routing across models |
| **ASR Provider** | Deepgram, Whisper, Nuance, proprietary |
| **ASR Medical Tuning** | Medical vocabulary fine-tuning? |
| **Agentic Architecture** | Single-shot vs. multi-agent orchestration |
| **Tool Use** | EHR read/write, coding lookup, order entry |
| **Memory / Context** | Stateless vs. persistent across encounters |
| **Knowledge Graph** | Patient 360, ontology mapping (SNOMED, LOINC, RxNorm) |
| **RAG Implementation** | Vector store, retrieval strategy |
| **Fine-Tuning** | Custom models per specialty/org |
| **On-Prem Option** | Cloud-only vs. on-prem/private cloud |

---

## 3. Clinical Capabilities

### 3a. Ambient Documentation
| Field | Description |
|-------|-------------|
| Real-time vs. Post-visit | When is note generated? |
| Specialties Supported | # and which (EM, primary care, specialty) |
| Note Types | SOAP, H&P, procedure notes, consults |
| Template Customization | Per-provider, per-specialty, per-org |
| Multi-language | Languages supported |
| Interpreter Mode | Bilingual encounters handled? |
| Diarization | Speaker identification accuracy |

### 3b. Beyond Ambient (The New Frontier)
| Field | Description |
|-------|-------------|
| **Auto-Coding** | ICD-10, CPT/HCPCS suggestion |
| **CDI** | Real-time documentation integrity nudges |
| **CDS** | Care gap identification, risk scores, alerts |
| **Pre-Charting** | Patient summary before encounter |
| **After-Visit Summary** | Patient-facing output |
| **Referral Letters** | Auto-generated |
| **Orders Suggestion** | Labs, imaging, referrals |
| **MDM Calculation** | E/M level support |

---

## 4. EHR Integration

| Field | Description |
|-------|-------------|
| **EHRs Supported** | Epic, Cerner, Meditech, Athena, etc. |
| **Integration Depth** | |
| - SMART on FHIR | Embedded app? |
| - API Write-back | Direct note insertion? |
| - RPA/Screen Scrape | Workaround method? |
| - HL7/FHIR Ingest | Data pull from EHR |
| **Bi-directional** | Read AND write? |
| **Epic App Orchard** | Listed? Validated? |
| **Cerner Code** | Listed? |
| **Meditech Integration** | Expanse, 6.x support? |
| **Time to Go-Live** | Days/weeks/months |

---

## 5. User Experience

| Field | Description |
|-------|-------------|
| **Platforms** | iOS, Android, Web, Desktop |
| **In-EHR vs. Standalone** | Embedded or separate app |
| **Editing Interface** | Inline, side panel, copy-paste |
| **Voice Commands** | Navigate EHR by voice? |
| **Dictation Mode** | Traditional dictation option |
| **Provider Feedback** | Accept/reject/edit tracking |
| **NPS / Satisfaction** | Published scores? |
| **Self-Onboarding** | Provider can start without IT? |

---

## 6. Safety & Trust

| Field | Description |
|-------|-------------|
| **Guardrails Architecture** | Deterministic checks on LLM output |
| **Hallucination Mitigation** | Grounding, citation, verification |
| **Red-Teaming Program** | Adversarial testing (prompt injection, jailbreaks) |
| **PHI/PII Controls** | De-identification, pseudonymization |
| **Audit Trail** | Full traceability of AI decisions |
| **Human-in-Loop** | When/how humans review |
| **Citation to Source** | Link output to transcript/EHR data |
| **Confidence Scoring** | Does system flag uncertainty? |
| **Error Reporting** | How are mistakes captured/learned from? |

---

## 7. Security & Compliance

| Field | Description |
|-------|-------------|
| **HIPAA** | BAA available |
| **SOC 2 Type II** | Certified? |
| **HITRUST** | Certified? |
| **GDPR** | EU compliance (critical for Ramsay UK/EU) |
| **TGA** | Australia regulatory (critical for Ramsay AU) |
| **FDA Status** | Registered? 510(k)? Exempt? |
| **Data Residency** | Where is data stored? Regional options? |
| **Retention Policy** | How long is data kept? |
| **Encryption** | At rest, in transit |
| **Penetration Testing** | Frequency, third-party? |

---

## 8. Pricing & ROI

| Field | Description |
|-------|-------------|
| **Pricing Model** | Per-provider, per-encounter, site license |
| **List Price** | $/provider/month |
| **Enterprise Discount** | Volume pricing available? |
| **Implementation Cost** | One-time fees |
| **ROI Metrics Claimed** | Time saved, revenue capture, denial reduction |
| **Published Case Studies** | Health system references |
| **Time to Value** | When do benefits materialize? |

---

## 9. Market Position & Partnerships

| Field | Description |
|-------|-------------|
| **Cloud Partner** | AWS, Azure, GCP |
| **LLM Partner** | OpenAI, Anthropic, Google, Microsoft |
| **EHR Partnership** | Strategic relationship with Epic, Cerner, etc. |
| **Health System Anchors** | Flagship customers (HCA, Kaiser, etc.) |
| **Geographic Focus** | US-only, global, specific regions |
| **Competitive Positioning** | How do they differentiate? |

---

## 10. Roadmap & Future

| Field | Description |
|-------|-------------|
| **2025 Roadmap** | What's coming? |
| **Multimodal** | Images, waveforms, pathology |
| **Nursing/MA Workflows** | Beyond physician documentation |
| **Patient Messaging** | AI-assisted inbox |
| **Revenue Cycle** | Coding → billing → denial management |
| **Voice-Native EHR** | Full ambient + command mode |

---

## Vendor Comparison Matrix (Example)

| Vendor | LLM | EHR Integration | Beyond Ambient | Enterprise Ready | Global |
|--------|-----|-----------------|----------------|------------------|--------|
| Nuance/Microsoft | GPT-4 | Epic deep | Coding, CDS | Yes | Yes |
| Abridge | Proprietary + GPT | Epic, others | CDI | Yes | US-focused |
| Nabla | Llama + proprietary | Moderate | Coding | Growing | EU + US |
| Suki | GPT-4 | Broad | Basic CDS | Yes | US-focused |
| Augmedix/Commure | Multi-model | Epic, Meditech | Coding, CDI, CDS | Yes | US-focused |
| Freed | GPT-4 | Limited | Basic | SMB | US-focused |
| Deepscribe | Proprietary + AWS | Moderate | Coding | Growing | US-focused |

---

## Ramsay-Specific Considerations

Given Ramsay's global footprint (Australia, UK, France, Nordics, Asia):

1. **Multi-jurisdiction compliance** - GDPR, TGA, local regulations
2. **EHR diversity** - Different systems in each region
3. **Language support** - English, French, Swedish, etc.
4. **Data residency** - Must support regional data storage
5. **Vendor stability** - Need established players, not just US startups
6. **Integration approach** - FHIR-first for cross-EHR portability

---

## How to Use This Framework

1. **Initial Screen** - Filter vendors by must-haves (EHR support, compliance, geo)
2. **Deep Dive** - Complete full evaluation for top 3-5 vendors
3. **Pilot Design** - Define success metrics before pilot
4. **Reference Checks** - Talk to similar health systems
5. **Negotiate** - Use framework to compare apples-to-apples

---

*Framework v1.0 - November 2025*
*Author: Alex Stinard, MD*
