# Ramsay Health Care Technology Landscape Analysis

**Research Date:** November 2025
**Scope:** Global clinical systems, EHR infrastructure, and digital maturity by region

---

## Executive Summary

Ramsay Health Care operates 350+ facilities across 10 countries with a fragmented technology landscape reflecting regional acquisitions and local healthcare requirements. The organization has embarked on an ambitious 10-year digital transformation strategy (2030 Digital Strategy) with Google Cloud as its data and innovation partner. New technology leadership under Dr. John Doulis (former HCA Healthcare VP) signals intent to accelerate AI adoption and standardization.

**Key findings:**
- Australia: MEDITECH patient administration, building centralized data hub with BigQuery
- UK: IMS MAXIMS EPR deployed across all 35 hospitals (industry-leading standardization)
- France: Likely Softway Medical Hopital Manager (legacy Générale de Santé relationship)
- Nordics: Operating within established Nordic EHR ecosystems (Cambio COSMIC, TakeCare)
- Asia: InterSystems TrakCare (Indonesia) - operations divested in 2023

---

## 1. AUSTRALIA

### Scale
- **70+ hospitals, clinics, and surgical centers**
- Australia's largest private hospital operator
- Mix of acute care, day surgery, mental health, and rehabilitation

### EHR/Clinical Systems

| System | Vendor | Use Case |
|--------|--------|----------|
| MEDITECH | MEDITECH | Patient administration, billing, order communications |
| Ramsay Scribe | T-Pro / Internal | AI-powered clinical documentation (pilot) |
| Google Cloud BigQuery | Google | Centralized data hub |
| Various | Multiple | Site-specific clinical applications |

**Patient Administration:** MEDITECH is best known in Australia for providing patient administration and billing systems for Ramsay Health Care hospitals. The system provides order communications, electronic patient records, and clinical decision support.

**Clinical Documentation:** Ramsay developed **Ramsay Scribe** in partnership with T-Pro, piloting at St Andrew's Ipswich Private Hospital (January 2025). Uses AI-powered speech recognition and LLMs for clinical note-taking in emergency departments, with plans to expand to inpatient and mental health outpatient settings.

### Patient Administration Systems
- MEDITECH handles core patient administration, scheduling, and billing functions
- Medicare (MBS) and private insurance billing workflows integrated
- Cloud-based patient platform under development for pre-admission, digital consent, and payments

### Clinical Documentation Current State
- **Legacy:** Manual clinical note-taking, paper-based workflows still common
- **Transformation:** Ramsay Scribe pilot represents first AI documentation deployment
- **Timeline:** Prototyping mid-2024, pilot January 2025
- **Feedback:** "Overwhelmingly positive" from clinicians, significant time savings reported

### Digital Maturity Assessment

**Rating: Moderate (with accelerating trajectory)**

| Dimension | Status |
|-----------|--------|
| EHR Standardization | Partial - MEDITECH for admin, fragmented clinical |
| Data Integration | Building - BigQuery data hub in progress |
| AI Adoption | Early - Ramsay Scribe pilot |
| Patient Portal | Developing - Cloud platform under construction |
| Interoperability | Building - Apigee API Management deployed |

**Leadership Perspective:** Dr. Rachna Gandhi (former Group Chief Digital Officer) stated: "Healthcare is an industry with very low digital maturity... We have a late mover advantage. Benefits come from leapfrogging."

### Sources - Australia
- [Healthcare IT News - Advancing clinical note-taking at Ramsay](https://www.healthcareitnews.com/news/anz/advancing-clinical-note-taking-ramsay-health-care)
- [Ramsay Health Care - Digital Healthcare Transformation](https://www.ramsayhealth.com.au/News/General-News/Celebrating-significant-strides-in-digital-healthcare-transformation)
- [Hospital Health - Ramsay data hubs, AI and ML](https://www.hospitalhealth.com.au/content/technology/news/ramsay-to-set-up-central-data-hubs-use-ai-and-ml-for-transformation-301250413)
- [iTnews - Ramsay Health Care data hub](https://www.itnews.com.au/news/ramsay-health-care-to-stand-up-central-data-hub-ai-599041)
- [MEDITECH Global](https://ehr.meditech.com/global)

---

## 2. UK (RAMSAY UK)

### Scale
- **35 hospital sites**
- Private healthcare with significant NHS contract work
- Over 11,000 system users

### Systems in Use

| System | Vendor | Status |
|--------|--------|--------|
| IMS MAXIMS EPR | IMS MAXIMS | Live across all 35 sites (2022) |
| T-Pro | T-Pro | Speech recognition & documentation |
| Loop Workforce App | RLDatix | Workforce management |

**Electronic Patient Record:** Ramsay UK became the **first independent healthcare provider in the UK to implement a single EPR at this scale** when it deployed IMS MAXIMS across all 35 hospitals in February 2022. This represents the most standardized system within the Ramsay group globally.

**MAXIMS Capabilities:**
- Patient admissions and discharge
- Referral management and triage
- Scheduling and appointment correspondence
- Order communications
- Referral to treatment (RTT) pathways
- Real-time bed management
- Theatre management

**Clinical Documentation:** T-Pro speech recognition deployed in conjunction with MAXIMS EPR. Result: Average clinic letter turnaround dropped from **27 days to 6 days**.

### NHS Integration Requirements

Ramsay UK operates within the NHS framework through:
- **Integrated Care Board (ICB) contracts** - Each ICB determines budget allocation to private providers
- **NHS Choice Framework** - Patients can choose Ramsay for NHS-funded care
- **National tariff compliance** - Paid at same fixed rates as NHS trusts
- **NHS data standards** - Interoperability with NHS Spine, e-Referral Service

### Private Healthcare Tech Stack
- IMS MAXIMS as core EPR
- Integration with private medical insurers
- Patient portal and digital booking
- Component library/design system for web presence (Optimizely CMS)

### Digital Health Initiatives
- T-Pro for AI-assisted documentation
- RLDatix Loop for workforce management (rotas, leave, shift booking)
- Digital transformation strategy aligned with group 2030 vision
- Investment in website consolidation (36 sites → 1 dynamic platform)

### Digital Maturity Assessment

**Rating: High (most advanced in Ramsay group)**

| Dimension | Status |
|-----------|--------|
| EHR Standardization | Complete - Single EPR across all sites |
| Data Integration | Strong - Consistent outcome data for benchmarking |
| AI Adoption | Moderate - T-Pro deployed |
| Patient Portal | Established |
| NHS Interoperability | Compliant |

### Sources - UK
- [Digital Health Net - IMS MAXIMS EPR rolled out across Ramsay](https://www.digitalhealth.net/2022/02/ims-maxims-epr-rolled-out-ramsay/)
- [IMS MAXIMS - Ramsay Health Care UK now live](https://www.imsmaxims.com/news/ramsay-health-care-uk-maxims-epr-)
- [HTN - Ramsay Health Care goes live with MAXIMS EPR](https://htn.co.uk/2022/02/02/ramsay-health-care-goes-live-with-maxims-epr/)
- [Ramsay UK - MAXIMS EPR announcement](https://www.ramsayhealth.co.uk/about/news/ramsay-health-care-uk-now-live-with-maxims-electronic-patient-record-epr)
- [T-Pro Blog - Ramsay Health Care UK partnership](https://blog.tpro.io/ramsay-health-care-uk-partners-with-t-pro)

---

## 3. FRANCE (RAMSAY SANTÉ)

### Scale
- **Largest private hospital operator in France**
- Part of 350 facilities across 5 European countries
- 36,000 employees across Ramsay Santé Europe
- ~130 establishments in France

### French Healthcare IT Requirements

**Regulatory Framework:**
- **Dossier Médical Partagé (DMP)** - National shared medical record initiative
- **Ma Santé 2022** - Government digital health plan with substantial funding
- **Sécurité sociale** - Mandatory integration with French reimbursement systems
- **T2A (Tarification à l'activité)** - Activity-based tariff system
- **GDPR** - EU data protection compliance
- **HAS standards** - Haute Autorité de Santé secure communication requirements

### Systems in Use

| System | Vendor | Notes |
|--------|--------|-------|
| Hopital Manager (likely) | Softway Medical | Legacy relationship from Générale de Santé era |
| OpenXtrem modules | Softway Medical | Clinical modules |
| Various local systems | Multiple | French healthcare fragmentation |

**Historical Context:** When Softway Medical developed Hopital Manager, Générale de Santé (now Ramsay Santé) was among the early adopters who "believed in this project." OpenXtrem (acquired by Softway 2019) claims Ramsay Santé among its clients.

**Hopital Manager Features:**
- Comprehensive hospital information system (PGI/ERP)
- Certified as Hospital Prescription Aid Software (LAP)
- HAS-compliant secure communication
- Electronic patient file management
- "Best in KLAS" 2025 distinction (French market)

### Interoperability Status

**Current challenges in French market:**
- Data sources fragmented across non-interoperable systems
- Some vendors do not make systems fully open
- 80% of French healthcare decision-makers identify interoperability as most critical factor in future EHR selection

**Emerging standards:**
- HL7 FHIR and openEHR gaining traction
- DMP integration driving standardization
- Ma Santé 2022 funding accelerating upgrades

### AI Adoption

**French market context:**
- 83% of IT/clinical decision-makers interested in AI-powered EHR tools
- Only **4%** have commenced AI pilots or production deployments
- Key barriers: Data privacy concerns (91%), integration complexity (88%), cost (70%)

**Ramsay Santé position:**
- Innovation Hub established
- "Digi-physical pathways" vision for patient journey
- Limited public information on specific AI deployments

### Digital Maturity Assessment

**Rating: Moderate-Low (regulatory complexity, fragmentation)**

| Dimension | Status |
|-----------|--------|
| EHR Standardization | Low - Fragmented legacy systems |
| Data Integration | Developing - DMP compliance ongoing |
| AI Adoption | Very Early - 4% market adoption rate |
| Patient Portal | Developing |
| Interoperability | Improving - FHIR/openEHR emerging |

### Sources - France
- [Ramsay Santé - Innovation](https://www.ramsaysante.eu/group-group-innovation-partnership-hub/innovation-ramsay-sante)
- [Infermedica - Ramsay Santé personalized patient connection](https://infermedica.com/blog/articles/ramsay-sante-a-hospital-offering-patients-a-personalized-connection-to-medical-services)
- [Softway Medical - Hopital Manager](https://www.softwaymedical.fr/produit/hopital-manager)
- [Access Newswire - France's EHR Revolution 2025](https://www.accessnewswire.com/newsroom/en/healthcare-and-pharmaceutical/frances-ehr-revolution-ai-compliance-and-interoperability-drive-2025-1006944)
- [PMC - French Health Data Hub](https://pmc.ncbi.nlm.nih.gov/articles/PMC6697511/)

---

## 4. NORDICS (SWEDEN, NORWAY, DENMARK)

### Scale (via Capio acquisition 2018)
- **140+ facilities** across Sweden, Norway, Denmark
- 100+ primary care centers (Sweden)
- ~30 specialist clinics
- 13 orthopedic/specialized centers
- 1 major hospital (St. Göran, Stockholm)
- ~900,000 registered patients in Sweden (10% of population)

### Nordic Healthcare Digitization Context

**The Nordics represent the most digitally advanced healthcare market globally:**
- 99% e-prescription rates in Sweden
- ~$1.22 billion annual regional IT investment (Sweden)
- National patient portals in all countries
- Personal identity numbers enabling cross-system integration
- Strong government-led digital health strategies

### Systems in Use by Country

#### SWEDEN
| System | Vendor | Coverage |
|--------|--------|----------|
| Cambio COSMIC | Cambio | Most widely used EHR in Sweden |
| TakeCare | CompuGroup Medical | Stockholm region, Karolinska |
| Webdoc | Various | Primary care |
| Various | Multiple | Site-specific |

**Capio/Ramsay likely operates within existing regional EHR ecosystems** rather than deploying proprietary systems, as Swedish healthcare IT is highly standardized at regional level.

**St. Göran Hospital:** Sweden's largest private hospital, elected "Best Hospital in Sweden" (small hospital category) in 2017 and 2019. Highly integrated with Stockholm County systems.

#### NORWAY
| System | Vendor | Market Share |
|--------|--------|--------------|
| DIPS | DIPS AS | 80% of Norwegian hospital market |
| Helseplattformen (Epic) | Epic | Central Norway (troubled rollout) |

**Capio Norway:** 10 community health centers + 7 specialized centers. Likely operates on DIPS given 80% market dominance. Helseplattformen (Epic) implementation in Central Norway has faced significant challenges (usability score 17.3 vs. DIPS 57.7).

#### DENMARK
| System | Vendor | Notes |
|--------|--------|-------|
| Epic | Epic | Major hospital systems |
| Various | Multiple | Private sector |
| Patient Portal | Capio | capio.patientportal.dk |

**Capio Denmark:** 5 specialized clinics across 4 of 5 Danish health regions. Largest private hospital chain in Denmark. Digital Transformation Office established in Copenhagen.

### National Health Record Integration
- **Sweden:** Full integration with national e-prescription system, 1177 patient portal
- **Norway:** NPR (Norwegian Patient Register) reporting, Helseplattformen expansion ongoing
- **Denmark:** Sundhed.dk national health portal integration

### AI Readiness

**Rating: High (infrastructure-ready, cautious adoption)**

Nordic markets have:
- Strong data infrastructure for AI
- Established interoperability standards
- Privacy-conscious regulatory environment
- Capio "voice-to-invoice" project using voice-to-text in medical records
- Innovation Hub partnership model

### Digital Maturity Assessment

**Rating: High (benefiting from Nordic digital health leadership)**

| Dimension | Status |
|-----------|--------|
| EHR Standardization | High - Regional/national systems |
| Data Integration | Strong - National registries, portals |
| AI Adoption | Moderate - Infrastructure ready |
| Patient Portal | Established - National + Capio portals |
| Interoperability | Strong - Nordic standardization |

### Sources - Nordics
- [Ramsay Santé - Sweden](https://www.ramsaysante.eu/countries/ramsay-sante-sweden)
- [Ramsay Santé - Denmark](https://www.ramsaysante.eu/countries/ramsay-sante-denmark)
- [Nordic Council - eHealth standardisation](https://norden.diva-portal.org/smash/get/diva2:1340369/FULLTEXT01.pdf)
- [JMIR - Nordic Patient Online Record Access](https://www.jmir.org/2024/1/e49084)
- [Cambio Group - COSMIC](https://www.cambiogroup.com/our-solutions/cambio-cosmic/)
- [Tidsskriftet - Norwegian EHR usability](https://tidsskriftet.no/en/2025/10/perspectives/poor-usability-electronic-health-records-norway)

---

## 5. ASIA (MALAYSIA, INDONESIA, HONG KONG)

**Note: Ramsay divested Asian operations in 2023** - sold to Hong Leong Group/TPG for 5.7 billion ringgit.

### Historical Operations (Pre-Divestiture)

**Ramsay Sime Darby Health Care (RSDH):**
- Joint venture between Ramsay Health Care and Sime Darby
- 6 hospitals across Malaysia and Indonesia
- 1 ambulatory center in Hong Kong

#### MALAYSIA
| Facility | Location |
|----------|----------|
| Subang Jaya Medical Centre | Selangor |
| Ara Damansara Medical Centre | Selangor |
| ParkCity Medical Centre | Kuala Lumpur |

#### INDONESIA
| Facility | EHR System |
|----------|------------|
| RS Premier Jatinegara | InterSystems TrakCare |
| RS Premier Bintaro | InterSystems TrakCare |
| RS Premier Surabaya | InterSystems TrakCare |

**Technology Partnership:** RSDHI pioneered InterSystems TrakCare EMR deployment in Indonesia in a 20-year partnership. Among first in Southeast Asia to implement electronic ordering, result reporting, and clinical functions.

### Systems by Country (Historical)

| Country | Primary System | Vendor |
|---------|---------------|--------|
| Indonesia | TrakCare (Cloud EMR) | InterSystems |
| Malaysia | Unknown | Unknown |
| Hong Kong | Unknown | Unknown |

**Indonesian capabilities included:**
- Electronic ordering and result reporting
- Cloud-based EMR deployment
- Clinical and operational analytics
- Third-party booking integration
- Self-service kiosks
- Smart-ward technology

### Digital Maturity (Historical)

**Rating: Moderate (Indonesia highest)**

Indonesia operations were notably advanced:
- "Pioneered world-class healthcare information systems in Indonesia"
- Cloud EMR deployment
- Digital services integration

### Local Requirements
- **Malaysia:** PDPA (Personal Data Protection Act), MyKAD integration
- **Indonesia:** BPJS (national insurance) integration, Ministry of Health standards
- **Hong Kong:** HKHA (Hospital Authority) interoperability for public referrals

### Current Relevance

Post-divestiture, these operations are **no longer part of Ramsay Health Care**. The new ownership (Hong Leong/TPG) continues operating as Asia OneHealthcare.

### Sources - Asia
- [InterSystems - RSDHI Cloud EMR deployment](https://www.intersystems.com/sg/news/products/trakcare/ramsay-sime-darby-health-care-indonesia-and-intersystems-deploy-cloud-emr-system/)
- [Ramsay Sime Darby Health Care - Corporate](https://www.ramsaysimedarby.com/corporate)
- [Asia OneHealthcare - Columbia Asia transition](https://asiaonehealth.com/columbia-asia-healthcare-is-now-asia-onehealthcare/)
- [Wikipedia - Ramsay Health Care](https://en.wikipedia.org/wiki/Ramsay_Health_Care)

---

## 6. INTEGRATION CHALLENGES

### Cross-Region Data Sharing

**Current State: Highly Fragmented**

| Challenge | Description |
|-----------|-------------|
| Multiple EHR vendors | MEDITECH, IMS MAXIMS, Softway, Cambio, etc. |
| Regional autonomy | Each region manages own IT infrastructure |
| Regulatory differences | TGA (AU), MHRA (UK), MDR (EU), country-specific |
| Data residency | Local storage requirements vary by jurisdiction |
| Language | English (AU/UK), French, Swedish, Norwegian, Danish |

**No unified patient record exists across Ramsay's global operations.**

### Standardization Efforts

#### Google Cloud Partnership (2023)
Key initiatives to drive standardization:
1. **BigQuery Data Hub** - Centralized data warehouse (initially Australia)
2. **Apigee API Management** - Healthcare data protocol support
3. **Anthos Service Mesh** - Secure inter-facility data access
4. **Common data model** - Single source of truth with standardized definitions
5. **Data governance framework** - Quality and security standards

#### Regional Standardization
- **UK:** Complete - single IMS MAXIMS EPR across all 35 sites
- **Australia:** Building - data hub initiative, fragmented clinical systems
- **Nordics:** Leveraging regional/national standards
- **France:** Low - legacy fragmentation

### FHIR Adoption Status

**Assessment: Early Stage**

| Region | FHIR Status |
|--------|-------------|
| Australia | Building via Apigee; not explicitly FHIR-first |
| UK | IMS MAXIMS supports FHIR; NHS increasingly mandating |
| France | Emerging - HL7 FHIR and openEHR gaining traction |
| Nordics | Advanced - Swedish regions implementing FHIR |

**Google Cloud Capability:** Cloud Healthcare API supports FHIR data ingestion to BigQuery, but Ramsay announcements do not explicitly confirm FHIR-first strategy.

### Barriers to Unified Platform

| Barrier | Severity | Mitigation |
|---------|----------|------------|
| EHR diversity | High | Data hub abstraction layer |
| Regulatory fragmentation | High | Regional compliance teams |
| Language requirements | Medium | Multi-language support needed |
| Clinical workflow variation | Medium | Standardized APIs |
| Cost of replacement | High | Incremental modernization |
| Clinician change management | Medium | Phased rollouts |
| Local vendor relationships | Medium | Integration partnerships |

### Strategic Implications

**For AI Vendor Evaluation:**
1. Any vendor must support multiple EHR integrations (not Epic/Cerner-centric)
2. FHIR-first approach essential for future state
3. UK offers most standardized deployment environment
4. Australia data hub creates central integration point
5. France and Nordics require local system expertise

---

## 7. LEADERSHIP & DIGITAL STRATEGY

### New Technology Leadership (November 2025)

**Dr. John Doulis** - Group Executive, Technology and Digital
- **Previous:** VP and Distinguished Architect, HCA Healthcare Digital Transformation & Innovation
- **HCA Accomplishments:**
  - Rostering/scheduling platform for 100,000 nurses
  - Digital handover systems
  - Ambient speech recognition tools
  - AI-driven clinical guidance
- **Education:** MD from Monash University (Australia)
- **Experience:** 20+ years senior leadership in US and Australia

**Replaces:** Dr. Rachna Gandhi (Group Chief Digital and Data Officer, departed September 2025 after 4 years)

### 2030 Digital Strategy

**Vision:** "Seamless, patient-centred, digitally enabled care that supports better outcomes for patients, doctors and teams"

**Key pillars:**
1. Centralized data hub (BigQuery)
2. AI-powered clinical tools (Ramsay Scribe)
3. Single patient platform entry point
4. Predictive analytics for risk assessment
5. Operational optimization (demand forecasting, coding)

**Partner:** Google Cloud (data and innovation partner)

### Sources - Leadership
- [Healthcare IT News - Ramsay new tech exec](https://www.healthcareitnews.com/news/anz/ramsay-health-care-reveals-new-tech-exec)
- [iTnews - Ramsay under new tech leadership](https://www.itnews.com.au/news/ramsay-health-care-under-new-tech-leadership-from-november-620414)
- [CIO - Rachna Gandhi interview](https://www.cio.com/article/4001875/perfecting-the-patient-customer-and-tech-health-plan-at-ramsey.html)
- [Ramsay - Google Cloud partnership](https://www.ramsayhealth.com.au/News/General-News/Ramsay-Health-Care-Joins-Forces-with-Google-Cloud-to-Help-Support-Its-2030-Digital-Strategy)

---

## Summary Matrix

| Region | Primary EHR | Standardization | Digital Maturity | AI Readiness |
|--------|-------------|-----------------|------------------|--------------|
| **Australia** | MEDITECH (admin) | Low | Moderate | Building |
| **UK** | IMS MAXIMS | High (complete) | High | Moderate |
| **France** | Hopital Manager (likely) | Low | Moderate-Low | Very Early |
| **Sweden** | Regional (COSMIC/TakeCare) | High (national) | High | High |
| **Norway** | DIPS (likely) | High (national) | High | Moderate |
| **Denmark** | Various | Moderate | High | Moderate |
| **Asia** | Divested 2023 | N/A | N/A | N/A |

---

## Implications for AI Vendor Selection

1. **UK is the proving ground** - Most standardized, single EPR, fastest path to scale
2. **Australia is strategic priority** - HQ market, data hub investment, leadership attention
3. **Nordics offer infrastructure** - Digital maturity enables rapid deployment
4. **France requires patience** - Regulatory complexity, low AI adoption market-wide
5. **Multi-EHR integration is mandatory** - Cannot assume single vendor environment
6. **T-Pro relationship established** - Existing partnership for Ramsay Scribe
7. **Google Cloud ecosystem preferred** - BigQuery, Vertex AI, Cloud Healthcare API alignment

---

*Research compiled: November 2025*
*Classification: Commercial Intelligence*
