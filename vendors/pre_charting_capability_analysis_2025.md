# AI Pre-Charting & Patient Context Capabilities - 2025 Analysis

## Executive Summary

AI pre-charting represents the next frontier beyond ambient documentation, shifting the value proposition from "during encounter" to "before encounter" workflow optimization. This analysis examines vendor capabilities, technology approaches, and clinical outcomes in the rapidly evolving pre-charting landscape.

---

## 1. What Is AI Pre-Charting

### Definition
AI pre-charting automates the preparation of patient information before a clinical encounter, providing clinicians with contextually relevant summaries, clinical priorities, and care gaps without manual chart review.

### Core Components

| Component | Description | Clinical Value |
|-----------|-------------|----------------|
| **Patient Summary** | Condensed view of relevant history | Rapid orientation before encounter |
| **Chart Prep Automation** | AI-generated synopsis from EHR data | Eliminates manual chart review |
| **History Surfacing** | Relevant past encounters, diagnoses, procedures | Context for current presentation |
| **Problem List Maintenance** | AI-suggested updates to active conditions | Accuracy of clinical record |
| **Care Gap Identification** | Missing screenings, overdue tests | Proactive care opportunities |
| **Pre-Visit Intelligence** | Chief complaint prediction, likely discussion topics | Anticipatory preparation |

### Why Pre-Charting Matters

Traditional chart review burden:
- **14.1 minutes** average prep time for complex patients (AAFP study)
- Clinicians spend **16 minutes per encounter** on EHR tasks (beyond visit time)
- Chart complexity increases with chronic disease, multiple providers, external records

Pre-charting AI addresses the "information overload" problem: too much data, not enough actionable insight.

---

## 2. Vendor Capabilities Comparison

### 2.1 Ambience Healthcare - Patient Recap

**Status:** First ambient AI platform with comprehensive pre-charting (June 2025)

| Feature | Capability |
|---------|------------|
| **Patient Recap** | Pre-visit chart summarization with specialty-specific tailoring |
| **View Options** | Chronological OR problem-based (configurable) |
| **Specialty Support** | 200+ specialties including oncology, psychiatry, ED |
| **Launch** | GA at St. Luke's Health System, June 2025 |

**Differentiator:** First ambient AI to cover full encounter lifecycle (pre, during, post).

**Clinical Results (Cleveland Clinic pilot):**
- 25,000 encounters across 20 specialties
- 80% documentation acceptance rate
- 67% reported reduced cognitive burden
- Nephrology: 99% adoption; Urology: 55% (lowest)

**Source:** [Ambience Healthcare](https://www.ambiencehealthcare.com/blog/ambience-healthcare-s-patient-recap-offers-clinicians-the-first-chart-summarization-technology-from-an-ambient-ai-platform)

---

### 2.2 DeepScribe - AI Pre-Charting

**Status:** Oncology-focused pre-charting leader

| Feature | Capability |
|---------|------------|
| **Data Sources** | EHR + referrals + clinical notes + labs + imaging + prior visit summaries |
| **Output** | Structured pre-chart with clinical priorities and chief complaints |
| **Specialty Focus** | Oncology-optimized (40% of US cancer visits use DeepScribe) |
| **Context Awareness** | Pulls forward longitudinal care journey |

**Key Capability:** Synthesizes structured EHR fields AND unstructured PDFs into contextual pre-visit views.

**Technology Approach:**
- Specialty-specific context awareness
- Adapts information surfacing to visit type (consult vs. follow-up)
- Reduces note redundancy by incorporating prior visit context

**KLAS Score:** 98.8 overall performance (early 2025)

**Sources:** [DeepScribe Pre-Charting](https://www.deepscribe.ai/solutions/ai-medical-scribe/pre-charting), [DeepScribe Oncology](https://www.deepscribe.ai/resources/the-critical-role-of-ai-pre-charting-in-cancer-care)

---

### 2.3 Nabla - Context-Aware Agent

**Status:** Agentic AI with pre-charting infrastructure

| Feature | Capability |
|---------|------------|
| **Pre-Charting** | Patient summaries from historical EHR data |
| **Context-Aware Agent** | Expands pre-charting to smarter documentation, orders, EHR commands |
| **Customization** | Specialty and organization-specific agent configuration |
| **Scale** | 85,000+ clinicians, 20M annual encounters |

**Technology Platform:**
- Built on pre-charting infrastructure as foundation for broader agentic capabilities
- Agents understand patient context, structure documentation, extract medical coding
- Deep customization per organization/specialty/clinician

**EHR Integration:** Epic, Cerner, athenahealth, NextGen, Greenway

**Funding:** $70M Series C (June 2025), $120M total

**Source:** [Nabla Series C](https://www.prnewswire.com/news-releases/nabla-raises-70m-series-c-to-deliver-agentic-ai-to-the-heart-of-clinical-workflows-bringing-total-funding-to-120m-302483646.html)

---

### 2.4 Navina - Chart Review Specialist

**Status:** #1 KLAS 2025 for Clinician Digital Workflow (2nd consecutive year)

| Feature | Capability |
|---------|------------|
| **AI Chart Review** | Reviews entire chart including scanned documents |
| **Output** | Problem-oriented summary with missing diagnoses and care gaps |
| **Coding** | Billing and risk adjustment code suggestions |
| **Trust** | 84% physician acceptance of diagnosis recommendations |

**Clinical Results (AAFP Independent Study):**

| Metric | Before AI | After AI | Improvement |
|--------|-----------|----------|-------------|
| Prep Time (complex patients) | 14.1 min | 5.5 min | **61% reduction** |
| Chart Review Burden | Baseline | -30% | 30% reduction |
| Burnout | Baseline | -23% | 23% reduction |
| Confidence/Preparedness | Baseline | +45% | 45% increase |
| Care Gap Identification | 72% | 93% | 21 point improvement |

**Scale:** 1,800 providers, 700,000 patient encounters studied

**Customers:** Tampa General Hospital, major primary care networks

**Focus:** Primary care, value-based care, HCC recapture

**Sources:** [Navina Chart Review](https://www.navina.ai/products/chart-review), [AAFP Study](https://www.aafp.org/family-physician/practice-and-career/administrative-simplification/chart-review/technologies-chart-review-burden.html)

---

### 2.5 Abridge - Inpatient Pre-Charting

**Status:** Expanding from outpatient to inpatient with pre-charting

| Feature | Capability |
|---------|------------|
| **Abridge Inside for Inpatient** | Pre-charting + post-charting + patient switching |
| **Integration** | Epic Haiku (mobile) + Hyperspace (desktop) |
| **Note Types** | H&P, progress notes, consult notes |
| **Languages** | 28+ languages, 55+ specialties |

**Launch:** June 2025 via Epic Workshop co-development program

**Patient Visit Summary (PVS):**
- AI-generated at 8th grade reading level
- Real-time generation for immediate patient access
- Addresses 40-80% medical information forgotten immediately after visits

**Sources:** [Abridge Inpatient](https://www.fiercehealthcare.com/health-tech/abridge-launches-gen-ai-tool-inpatient-clinicians-adds-outpatient-orders-feature), [Patient Visit Summaries](https://www.abridge.com/blog/patient-visit-summaries--now-generated-in-real-time)

---

### 2.6 Nuance/Microsoft - DAX Copilot

**Status:** Market leader, chart prep via workflow integration

| Feature | Capability |
|---------|------------|
| **Order Suggestions** | Surfaces orders from ambient recording for Epic review |
| **Referral Letters** | One-click outputs from conversation |
| **After-Visit Summaries** | Auto-generated patient instructions |
| **Trained On** | 15+ million encounters |

**Limitations:** Search results did not reveal a dedicated "pre-charting" feature comparable to Ambience Patient Recap or DeepScribe. Primary focus remains on ambient documentation during/after encounter.

**Pricing:** ~$600/provider/month (third-party reseller signals)

**Source:** [Nuance DAX Copilot](https://www.nuance.com/healthcare/dragon-ai-clinical-solutions/dax-copilot.html)

---

### 2.7 Suki AI - Chart Q&A

**Status:** Voice-first assistant with chart interrogation

| Feature | Capability |
|---------|------------|
| **Pre-Charting** | Patient summaries, lab summarization |
| **Chart Q&A** | Clinicians ask for specific data (last A1c, recent imaging, med gaps) |
| **Ambient Order Staging** | Speak prescription orders, Suki structures and stages |
| **Integration** | Epic, Oracle Health, athenahealth, MEDITECH (deepest integrations) |

**Pricing:** $299/month (Compose), $399/month (Assistant)

**Differentiator:** Bidirectional EHR integration - pulls chart data AND writes finished notes back (no copy/paste).

**Source:** [Suki AI](https://www.suki.ai/), [Suki Review](https://www.trytwofold.com/compare/suki-ai-review)

---

### 2.8 Notable Health - AI Agents for Operations

**Status:** Operational AI platform with chart review capabilities

| Feature | Capability |
|---------|------------|
| **Pre-Visit Chart Review** | AI agent reviews before encounter |
| **HCC Chart Review** | Risk adjustment coding |
| **Care Gap Closure** | AI identifies and acts on gaps |
| **Flow Builder** | Low-code agent configuration |

**Scale:** 12,000+ sites, 1M+ workflows automated daily

**Focus:** Operations-heavy (registration, scheduling, authorizations) with clinical AI layered on.

**Customers:** Intermountain Health, MUSC, North Kansas City Hospital

**Source:** [Notable Health](https://www.notablehealth.com/)

---

### 2.9 Epic Native - Art for Clinicians (Coming 2026)

**Status:** In development, limited availability early 2026

| Feature | Capability |
|---------|------------|
| **Chart Prep** | AI analyzes recent patient data, highlights important updates |
| **Pre-Visit Prep Agents** | Chat with patients, identify missing tasks, schedule/complete, create summary |
| **Patient Search** | Natural language search of free text (November 2025) |
| **Art Assistant** | Anticipates needed info, pulls trends, updates history, places orders |

**Timeline:**
- November 2025: Free text search capability
- Early 2026: Note-drafting (ambient scribe equivalent)
- November 2026: Additional features

**Threat Level:** Significant - Epic building native AI challenges all third-party vendors.

**Source:** [Epic AI for Clinicians](https://www.epic.com/software/ai-clinicians/), [Epic UGM 2025](https://www.fiercehealthcare.com/health-tech/epic-unveils-major-ai-features-ai-charting-microsoft-cosmos-ai-risk-prediction-and-rcm)

---

### 2.10 Stanford ChatEHR (Research/Pilot)

**Status:** Pilot stage, emergent technology

| Feature | Capability |
|---------|------------|
| **Chat Interface** | Clinicians ask questions of medical records |
| **Chart Summary** | Automatic summarization of entire chart |
| **Data Retrieval** | Specific data points on demand |
| **Use Case** | ED rapid orientation to complex patients |

**Value:** "When a patient comes to the emergency room, the admitting doctor needs to quickly understand their whole story—not just current symptoms, but prior history, medications, side effects, and surgeries."

**Source:** [Stanford ChatEHR](https://med.stanford.edu/news/all-news/2025/06/chatehr.html)

---

## 3. Technology Approaches

### 3.1 Knowledge Graphs for Patient Context

**Emerging Standard:** Knowledge graphs provide structured relationships across patient data domains.

| Vendor | Knowledge Graph Capability |
|--------|---------------------------|
| **Commure/Augmedix** | Multi-agent orchestration with knowledge graph memory, durable across encounters |
| **Oracle Health** | Oracle Knowledge Graph maps diagnoses, labs, medications, procedures, payer rules |
| **DR.KNOWS (Research)** | UMLS-based knowledge graph integrated with LLMs for diagnosis prediction |

**Oracle's Approach:**
- Maps relationships across healthcare domains
- Enables semantic understanding (e.g., "heart attack" = "myocardial infarction")
- Powers AI tools for terminology normalization

**Research Direction:** DR.KNOWS system (2025) integrates UMLS knowledge graphs with LLMs, retrieving contextually relevant paths aligned with patient-specific information to improve diagnostic accuracy.

**Sources:** [Oracle AI Strategy](https://distilinfo.com/hospitalit/2025/09/11/oracles-ai-strategy/), [DR.KNOWS Study](https://ai.jmir.org/2025/1/e58670)

---

### 3.2 EHR Data Aggregation

**Data Sources Aggregated:**

| Source Type | Examples | Aggregation Challenge |
|-------------|----------|----------------------|
| **Structured EHR** | Diagnoses, medications, labs, vitals | Standard but siloed |
| **Unstructured EHR** | Clinical notes, consult letters | NLP extraction required |
| **Scanned Documents** | Outside records, faxed referrals | OCR + NLP |
| **Imaging Reports** | Radiology, pathology | Report parsing |
| **Claims Data** | Payer-submitted encounter history | Cross-system integration |

**DeepScribe Approach:** Synthesizes both structured EHR fields AND unstructured PDFs.

**Navina Approach:** Reviews entire chart including labs, diagnostics, referrals, consult notes, discharge summaries, and scanned documents.

---

### 3.3 External Data Integration (HIE, Claims)

**Health Information Exchange (HIE):**
- ONC Patient Matching, Aggregating, and Linking project using APIs
- FHIR standard enables flexible data pulling from EHR into third-party software
- CommonWell, Carequality networks provide cross-organization data

**Claims Integration:**
- Epic Healthy Planet: Aggregates clinical, claims, and SDOH data
- Oracle: 120M real-world data records with longitudinal patient information including genomic data

**PGHD Integration Challenges:**
- Technical infrastructure gaps in ambulatory care
- Workflow integration barriers
- Patient burden vs. clinical value tradeoff

**Source:** [AHRQ PGHD Guide](https://digital.ahrq.gov/health-it-tools-and-resources/patient-generated-health-data-i-patient-reported-outcomes/practical-guide)

---

### 3.4 Longitudinal Patient View

**Why Longitudinal Context Matters:**

Stanford HAI released de-identified longitudinal EHR datasets (25,991 patients, 441,680 visits, 295M clinical events) specifically because:

> "Current medical datasets fail to reflect the full scope of past and future health information in real-world EHRs. Providing such longitudinal health context is essential for training multimodal models to understand complex, long-term health patterns, such as managing chronic diseases or cancer treatment planning."

**KGDNet Research:** Uses longitudinal EHR data + Drug-Drug Interaction knowledge to construct admission-wise knowledge graphs for each patient, enabling medicine recommendations that account for medical history (not just current admission).

**Source:** [Stanford HAI Longitudinal EHR](https://hai.stanford.edu/news/advancing-responsible-healthcare-ai-longitudinal-ehr-datasets)

---

## 4. Data Sources for Pre-Charting

### 4.1 EHR Historical Data
- Problem lists, diagnoses (ICD-10)
- Procedure history (CPT)
- Prior visit notes and assessments
- Discharge summaries

### 4.2 Labs and Imaging
- Laboratory results with trends
- Imaging reports and findings
- Pathology results

### 4.3 Medications
- Active medication list
- Allergy and adverse reaction history
- Medication reconciliation data

### 4.4 External Records
- HIE data (CommonWell, Carequality)
- Referral letters and consult notes
- Transferred records (scanned PDFs)
- Claims data from payers

### 4.5 Patient-Reported Data (PGHD/PRO)
- Patient portal questionnaires
- Remote monitoring device data
- Wearable-generated health data
- Pre-visit symptom checkers

**Integration Reality:**
> "Despite significant progress in digital health technologies, integration across platforms remains limited. Current systems are frequently characterized by fragmented data silos, inadequate interoperability, and insufficient personalization."

**Source:** [PMC PGHD Study](https://pmc.ncbi.nlm.nih.gov/articles/PMC11141850/)

---

## 5. Specialty-Specific Applications

### 5.1 Primary Care (Chronic Disease Management)

**Challenge:** Managing heterogeneous populations with concurrent chronic diseases and polypharmacy.

**AI Value:**
- Chronic disease trending (A1c, BP, weight over time)
- Preventive care gap closure
- HCC recapture for risk adjustment

**Navina Results:** 61% reduction in prep time, 93% care gap identification (vs. 72% baseline)

**Source:** [AAFP AI Study](https://www.aafp.org/family-physician/practice-and-career/administrative-simplification/chart-review/technologies-chart-review-burden.html)

---

### 5.2 Oncology (Treatment History)

**Challenge:** Complex, longitudinal care with multiple treatment modalities, clinical trials, and evolving disease status.

**DeepScribe Oncology Pre-Charting:**
- Synthesizes data from disparate sources
- Creates contextual view tailored to visit type (consult vs. follow-up)
- Helps oncologists quickly surface key context

**AI Agent Research (Nature Cancer 2025):**
- Autonomous AI agents using GPT-4 with multimodal precision oncology tools
- 91% correct clinical conclusions (vs. 30% GPT-4 alone)
- 87.5% appropriate tool use accuracy

**Sources:** [DeepScribe Oncology](https://www.deepscribe.ai/resources/the-critical-role-of-ai-pre-charting-in-cancer-care), [Nature Cancer AI Agent](https://www.nature.com/articles/s43018-025-00991-6)

---

### 5.3 Surgery (Pre-Operative Requirements)

**AI Applications:**
- Risk prediction accuracy improvement
- Imaging analysis refinement
- Virtual surgical training/planning
- Treatment strategy optimization (systemic therapy vs. radiotherapy vs. surgery)

**Challenge:** Initial treatment strategy formulation is the most pivotal AI touchpoint - directly influences patient management.

**Source:** [AI in Surgical Oncology](https://www.sciencedirect.com/science/article/pii/S2950261625000470)

---

### 5.4 Emergency Medicine

**Challenge:** Rapid orientation to unknown patients with time-sensitive presentations.

**ChatEHR Value Proposition:**
> "When a patient comes to the emergency room, the admitting doctor needs to quickly understand their whole story... Finding all this information during time-sensitive cases is intensive work."

**Adoption:** ED departments showed highest AI documentation adoption alongside mental health and primary care.

---

### 5.5 Psychiatry/Mental Health

**Challenge:** High documentation burden, longitudinal therapeutic relationships.

**Adoption:** Mental health departments among highest adoption of AI documentation tools.

**Ambience:** Specifically calls out psychiatry as "complex and under-served domain" with specialty support.

---

## 6. Outcomes and Evidence

### 6.1 Time Savings

| Organization | Tool | Time Savings | Source |
|--------------|------|--------------|--------|
| TPMG (Kaiser) | AI Scribes | **15,791 hours** total (1,794 workdays) | [AMA](https://www.ama-assn.org/practice-management/digital-health/ai-scribes-save-15000-hours-and-restore-human-side-medicine) |
| TPMG | AI Scribes | **1 hour/day** average per physician | [Permanente](https://permanente.org/analysis-ai-scribes-save-physicians-time-improve-patient-interactions-and-work-satisfaction/) |
| John Muir Health | AI Charting | **34 minutes/day** on notes | [EpicShare](https://www.epicshare.org/share-and-learn/john-muir-upmc-ai-charting) |
| UPMC | AI Charting | **~2 hours/day** "pajama time" reduction | [EpicShare](https://www.epicshare.org/share-and-learn/john-muir-upmc-ai-charting) |
| AAFP Study (Navina) | Chart Review AI | **61% reduction** in prep time (14.1→5.5 min) | [AAFP](https://www.aafp.org/family-physician/practice-and-career/administrative-simplification/chart-review/technologies-chart-review-burden.html) |

---

### 6.2 Completeness Improvement

| Metric | Before AI | After AI | Source |
|--------|-----------|----------|--------|
| Care Gap Identification | 72% | 93% | AAFP/Navina Study |
| Diagnosis Recommendation Acceptance | N/A | 84% | Navina |
| Confidence/Preparedness | Baseline | +45% | AAFP/Navina Study |

---

### 6.3 Clinician Satisfaction

| Metric | Result | Source |
|--------|--------|--------|
| Improved Patient Communication | 84% positive | [Permanente](https://permanente.org/analysis-ai-scribes-save-physicians-time-improve-patient-interactions-and-work-satisfaction/) |
| Improved Work Satisfaction | 82% positive | Permanente Study |
| Undivided Patient Attention | 90% (vs 49% baseline) | UChicago Medicine |
| Kaiser User Ratings | 47% 5-star, 31% 4-star | Kaiser AI Rollout |
| Reduced Cognitive Burden | 67% report improvement | Cleveland Clinic/Ambience |

---

### 6.4 Care Quality Impact

| Metric | Finding | Source |
|--------|---------|--------|
| Patient Perception - Less Computer Time | 47% noticed reduction | Permanente Study |
| Patient Perception - More Direct Conversation | 39% noticed increase | Permanente Study |
| Patient Visit Quality | 56% positive, 0% negative | Permanente Study |
| Burnout Reduction | 23-26% | Navina, Nabla |
| Physician Turnover | 44% reduction | John Muir Health |

---

### 6.5 Who Benefits Most

**Counterintuitive Finding:**

> "Those who benefited the most were not their tech-savvy early adopters, as those individuals had typically already optimized their documentation processes. Instead, the clinicians experiencing the greatest benefits were those who had not yet optimized their EHR-based clinical documentation workflows, were consistently behind in notes, or spent more time in conversation with their patients."

**Highest Adoption Departments:** Mental health, primary care, emergency medicine (historically high documentation burdens).

**Source:** [PHTI AI Adoption Report](https://phti.org/wp-content/uploads/sites/3/2025/03/PHTI-Adoption-of-AI-in-Healthcare-Delivery-Systems-Early-Applications-Impacts.pdf)

---

## 7. Vendor Capability Matrix

| Vendor | Pre-Chart Summary | Chart Q&A | Care Gaps | Longitudinal Context | External Data | Specialty-Specific |
|--------|-------------------|-----------|-----------|---------------------|---------------|-------------------|
| **Ambience** | ✓ Patient Recap | - | - | ✓ | - | ✓ 200+ |
| **DeepScribe** | ✓ Full | - | - | ✓ Strong | ✓ PDFs/Referrals | ✓ Oncology focus |
| **Nabla** | ✓ Context Agent | - | - | ✓ | - | ✓ |
| **Navina** | ✓ Full | ✓ | ✓ HCC/Gaps | ✓ | ✓ Scanned docs | Primary Care |
| **Abridge** | ✓ Inpatient | - | - | - | - | ✓ 55+ |
| **Nuance/MS** | Limited | - | - | - | - | ✓ |
| **Suki** | ✓ | ✓ Chart Q&A | - | - | - | ✓ |
| **Notable** | ✓ Agents | - | ✓ | - | - | Operations focus |
| **Epic Art** | Coming 2026 | ✓ Search | ✓ | TBD | TBD | TBD |

---

## 8. Strategic Implications

### 8.1 Market Trajectory

- **Pre-charting is the next battleground** after ambient documentation matures
- Vendors differentiating on "before encounter" value, not just "during encounter"
- Epic's native AI (Art) threatens all third-party vendors by 2026

### 8.2 Technology Convergence

- Knowledge graphs + LLMs emerging as architecture pattern
- Longitudinal context becoming essential differentiator
- Multi-modal data (structured + unstructured + scanned) required for complete picture

### 8.3 Evaluation Criteria for Pre-Charting

| Criterion | Questions to Ask |
|-----------|------------------|
| **Data Breadth** | What data sources are aggregated? External records? Scans? |
| **Specialty Adaptation** | Does output vary by specialty/visit type? |
| **Care Gap Intelligence** | Beyond summary - does it identify actionable gaps? |
| **Longitudinal Memory** | Does context persist across encounters? |
| **EHR Integration Depth** | Bidirectional? Pre-populated in workflow? |
| **Customization** | Can organizations/clinicians configure output? |

---

## 9. Key Sources

### Vendor Sources
- [Ambience Patient Recap](https://www.ambiencehealthcare.com/blog/ambience-healthcare-s-patient-recap-offers-clinicians-the-first-chart-summarization-technology-from-an-ambient-ai-platform)
- [DeepScribe Pre-Charting](https://www.deepscribe.ai/solutions/ai-medical-scribe/pre-charting)
- [Nabla Series C](https://www.prnewswire.com/news-releases/nabla-raises-70m-series-c-to-deliver-agentic-ai-to-the-heart-of-clinical-workflows-bringing-total-funding-to-120m-302483646.html)
- [Navina Chart Review](https://www.navina.ai/products/chart-review)
- [Abridge Inpatient Launch](https://www.fiercehealthcare.com/health-tech/abridge-launches-gen-ai-tool-inpatient-clinicians-adds-outpatient-orders-feature)
- [Nuance DAX Copilot](https://www.nuance.com/healthcare/dragon-ai-clinical-solutions/dax-copilot.html)
- [Suki AI](https://www.suki.ai/)
- [Notable Health](https://www.notablehealth.com/)
- [Epic AI for Clinicians](https://www.epic.com/software/ai-clinicians/)

### Research & Studies
- [AMA AI Scribes Time Savings](https://www.ama-assn.org/practice-management/digital-health/ai-scribes-save-15000-hours-and-restore-human-side-medicine)
- [Permanente AI Study](https://permanente.org/analysis-ai-scribes-save-physicians-time-improve-patient-interactions-and-work-satisfaction/)
- [AAFP Chart Review Technologies](https://www.aafp.org/family-physician/practice-and-career/administrative-simplification/chart-review/technologies-chart-review-burden.html)
- [Stanford ChatEHR](https://med.stanford.edu/news/all-news/2025/06/chatehr.html)
- [Stanford HAI Longitudinal EHR](https://hai.stanford.edu/news/advancing-responsible-healthcare-ai-longitudinal-ehr-datasets)
- [DR.KNOWS Knowledge Graph Study](https://ai.jmir.org/2025/1/e58670)
- [PHTI AI Adoption Report](https://phti.org/wp-content/uploads/sites/3/2025/03/PHTI-Adoption-of-AI-in-Healthcare-Delivery-Systems-Early-Applications-Impacts.pdf)

### Market Intelligence
- [Menlo Ventures State of AI 2025](https://menlovc.com/perspective/2025-the-state-of-ai-in-healthcare/)
- [Cleveland Clinic Ambience Selection](https://www.fiercehealthcare.com/ai-and-machine-learning/cleveland-clinic-chooses-ambience-ai-scribe)
- [Epic UGM 2025 Announcements](https://www.fiercehealthcare.com/health-tech/epic-unveils-major-ai-features-ai-charting-microsoft-cosmos-ai-risk-prediction-and-rcm)

---

*Analysis compiled November 2025*
*Author: Healthcare AI Vendor Analysis Project*
