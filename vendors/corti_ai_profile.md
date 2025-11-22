# Corti AI - Vendor Research Profile

**Research Date:** November 2025
**Analyst:** Healthcare AI Vendor Analysis Framework
**Primary Focus:** Emergency/Triage AI, Ambient Documentation

---

## 1. Company Profile

| Field | Details |
|-------|---------|
| **Company Name** | Corti ApS |
| **Founded** | 2016 |
| **HQ Location** | Copenhagen, Denmark |
| **US Office** | New York (opened for US expansion) |
| **Total Funding** | $93M across 8 rounds |
| **Latest Round** | Series B - $60M (September 2023) |
| **Key Investors** | Prosus Ventures (co-lead), Atomico (co-lead), Eurazeo, EIFO, Chr. Augustinus Fabrikker |
| **Employees** | ~53 (as of Nov 2024) |
| **Founders** | Lars Maaløe, Andreas Cleve (also: Michael Reibel Boesen, Anders Friis) |
| **Revenue Model** | API-based pricing, enterprise licensing |
| **Target Market** | Enterprise health systems, emergency services, public safety |

### Funding History
| Round | Amount | Date | Lead Investors |
|-------|--------|------|----------------|
| Seed | $5M | 2019 | - |
| Series A | $27M (~€22.82M) | September 2021 | - |
| Series B | $60M | September 2023 | Prosus Ventures, Atomico |

---

## 2. Foundation Model & AI Stack

| Field | Details |
|-------|---------|
| **Primary LLM** | Proprietary healthcare-specific foundation models |
| **Multi-Model Strategy** | Yes - Solo, Ensemble, Symphony (task-based routing) |
| **ASR Provider** | Proprietary medical speech recognition |
| **ASR Medical Tuning** | Yes - trained on 100M+ patient interactions |
| **Agentic Architecture** | Multi-agent with FactsR reasoning layer |
| **Tool Use** | EHR read/write, note composition, clinical fact extraction |
| **Memory / Context** | Real-time streaming with contextual awareness |
| **Knowledge Graph** | Clinical ontology mapping, specialty-specific |
| **RAG Implementation** | Integrated into FactsR extraction/reasoning pipeline |
| **Fine-Tuning** | Healthcare-specific "AI residency" training approach |
| **On-Prem Option** | Yes - sovereign cloud options, multi-cloud deployment |

### Proprietary Foundation Models

| Model | Purpose | Key Capability |
|-------|---------|----------------|
| **Solo** | Audio reasoning | Dictation, transcription, diarization (10+ languages) |
| **Ensemble** | Documentation | 25% more concise than general-purpose AI |
| **Symphony** | Clinical support | Real-time support 35x faster than GPT-4 |

### FactsR - Clinical Reasoning Layer (June 2025)
- **Extract**: Pull clinically relevant facts in real-time as conversation unfolds
- **Refine**: Evaluate each fact using specialized reasoning agents
- **Compose**: Build final note using only validated facts (SOAP format)
- **Performance**: 49% reduction in missing content, 86% reduction in extraneous detail, 65% reduction in "note bloat"

---

## 3. Clinical Capabilities

### 3a. Emergency/Triage Focus (Primary Specialty)

| Field | Details |
|-------|---------|
| **Out-of-Hospital Cardiac Arrest Detection** | 84.1% sensitivity (vs. 72.5% human dispatchers) |
| **Cardiac Arrest Time-to-Recognition** | 44 seconds (vs. 54 seconds human) |
| **Undetected OHCA Reduction** | 43% fewer missed cases |
| **Stroke Detection** | 13% faster identification |
| **911/Emergency Call Analysis** | Real-time speech analysis during emergency calls |
| **Triage Decision Support** | Protocol-based guidance for dispatchers |

### 3b. Ambient Documentation

| Field | Details |
|-------|---------|
| **Real-time vs. Post-visit** | Real-time |
| **Specialties Supported** | Emergency medicine, primary care, expanding |
| **Note Types** | SOAP, customizable formats |
| **Template Customization** | Per-provider, per-specialty, per-org |
| **Multi-language** | 10+ languages supported |
| **Diarization** | Multi-speaker identification |
| **Time Savings** | Up to 2 hours/day per clinician |
| **Admin Reduction** | Up to 80% reduction in documentation time |

### 3c. Beyond Ambient

| Capability | Status |
|------------|--------|
| Auto-Coding | Via structured fact extraction |
| CDI | Real-time documentation support |
| Pre-Charting | Patient summary capabilities |
| After-Visit Summary | Patient-facing outputs |
| Care Navigation | Workflow integration |

---

## 4. EHR Integration

| Field | Details |
|-------|---------|
| **EHRs Supported** | Epic, Cerner, and others |
| **Integration Standards** | SMART on FHIR, direct API |
| **Epic Integration** | Ambient Voice Recognition workflow, SmartSections |
| **Epic Apps** | Haiku, Canto (iOS) supported |
| **Cerner Integration** | Yes - streamlined workflows |
| **Bi-directional** | Yes - read AND write |
| **API Architecture** | API-first, modular framework |

### Epic-Specific Features
- Conversational audio capture from Epic mobile apps
- AI-generated note output directly into Epic SmartSections
- Clinician-customizable SmartSection templates
- Embedded within Epic's best practice ambient documentation workflow

---

## 5. User Experience

| Field | Details |
|-------|---------|
| **Platforms** | Web, Desktop, iOS, Android, Apple Watch |
| **Deployment Options** | Embedded (in-EHR) or standalone |
| **Interface** | Corti Assistant - next-gen ambient AI solution |
| **Voice Commands** | Yes |
| **Provider Feedback** | Accept/edit/reject tracking |
| **Self-Onboarding** | Available for some deployments |

---

## 6. Safety & Trust

| Field | Details |
|-------|---------|
| **Guardrails Architecture** | FactsR reasoning layer with validation |
| **Hallucination Mitigation** | Fact-based extraction with source grounding |
| **Audit Trail** | Full traceability |
| **Human-in-Loop** | Dispatcher/clinician review |
| **Citation to Source** | Facts linked to transcript |
| **Confidence Scoring** | Via reasoning agent evaluation |

---

## 7. Security & Compliance

| Certification | Status |
|---------------|--------|
| **HIPAA** | Compliant |
| **GDPR** | EU and UK compliant |
| **SOC 2 Type II** | Certified |
| **ISO 27001** | Certified |
| **ISAE 3000 Type II** | Passed (June 2025) - privacy/data protection |
| **BSI C5 Type II** | Passed (June 2025) - German cloud compliance |
| **NIS2** | Compliant |
| **DORA** | Compliant |
| **UK Cyber Essentials** | Certified |
| **UK DSPT** | Compliant |
| **EU-US Data Privacy Framework** | Aligned (incl. Swiss-US, UK-US extensions) |

### Data Security Infrastructure
- **Encryption**: FIPS-compliant AES encryption at rest, TLS 1.2+ in transit
- **Key Management**: Per-customer encryption keys
- **Access Control**: Role-based with Azure AD integration
- **Audit Logging**: Full audit trail

### Sovereign Cloud (July 2025)
- Europe's first sovereign healthcare AI infrastructure
- Operates across any cloud or on-premises data center
- Provider exit flexibility for regulatory/geopolitical needs
- Designed for strictest data privacy regimes (Switzerland, Germany, France)

---

## 8. Customers & Case Studies

### Public Safety / Emergency Services

| Customer | Use Case | Results |
|----------|----------|---------|
| **Copenhagen EMS** | Cardiac arrest detection | 10% more heart attacks identified; 40% reduction in undetected OHCA |
| **Seattle Fire Department** | 911 triage | 50%+ increase in nurse triage referrals; 13% faster stroke detection |
| **NHS Wales** | Emergency call analysis | AI implementation for critical illness detection |
| **EENA (European Emergency Number Association)** | Multi-city trials | Rolled out to Munich, Milan, Paris, London for trials |

### Healthcare Systems

| Customer/Partner | Details |
|------------------|---------|
| **NHS (UK)** | 76 NHS Trusts via BigHand partnership (40,000 frontline workers) |
| **BigHand** | Strategic partnership for NHS distribution |
| **Voicepoint** | Swiss medical documentation partner (sovereign AI) |
| **Wolters Kluwer Health** | Clinical decision support partnership (Feb 2025) |
| **MARIS Healthcare** | Strategic partnership (April 2025) |
| **Northland Systems** | US distribution partner |

### Market Reach
- US: 100,000+ patient interactions daily across all 50 states
- Goal: 100 million patient interactions in US by 2025

---

## 9. Geographic Presence

| Region | Status |
|--------|--------|
| **Denmark** | Headquarters, origin market |
| **Europe** | UK (NHS), Germany, France, Switzerland, Nordics |
| **United States** | Rapid expansion, NY headquarters, all 50 states |
| **Middle East** | Expansion target |

### European Market Strategy
- Switzerland chosen as first sovereign AI market (strictest regulations)
- C5 certification grants access to German healthcare market
- GDPR compliance enables EU-wide operations
- Swiss model enables faster expansion to France, Germany, Middle East

---

## 10. Clinical Validation & Research

### Peer-Reviewed Studies

| Study | Publication | Findings |
|-------|-------------|----------|
| Copenhagen OHCA Study | Resuscitation Journal | AI sensitivity 84.1% vs. human 72.5%; recognition 44s vs. 54s |
| Randomized Clinical Trial (2021) | PubMed | AI recognition superior but dispatcher compliance variable |
| Stroke Detection Study | PMC | Significant time reduction in stroke identification |

### Key Metrics from Clinical Use
- **Cardiac Arrest Diagnosis**: 93% accuracy (vs. 73% human)
- **Time Savings**: 30 seconds faster than human dispatchers
- **OHCA Reduction**: 43% fewer undetected cases
- **Nurse Triage Referrals**: 50%+ increase (Seattle FD)

---

## 11. KLAS Research Status

| Field | Status |
|-------|--------|
| **KLAS Rating** | Not found in public KLAS reports |
| **KLAS Category** | Emergency/triage AI (emerging category) |
| **Comparable Vendors Rated** | Beckman Coulter TriageGO has KLAS First Look (Aug 2024) |

**Note:** Corti does not appear to have published KLAS ratings. This may be due to:
- Focus on emergency services (not traditional EHR-integrated clinical AI)
- European-first market strategy
- KLAS coverage gaps in emergency/triage AI category

---

## 12. Roadmap & Future (2025-2026)

### 2025 Announced Launches
| Date | Launch |
|------|--------|
| January 2025 | Specialized healthcare AI infrastructure (Solo, Ensemble, Symphony) |
| February 2025 | Wolters Kluwer Health partnership for clinical decision support |
| April 2025 | MARIS Healthcare strategic partnership |
| June 2025 | FactsR clinical reasoning layer |
| July 2025 | Europe's first sovereign healthcare AI infrastructure |

### Strategic Direction
- **API-First Platform**: Dedicated growth team for API customer expansion
- **Developer Experience**: Console and playground product development
- **Advanced NLP**: Improved handling of diverse linguistic/acoustic environments
- **False Positive Reduction**: Ongoing accuracy improvements
- **Global Expansion**: Switzerland → Germany → France → Middle East

### 2025 Goals
- 100 million patient interactions in US
- Expanded sovereign cloud to multiple European markets
- Deeper EHR integrations

---

## 13. Competitive Positioning

### Strengths
1. **Deep Emergency Medicine Expertise** - Originated in OHCA detection, validated research
2. **Proprietary Foundation Models** - Purpose-built for healthcare, not adapted general-purpose AI
3. **European Compliance Leadership** - GDPR, C5, sovereign cloud capabilities
4. **Clinical Validation** - Published peer-reviewed research
5. **Real-time Performance** - 35x faster than GPT-4 for clinical tasks
6. **API-First Architecture** - Developer-friendly, flexible deployment

### Considerations
1. **KLAS Visibility** - Limited presence in traditional healthcare IT ratings
2. **US Market Position** - Still expanding (behind established US players)
3. **Company Size** - ~53 employees vs. larger competitors
4. **Specialty Breadth** - Strong in EM/triage, expanding in other specialties

### Differentiation
- "AI Residency" approach: specialized models trained exclusively on healthcare data
- FactsR reasoning layer: unique clinical fact extraction vs. generic summarization
- Sovereign cloud: regulatory compliance advantage in European markets
- Emergency medicine heritage: unique positioning vs. ambient-first competitors

---

## 14. Pricing

| Field | Details |
|-------|---------|
| **Pricing Model** | API-based, enterprise licensing |
| **Public Pricing** | Not publicly disclosed |
| **Contact** | Enterprise sales for custom quotes |

---

## 15. Sources

### Primary Sources
- [Corti Official Website](https://www.corti.ai/)
- [Corti Help Center - EHR Integration](https://help.corti.app/en/articles/10723547-integrating-corti-with-epic-ehr)
- [Corti API Documentation](https://docs.corti.ai/textgen/factsr)

### Funding & Company
- [Corti $60M Series B Announcement](https://www.corti.ai/stories/corti-raises-60m-in-series-b-funding-to-accelerate-healthcare-ai-innovation-and-expand-work-in-public-safety)
- [TechCrunch: Corti Raises $60M](https://techcrunch.com/2023/09/20/corti-an-ai-co-pilot-for-healthcare-clinicians-raises-60m/)
- [Tracxn: Corti Company Profile](https://tracxn.com/d/companies/corti/__0s9fLHIXnFrC5tD32K5PLq7c3jKthk5baNst_XJEMfI)

### Product Launches
- [Corti Launches Specialized Healthcare AI Infrastructure (Jan 2025)](https://www.corti.ai/news/corti-launches-specialized-healthcare-ai-infrastructure-challenging-industry-misuse-of-general-purpose-models)
- [FactsR Launch Announcement (June 2025)](https://www.prnewswire.com/news-releases/introducing-factsr-by-corti--the-first-clinical-reasoning-layer-for-ambient-ai-in-healthcare-302478475.html)
- [Sovereign Healthcare AI Infrastructure (July 2025)](https://www.corti.ai/news/corti-pioneers-europes-first-sovereign-healthcare-ai-infrastructure)

### Partnerships & Growth
- [Corti Key Partnerships and US Growth (Aug 2024)](https://www.corti.ai/news/corti-announces-key-partnerships-and-record-us-growth)
- [NHS BigHand Partnership](https://healthcare.bighand.com/resources/news/corti-partnership/)
- [Bloomberg: Corti US Expansion](https://www.bloomberg.com/news/videos/2024-09-11/corti-ai-s-expansion-into-the-us-market-video)

### Clinical Validation
- [EENA Report: OHCA Detection Using AI](https://eena.org/wp-content/uploads/2020_01_13_Corti_Report.pdf)
- [PubMed: Machine Learning OHCA RCT](https://pubmed.ncbi.nlm.nih.gov/33404620/)
- [Resuscitation Journal: Machine Learning for Cardiac Arrest](https://www.resuscitationjournal.com/article/S0300-9572(18)30975-4/fulltext)

### Compliance & Security
- [Corti Safety & Compliance](https://www.corti.ai/safety)
- [New Certifications Announcement](https://www.corti.ai/stories/how-corti-supports-medical-device-manufacturers-regulatory-ready-ai)

### Customer Stories
- [Seattle Fire Dept Triage Accuracy](https://www.corti.ai/stories/seattle-fire-dept-triaging-accuracy)
- [NHS Wales AI Implementation](https://www.corti.ai/stories/the-nhs-implements-artificial-intelligence-to-support-emergency-calls-in-wales)

---

*Profile Version: 1.0*
*Last Updated: November 2025*
