# Ramsay Health Care: AI Vendor Requirements Analysis

**Date:** November 2025
**Prepared for:** Strategic Technology Evaluation
**Scope:** Global operations across Australia, UK, France, Nordics, and Asia

---

## Executive Summary

Ramsay Health Care, as one of the world's largest private hospital operators with **530+ facilities** across **9 countries** and **90,000+ employees**, has uniquely complex requirements for AI vendor selection. Any AI solution—particularly clinical documentation AI—must navigate a web of jurisdictional compliance requirements, integrate with a diverse EHR landscape, support multiple languages, respect strict data sovereignty rules, and scale to support thousands of clinicians across 24/7 operations.

This analysis identifies the critical requirements an AI vendor must meet to successfully deploy across Ramsay's global footprint.

---

## 1. Multi-Jurisdiction Regulatory Requirements

### 1.1 Australia

#### Therapeutic Goods Administration (TGA)
| Requirement | Detail |
|------------|--------|
| **Regulatory Framework** | Software-based medical devices regulated under the Therapeutic Goods Act 1989 |
| **Registration** | Must be registered on the Australian Register of Therapeutic Goods (ARTG) unless exempt/excluded |
| **Classification** | Technology-agnostic approach; AI ambient documentation may qualify as medical device if it generates clinical interpretations |
| **Digital Scribe Guidance** | TGA guidance clarifies: if a scribe analyzes/interprets clinical conversations or generates diagnoses/recommendations not explicitly stated by the clinician, it is a medical device |
| **LLM Considerations** | When LLMs have a medical purpose and are supplied to Australians, they may be subject to medical device regulations |
| **Compliance Focus (2024)** | TGA actively monitoring unregistered SaMD and AI products; enforcement expected to increase |

**Key Source:** [TGA AI and Medical Device Software Guidance](https://www.tga.gov.au/how-we-regulate/manufacturing/manufacture-medical-device/manufacture-specific-types-medical-devices/artificial-intelligence-ai-and-medical-device-software)

#### Privacy Act 1988 & Australian Privacy Principles (APPs)
| Requirement | Detail |
|------------|--------|
| **Health Information** | Classified as "sensitive information" requiring stricter protection |
| **APP 8 (Cross-border)** | Organizations must ensure overseas data recipients adhere to Australian privacy standards |
| **My Health Records Act** | National health record data must remain within Australia |
| **2025 Changes** | National Health (Privacy) Rules 2025 commence April 2025 with enhanced privacy settings |
| **Coverage** | All organizations providing health services are covered regardless of size |

**Key Source:** [OAIC Health and Medical Research Guidance](https://www.oaic.gov.au/privacy/privacy-legislation/the-privacy-act/health-and-and-medical-research)

### 1.2 United Kingdom

#### NHS Standards & DTAC
| Requirement | Detail |
|------------|--------|
| **DTAC Compliance** | Digital Technology Assessment Criteria is the national baseline for digital health technologies |
| **Mandatory Status** | Although advisory nationally, practically required for NHS procurement; mandated by NHS England as procurement baseline from 2025 |
| **Assessment Areas** | Clinical Safety (DCB0129), Data Protection, Technical Security, Interoperability, Usability & Accessibility |
| **Clinical Safety Officer** | Appointment of CSO required for compliance |
| **Cybersecurity** | Penetration testing within 12 months, Cyber Essentials certification required |
| **AI-Specific** | Ambient scribe systems are candidates for MHRA's AI Airlock; require full DTAC and trust-level DPIA |

**Key Source:** [NHS DTAC Guidance](https://transform.england.nhs.uk/key-tools-and-info/digital-technology-assessment-criteria-dtac/how-to-use-the-dtac/)

#### UK GDPR & MHRA
| Requirement | Detail |
|------------|--------|
| **UK GDPR** | Post-Brexit alignment with EU GDPR via UK Data Protection Act 2018 |
| **Health Data (Article 9)** | Special category requiring explicit consent or qualifying exemption |
| **MHRA Strategy (2024)** | AI as Medical Device (AIaMD) must conform to UK Medical Devices Regulations 2002 |
| **Reclassification** | Many AI products in Class 1 to be "up-classified" for greater scrutiny |
| **2025 Guidance** | MHRA to publish cybersecurity and human factors guidance |

**Key Source:** [MHRA AI Regulatory Strategy](https://www.biosliceblog.com/2024/05/mhra-sets-out-its-ai-regulatory-strategy/)

### 1.3 European Union (France, Italy)

#### EU AI Act & MDR
| Requirement | Detail |
|------------|--------|
| **EU AI Act** | Regulation EU 2024/1689, approved March 2024 |
| **MDR Interaction** | AI systems with medical purpose regulated under MDR 2017/745 AND AI Act |
| **Classification** | AI healthcare software typically Class IIa, IIb, or III depending on risk |
| **High-Risk AI** | Most clinical AI classified as high-risk requiring QMS, data governance, transparency, human oversight |
| **GDPR Compliance** | Article 9 special category protections for health data |
| **Continuous Learning** | Self-learning AI models face certification challenges; notified bodies require validation controls |

**Key Source:** [Nature: Navigating the EU AI Act](https://www.nature.com/articles/s41746-024-01232-3)

#### France-Specific: HDS Certification
| Requirement | Detail |
|------------|--------|
| **Mandatory Certification** | HDS (Hébergeur de Données de Santé) required for hosting health data |
| **HDS v2.0 (May 2024)** | Revised framework with new data sovereignty requirements |
| **Data Localization** | Health data must be physically hosted exclusively within the EEA |
| **Transparency** | Must inform clients if data accessed remotely from outside EEA or subject to non-European laws |
| **ISO 27001+** | Builds on ISO 27001 with healthcare-specific requirements |
| **Certification Body** | Must obtain from COFRAC-approved body; valid 3 years with annual surveillance |

**Key Source:** [Hogan Lovells: French HDS Certification](https://www.hoganlovells.com/en/publications/health-data-hosting-the-new-french-hds-certification-has-been-released)

### 1.4 Nordic Countries (Sweden, Norway, Denmark)

| Requirement | Detail |
|------------|--------|
| **GDPR Compliance** | Full EU GDPR applies |
| **EHDS Regulation** | European Health Data Space entered force March 2025; impacts secondary use of health data |
| **National Variations** | Norway requires proactive regulation; others prioritize innovation |
| **DPA Cooperation** | Nordic DPAs joined forces on AI and children's data protection |
| **AI Sandbox** | Norwegian DPA operates regulatory sandbox for AI |
| **Registry Infrastructure** | Highly developed national registries with personal identity numbers enabling data linkage |

**Key Source:** [SCUP: AI and Healthcare in Nordic States](https://www.scup.com/doi/10.18261/nwr.9.2.5)

### 1.5 Asia (Malaysia, Indonesia)

Note: Ramsay divested Asian operations in December 2023 (sold to Columbia Asia Healthcare). Requirements included for context if re-entry considered.

#### Malaysia
| Requirement | Detail |
|------------|--------|
| **PDPA 2024 Amendment** | Enhanced Personal Data Protection Act effective 2025 |
| **Key Requirements** | Mandatory DPOs, 72-hour breach notification, data portability |
| **Health Data** | Falls within "sensitive personal data" category |
| **AI Regulation Gap** | PDPA does not yet regulate automated decision-making |
| **Penalties** | Up to RM1,000,000 |

**Key Source:** [FPF: Malaysia Data Protection Frameworks](https://fpf.org/blog/malaysia-charts-its-digital-course-a-guide-to-the-new-frameworks-for-data-protection-and-ai-ethics/)

#### Indonesia
| Requirement | Detail |
|------------|--------|
| **PDP Law (2022)** | Law No 27 of 2022 modeled on GDPR |
| **Healthcare Data** | MOH Regulation No 24/2022 allows digital medical records with certified cloud storage |
| **Data Residency** | ESO must have onshore data storage with MOH recommendation |
| **DPO Required** | For organizations processing sensitive data |

**Key Source:** [Chambers: Indonesia Data Protection 2025](https://practiceguides.chambers.com/practice-guides/data-protection-privacy-2025/indonesia/trends-and-developments)

---

## 2. EHR Integration Requirements

### 2.1 Diverse EHR Landscape by Region

| Region | Primary Systems | Key Considerations |
|--------|----------------|-------------------|
| **Australia** | WebPAS (Dedalus), MasterCare+ (Fujitsu), various EMRs | WebPAS predominant (252+ sites, 22,000 beds, 23% market share); FHIR adoption increasing |
| **UK** | Mix of private hospital systems | Must integrate with NHS systems for NHS-funded work |
| **France** | DMP (Dossier Médical Partagé) integration required | ASIP-Santé interoperability framework; Ramsay Services 2 patient portal |
| **Nordics** | Capio/Volvat brands; Welcome app (Sweden) | Doctrin platform for psychiatry digitalization; most digitally advanced |
| **Italy** | Single hospital facility | European standards apply |

**Key Source:** [Dedalus WebPAS](https://www.dedalus.com/anz/our-offer/products/web-patient-administration-system-webpas/)

### 2.2 FHIR-First Approach Requirements

| Requirement | Detail |
|------------|--------|
| **Standard** | HL7 FHIR R4 minimum; R5 preferred for new implementations |
| **Adoption Rate** | 78% of healthcare providers using FHIR report faster care coordination (HIMSS 2024) |
| **Australia** | WebPAS integrates with My Health Record, IHI; increasing FHIR resources |
| **France** | ANS financial penalties from 2025 for non-compliance with interoperability standards |
| **API Requirements** | RESTful APIs mandatory; ONC Cures Act bans information blocking |

**Key Source:** [Healthcare Interoperability Standards Guide 2024](https://www.getfocal.co/post/healthcare-interoperability-standards-complete-guide-2024)

### 2.3 Workflow Integration Patterns

| Setting | Workflow Requirements |
|---------|----------------------|
| **Acute Hospital** | Full EMR integration; real-time documentation; handover support; order entry |
| **Day Surgery** | Rapid turnaround workflows; pre-op/post-op documentation; same-day discharge summaries |
| **Mental Health** | Specialized templates; Elysium Healthcare (UK) requirements; outpatient psychiatry (France) |
| **Rehabilitation** | Progress notes; therapy documentation; outcome measures |
| **Primary Care** | Capio primary care (Nordics); high-volume encounters; preventive care documentation |

---

## 3. Language Requirements

### 3.1 Language Matrix by Region

| Language | Regions | Clinical Usage | Medical Terminology |
|----------|---------|---------------|---------------------|
| **English (AU)** | Australia | Primary | Australian medical terms, MBS items |
| **English (UK)** | United Kingdom | Primary | NHS terminology, British spellings |
| **French** | France (121 facilities) | Primary | French medical terminology |
| **Swedish** | Sweden (Capio) | Primary | Swedish + English medical terms mixed |
| **Norwegian** | Norway (Volvat) | Primary | Bokmål and Nynorsk variants |
| **Danish** | Denmark (Capio) | Primary | Danish medical terminology |
| **Italian** | Italy (1 hospital) | Primary | Limited scope |
| **Bahasa Indonesia** | Indonesia (divested) | If re-entry | Local medical terms |
| **Malay** | Malaysia (divested) | If re-entry | Local medical terms |

### 3.2 Multilingual AI Capabilities Required

| Capability | Requirement |
|-----------|-------------|
| **Speech Recognition** | Native support for all primary languages; accent recognition within each |
| **Medical Vocabulary** | 25+ clinical specialties per language; local medical terminology |
| **Dialect Support** | Norwegian Bokmål/Nynorsk; regional French accents |
| **Code-Switching** | Handle English medical terminology mixed with local language |
| **Translation** | After-visit summaries in patient's preferred language |

**Available Solutions:**
- **Augnito Omni**: Purpose-built for Nordic languages (Norwegian, Swedish, Danish, Finnish); 99.3% recognition accuracy; regional accent recognition
- **Speechmatics Medical Model**: Accent-independent; 93% clinical transcription accuracy
- **MultiMed**: Research dataset spanning Vietnamese, English, German, French, Mandarin

**Key Source:** [Augnito/MultiMed Research](https://arxiv.org/html/2409.14074v3)

---

## 4. Data Residency & Sovereignty Requirements

### 4.1 Data Residency Matrix

| Country | Requirement | Storage Location | Cross-Border Rules |
|---------|-------------|-----------------|-------------------|
| **Australia** | APP 8 compliance; My Health Records must stay onshore | Preferred: Australia | Requires adequate safeguards for offshore processing |
| **UK** | UK GDPR; adequacy with EU | UK or adequate countries | UK has EU adequacy decision |
| **France** | HDS v2.0 mandatory | EEA only | Remote access from non-EEA requires client notification |
| **Sweden** | EU GDPR | EEA | Standard GDPR transfer rules |
| **Norway** | EEA member (non-EU) | EEA | EHDS implementation pending |
| **Denmark** | EU GDPR | EEA | Standard GDPR transfer rules |
| **Italy** | EU GDPR | EEA | Standard GDPR transfer rules |

### 4.2 Adequacy Status for Key Third Countries

| Country | EU Adequacy | UK Adequacy | Australia APPs |
|---------|-------------|-------------|----------------|
| **United States** | Yes (DPF 2023) | Yes | Requires safeguards |
| **United Kingdom** | Yes | N/A | Yes (similar standards) |
| **Australia** | No | No | N/A |
| **Canada** | Partial (commercial) | Yes | Requires safeguards |
| **India** | No | No | Requires safeguards |

### 4.3 Vendor Infrastructure Requirements

| Requirement | Specification |
|------------|---------------|
| **Australia** | Local data center (Sydney/Melbourne preferred) |
| **UK** | UK-based or EU data center with UK adequacy |
| **France** | HDS-certified hosting provider; EEA-only storage |
| **Nordics** | EEA data center; preferably local for latency |
| **Global Vendor** | Multi-region deployment capability; data never leaves region |

### 4.4 Backup & Disaster Recovery

| Requirement | Specification |
|------------|---------------|
| **RPO** | < 1 hour for clinical data |
| **RTO** | < 4 hours for production systems |
| **Geographic Redundancy** | Within same jurisdiction (no cross-border DR that violates residency) |
| **Backup Encryption** | AES-256 minimum; key management within region |
| **Testing** | Annual DR testing with documented results |

---

## 5. Scale Requirements

### 5.1 Ramsay Global Scale

| Metric | Value |
|--------|-------|
| **Total Facilities** | 530+ (hospitals, clinics, surgical centers) |
| **Countries** | 9 (reduced from 11 post-Asia divestiture) |
| **Employees** | 90,000+ globally |
| **Australia** | 70+ hospitals; 35,000+ employees; 1M+ patients/year |
| **UK** | 22 private hospitals; 9 treatment centers; 3 neuro units |
| **France** | 121 facilities (110 hospitals) |
| **Nordics** | 50+ hospitals/clinics across Sweden, Norway, Denmark |
| **Italy** | 1 hospital (93 beds) |
| **Patient Volume** | 8.5M - 13M+ patients annually across network |

**Key Source:** [Ramsay Health Care 2025 Impact Report](https://www.marketscreener.com/news/ramsay-health-care-2025-impact-report-ce7d5ed9dc8cf622)

### 5.2 Clinician Scale Estimates

| Region | Estimated Clinicians | Employment Model |
|--------|---------------------|------------------|
| **Australia** | 15,000+ (doctors, nurses with documentation needs) | Mix of employed and visiting medical officers (VMOs) |
| **UK** | 5,000+ | Mix of employed and consulting |
| **France** | 20,000+ | Primarily employed |
| **Nordics** | 10,000+ | Primarily employed |
| **Total Addressable** | 50,000+ clinicians globally | Varied models |

### 5.3 Technical Scale Requirements

| Requirement | Specification |
|------------|---------------|
| **Concurrent Users** | Support 10,000+ simultaneous active sessions |
| **Transactions/Day** | 500,000+ clinical documentation events |
| **Peak Load** | Handle 3-5x normal load during shift changes |
| **Latency** | < 200ms response time for real-time transcription |
| **Uptime SLA** | 99.9% availability (8.76 hours/year downtime max) |
| **Geographic Distribution** | Low-latency access from all operating regions |

### 5.4 24/7 Operations Requirements

| Requirement | Detail |
|------------|--------|
| **Time Zones** | AEST/AEDT, GMT/BST, CET, SAST |
| **Shift Patterns** | 24/7/365 hospital operations |
| **Support Model** | Follow-the-sun support or regional support teams |
| **Maintenance Windows** | Rolling by region; no global downtime |
| **Incident Response** | < 15 minutes acknowledgment; < 1 hour resolution start for P1 |

---

## 6. Vendor Evaluation Framework

### 6.1 Critical Selection Criteria

| Category | Weight | Key Evaluation Points |
|----------|--------|----------------------|
| **Regulatory Compliance** | 25% | TGA registration (AU); DTAC/MHRA (UK); CE mark/MDR (EU); HDS certification (FR) |
| **Technical Capability** | 25% | FHIR integration; multi-language support; scalability; latency |
| **Data Security & Privacy** | 20% | ISO 27001; SOC 2; regional data residency; encryption; access controls |
| **Clinical Effectiveness** | 15% | Accuracy rates; specialty coverage; clinical validation studies |
| **Implementation & Support** | 10% | Local presence; implementation methodology; training; ongoing support |
| **Commercial** | 5% | TCO; pricing model; contract flexibility |

### 6.2 Must-Have Requirements (Deal Breakers)

1. **TGA Registration** (for Australia deployment) or clear pathway to registration
2. **HDS Certification** or HDS-certified hosting partner (for France deployment)
3. **DTAC Compliance** (for UK NHS-related work)
4. **FHIR R4 API** for EHR integration
5. **Multi-language Support** for English, French, Swedish, Norwegian, Danish at minimum
6. **Regional Data Residency** with no cross-border data transfers violating local requirements
7. **ISO 27001 Certification**
8. **Clinical Safety Case** documentation

### 6.3 Proof Points Required

| Area | Evidence Required |
|------|-------------------|
| **Clinical Validation** | Peer-reviewed studies or independent validation of accuracy |
| **Scale Reference** | Customer with 50+ facilities using the solution |
| **Multi-Region Deployment** | Evidence of operating in multiple regulatory jurisdictions |
| **Language Accuracy** | Demonstrated accuracy in each required language |
| **EHR Integration** | Live integrations with systems similar to Ramsay's (WebPAS, etc.) |
| **Uptime Track Record** | 12+ months of documented uptime metrics |
| **Security Audit** | Recent penetration test results; security incident history |

### 6.4 Local Support Requirements by Region

| Region | Support Requirement |
|--------|-------------------|
| **Australia** | Local implementation team; Sydney/Melbourne presence; AEST business hours support |
| **UK** | UK-based support; NHS experience; GMT business hours |
| **France** | French-speaking support; Paris presence or partner; HDS expertise |
| **Nordics** | Nordic language support capability; regional partner acceptable |
| **Global** | 24/7 critical incident support; escalation to engineering |

### 6.5 Procurement Process Recommendations

#### Phase 1: Market Scan & RFI (4-6 weeks)
- Issue RFI to shortlist of 5-8 vendors
- Focus on capability assessment against must-have requirements
- Evaluate regulatory pathway clarity

#### Phase 2: RFP & Evaluation (8-12 weeks)
- Detailed RFP to 3-4 shortlisted vendors
- Structured evaluation using weighted criteria
- Include clinical stakeholders, IT, compliance, procurement

#### Phase 3: Proof of Concept (8-12 weeks)
- Pilot in 2-3 sites per region
- Test against real workflows and EHR integrations
- Measure accuracy, user satisfaction, time savings

#### Phase 4: Commercial Negotiation (4-6 weeks)
- Negotiate enterprise agreement with regional flexibility
- Address data processing agreements for each jurisdiction
- Establish SLAs with financial penalties

#### Phase 5: Phased Rollout (12-18 months)
- Start with highest-readiness region
- Apply lessons learned to subsequent regions
- Build internal centers of excellence

### 6.6 Recommended Evaluation Team Composition

| Role | Responsibility |
|------|---------------|
| **Clinical Champion** (per region) | Clinical workflow validation; specialty requirements |
| **CIO/CTO Representative** | Technical architecture; integration approach |
| **Privacy/Compliance Officer** | Regulatory compliance; data protection |
| **Procurement Lead** | Commercial terms; vendor management |
| **Regional Operations** | Local requirements; change management |
| **Legal** | Contract review; liability; IP |

---

## 7. Risk Considerations

### 7.1 Regulatory Risk
- **Risk**: Vendor product not approved/registered in one or more jurisdictions
- **Mitigation**: Require regulatory roadmap; include registration milestones in contract; consider phased rollout by regulatory readiness

### 7.2 Data Sovereignty Risk
- **Risk**: Inadvertent cross-border data transfer; vendor acquisition by foreign entity
- **Mitigation**: Contractual protections; technical controls preventing data export; exit clauses triggered by ownership change

### 7.3 Vendor Concentration Risk
- **Risk**: Single global vendor creates dependency
- **Mitigation**: Evaluate regional best-of-breed approach; ensure data portability; maintain exit capability

### 7.4 Language/Accuracy Risk
- **Risk**: AI accuracy varies significantly by language or specialty
- **Mitigation**: Require performance guarantees by language; pilot in each language before full rollout

### 7.5 Integration Complexity Risk
- **Risk**: Diverse EHR landscape creates integration burden
- **Mitigation**: Prioritize FHIR-first approach; consider middleware layer; phase by system complexity

---

## 8. Appendix: Key Sources

### Regulatory Bodies
- [TGA AI and Medical Device Software](https://www.tga.gov.au/how-we-regulate/manufacturing/manufacture-medical-device/manufacture-specific-types-medical-devices/artificial-intelligence-ai-and-medical-device-software)
- [NHS DTAC Guidance](https://transform.england.nhs.uk/key-tools-and-info/digital-technology-assessment-criteria-dtac/how-to-use-the-dtac/)
- [EU AI Act (Nature Digital Medicine)](https://www.nature.com/articles/s41746-024-01232-3)
- [France HDS Certification](https://industriels.esante.gouv.fr/en/products-services/hds-health-data-hosting-certification)

### Data Protection
- [Australian Privacy Act (OAIC)](https://www.oaic.gov.au/privacy/privacy-legislation/the-privacy-act/health-and-and-medical-research)
- [UK GDPR (ICO)](https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/international-transfers/international-transfers-a-guide/)
- [EU GDPR Third Countries](https://gdpr-info.eu/issues/third-countries/)
- [European Commission Adequacy Decisions](https://commission.europa.eu/law/law-topic/data-protection/international-dimension-data-protection/adequacy-decisions_en)

### Ramsay Health Care
- [Ramsay Health Care Official](https://www.ramsayhealth.com/)
- [Ramsay Digital Transformation (CIO)](https://www.cio.com/article/4001875/perfecting-the-patient-customer-and-tech-health-plan-at-ramsey.html)
- [Ramsay Scribe (Healthcare IT News)](https://www.healthcareitnews.com/news/anz/advancing-clinical-note-taking-ramsay-health-care)
- [Ramsay Santé EU](https://www.ramsaysante.eu/)

### Clinical Systems
- [Dedalus WebPAS](https://www.dedalus.com/anz/our-offer/products/web-patient-administration-system-webpas/)
- [Healthcare FHIR Standards](https://www.hl7.org/fhir/overview.html)
- [Healthcare Interoperability Guide 2024](https://www.getfocal.co/post/healthcare-interoperability-standards-complete-guide-2024)

### AI & Speech Recognition
- [MultiMed Multilingual Medical ASR](https://arxiv.org/html/2409.14074v3)
- [Speechmatics Medical Model](https://www.speechmatics.com)

---

*Document Version: 1.0*
*Last Updated: November 2025*
