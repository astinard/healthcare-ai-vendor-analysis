# Australian EHR & Clinical Software Landscape Analysis

**Last Updated:** November 2025
**Purpose:** Market analysis for Ramsay Health Care AI vendor evaluation context

---

## Executive Summary

Australia's digital health market is maturing rapidly, with distinct systems serving GP/primary care versus hospital settings. The market is characterized by:
- **GP Sector:** Dominated by two players (Best Practice, MedicalDirector) with ~23,000+ GPs using these systems
- **Hospital Sector:** Mix of international vendors (Epic, Oracle Health) and strong local/regional players (Dedalus webPAS, InterSystems TrakCare)
- **Interoperability:** Transitioning from HL7 CDA to FHIR, with $45-50M invested in modernization
- **AI Integration:** Emerging but accelerating, with ambient documentation tools leading adoption

---

## 1. GP/Primary Care Software

### Best Practice Software (Bp Premier)

**Market Position:** Australia's leading GP practice management software

**Key Features:**
- Integrated clinical, billing, and practice management
- Medicare/DVA online claiming with instant electronic claims
- HICAPS integration for private health insurance claims
- SafeScript integration (real-time prescription monitoring)
- 200+ third-party integrations
- Automatic MBS, DVA, PBS, MIMS updates

**Technical Details:**
- Desktop-based with server architecture
- 50+ support specialists across Australia/NZ
- Free phone/email support included in licensing

**Sources:**
- [Best Practice Software](https://bpsoftware.net/)
- [BP Premier Features](https://bestpracticesoftware.com/products/bp-premier/)

---

### MedicalDirector (Helix)

**Market Position:** Claims ~23,000 GPs and specialists, 80+ million patient consultations annually

**Products:**
- **MedicalDirector Clinical** (legacy desktop)
- **Helix** (cloud-based, launched as Australia's first cloud clinical management software)

**Helix Key Features:**
- Cloud-native on Microsoft Azure (Australian data centers)
- Integrated telehealth
- ePrescribing with Real-Time Prescription Monitoring
- Australian Immunisation Register integration
- AusDI drug database integration
- Fortnightly automatic updates
- Full clinical history view in single screen

**Ownership:** Now part of Telstra Health

**Sources:**
- [MedicalDirector Helix](https://www.medicaldirector.com/products/helix)
- [Telstra Health Helix](https://www.telstrahealth.com/products/helix/)

---

### Genie Solutions (Magentus)

**Market Position:** Australia's leading specialist practice management software, 5,000+ practices, 27+ years in market

**Products:**
- **Genie** (desktop) - Most popular for complex specialist workflows
- **Gentu** (cloud) - Modern cloud alternative

**Key Features:**
- 50+ specialty-specific modules (orthopaedics, rheumatology, obstetrics, ophthalmology, dermatology, etc.)
- Up to 100 concurrent users per database
- Custom clinical workflows by specialty
- Built-in telehealth
- AI integration (Heidi ambient documentation)
- Australian data center storage

**Target Market:** Specialists and complex practices (vs. GP focus of Best Practice/MedicalDirector)

**Ownership:** Now branded as Magentus

**Sources:**
- [Genie Solutions](https://www.geniesolutionssoftware.com.au/)
- [Genie Practice Management](https://www.geniesolutionssoftware.com.au/products/genie)

---

### Cliniko

**Market Position:** 65,000+ health professionals globally, Australian-founded and headquartered

**Target Market:** Allied health practices (physiotherapy, psychology, chiropractic, etc.)

**Key Features:**
- Cloud-native SaaS
- Appointment scheduling with online booking
- Customizable treatment note templates
- Integrated telehealth (video/audio)
- SMS appointment reminders
- Xero accounting integration
- Real-time alerts for arrivals/cancellations

**Pricing:**
- Starts at USD $45/month
- Per-practitioner pricing model
- All features included at all tiers
- Free for registered charities/educational institutions
- No price increases since 2011

**Sources:**
- [Cliniko](https://www.cliniko.com/)
- [Cliniko Pricing](https://www.cliniko.com/pricing/)

---

### Other GP/Allied Health Systems

| System | Focus | Notes |
|--------|-------|-------|
| **Power Diary** | Allied health | Popular for multi-practitioner clinics |
| **Nookal** | Allied health | Strong in physiotherapy |
| **ZedMed** | GPs | Smaller market share |
| **Mediportal** | Allied health | Cloud-based |
| **Halaxy** | Allied health | Free tier available |

---

## 2. Hospital Systems

### Epic Systems

**Australian Presence:**

| State | Implementation | Status |
|-------|---------------|--------|
| **Victoria** | Parkville precinct (Royal Melbourne, Royal Children's, Royal Women's) | Live since 2020, $124M investment |
| **ACT** | Canberra Health Services | 10-year, $151M contract, deployment ongoing |
| **NSW** | Statewide Digital Patient Record (SDPR) | Contract signed 2023, Hunter New England lead site 2025-26 |

**Notable:**
- Royal Children's Hospital Melbourne was first Australian paediatric Epic go-live (2016)
- NSW SDPR is Australia's largest Epic deployment covering 220+ public hospitals
- Epic ranked 7th in Black Book's 2025 Australia EHR rankings

**Sources:**
- [Epic Australia Launches](https://www.epic.com/epic/post/three-hospitals-in-australia-launch-epic-in-the-midst-of-the-pandemic/)
- [NSW Health Epic Contract](https://www.darkdaily.com/2023/02/15/australias-nsw-health-chooses-epic-for-its-statewide-patient-ehr/)
- [ACT Epic Deal](https://www.itnews.com.au/news/epic-wins-114m-act-digital-health-records-platform-deal-551004)

---

### Oracle Health (formerly Cerner)

**Market Position:**
- Ranked #1 in Black Book Research's 2025 Australian Healthcare IT Rankings
- Strong in health data analytics via Health Data Intelligence Platform
- Global: ~22% US acute care market share

**Australian Presence:**
- Present but less visible than Epic in recent major contracts
- Health Data Intelligence Platform being sold for national-level data views

**AI Capabilities (2024):**
- AI-powered clinical agent for conversational note generation
- Oracle Clinical Digital Assistant
- Reported 4.5 minutes saved per patient, 20-40% documentation time reduction

**Sources:**
- [Black Book 2025 Rankings](https://www.newswire.com/news/australia-s-digital-health-transformation-black-book-research-reveals-22494342)
- [Oracle Health AI Features](https://www.oracle.com/news/announcement/oracle-delivers-new-electronic-health-record-innovations-2024-09-18/)

---

### InterSystems TrakCare

**Market Position:** Top EHR vendor in Asia/Oceania region (KLAS), 132 customers in region

**Australian Deployments:**

| Site | Type | Notes |
|------|------|-------|
| **Bendigo Health (VIC)** | Regional hospital | Largest regional hospital development in Victoria |
| **Macquarie University Hospital** | Private teaching hospital | Fully integrated digital hospital |
| **Northern Territory Government** | Territory-wide | Unified health information across NT |
| **South Australia** | Shared EPR | State-level deployment |
| **Western Australia** | Shared EPR | State-level deployment |
| **Victoria Community Health** | 22 agencies | Community health configuration |

**Sources:**
- [InterSystems TrakCare](https://www.intersystems.com/au/products/trakcare/)
- [Bendigo Health Implementation](https://www.healthcareitnews.com/news/australian-health-system-bendigo-health-taps-intersystems-electronic-health-record)

---

### Dedalus (webPAS + iSOFT legacy)

**Background:**
- Acquired DXC Technology's healthcare business (2020) for US$525M
- DXC previously acquired iSOFT (2011) for US$188M
- iSOFT was originally an Australian ASX-listed company

**webPAS (Patient Administration System):**
- Installed in 250+ sites across ANZ
- Manages 22,000+ hospital beds
- Used in majority of Australian/New Zealand public hospitals
- Supports both public and private hospital deployments

**Product Suite:**
- Patient Administration System (webPAS)
- Electronic Medication Management
- Clinical Documentation
- Pharmacy Systems

**Sources:**
- [Dedalus webPAS](https://www.dedalus.com/anz/our-offer/products/web-patient-administration-system-webpas/)
- [DXC Healthcare Sale](https://www.pulseit.news/australian-digital-health/dxc-sells-healthcare-software-business-to-european-clinical-it-firm-dedalus/)

---

### Other Hospital Systems

| Vendor | Product | Australian Presence |
|--------|---------|-------------------|
| **MEDITECH** | Expanse | Ranked #2 in Black Book 2025; Ramsay Health Care partnership |
| **Altera Digital Health** | Various | Ranked #3 in Black Book 2025 |
| **Telstra Health** | Kyra Clinical | Ranked #5 in Black Book 2025 |
| **Philips** | TASY | Ranked #8 in Black Book 2025 |
| **Orion Health** | Various | Ranked #10 in Black Book 2025 |

---

### State Health Department Systems

| State | Primary Systems | Notes |
|-------|-----------------|-------|
| **NSW** | Epic (SDPR rollout) | 220+ public hospitals, largest state system |
| **Victoria** | Mix: Epic (Parkville), TrakCare (regional), webPAS | Fragmented, multiple vendors |
| **Queensland** | Various including webPAS | Queensland Health manages |
| **South Australia** | InterSystems TrakCare | Shared EPR model |
| **Western Australia** | InterSystems TrakCare, webPAS | HSS manages IT services |
| **ACT** | Epic | Territory-wide deployment |
| **Northern Territory** | InterSystems TrakCare | Territory-wide unified system |
| **Tasmania** | Various | Smaller scale |

---

## 3. Interoperability

### My Health Record

**Status (November 2024):**
- 24.1+ million registered users (near-universal coverage)
- 1.8+ billion clinical documents uploaded
- Connected to hospitals, pathology labs, specialists, GPs

**Technical Architecture:**
- Currently based on Clinical Document Architecture (CDA)
- Transitioning to FHIR for better real-time interoperability

**Sources:**
- [My Health Record FHIR IG](https://developer.digitalhealth.gov.au/fhir/my-health-record/current/index.html)

---

### FHIR Adoption

**Current Status:**
- Australian Digital Health Agency (ADHA) leading modernization
- $45-50M contract issued for FHIR interoperability support
- 1,000+ participants trained in FHIR courses (partnership with HL7 Australia)
- Target: Fully connected health system by 2027

**Key Resources:**
- [ADHA FHIR Implementation Guide](https://build.fhir.org/ig/AuDigitalHealth/ci-fhir-r4/)
- [My Health Record FHIR IG v1.3.0](https://developer.digitalhealth.gov.au/fhir/my-health-record/current/index.html)
- [Digital Health Developer Portal](https://developer.digitalhealth.gov.au/fhir-resources)

**National Healthcare Interoperability Plan:**
- Vision: Fully connected Australian health system by 2027
- Strategy period: 2023-2028

**Sources:**
- [FHIR Modernization](https://www.digitalhealth.gov.au/newsroom/media/another-leap-forward-in-modernising-my-health-record-with-fhir)
- [FHIR Investment](https://www.healthcareitnews.com/news/anz/30m-my-health-record-interoperability-and-more-briefs)

---

### HL7 Usage

**Current State:**
- HL7 v2 widely used for messaging (ADT, lab results, etc.)
- HL7 CDA used for My Health Record documents
- HL7 FHIR R4 being adopted for modern APIs

**HL7 Australia:**
- Active chapter partnering with ADHA
- Developing Australian FHIR profiles and implementation guides

**Sources:**
- [HL7 Standards Portal](https://developer.digitalhealth.gov.au/standards/organisation/health-level-seven-hl7)

---

### Data Exchange Standards Summary

| Standard | Usage | Status |
|----------|-------|--------|
| **HL7 v2** | Hospital messaging | Legacy, still widely used |
| **HL7 CDA** | My Health Record documents | Current, being phased for FHIR |
| **HL7 FHIR R4** | Modern APIs | Growing adoption, government push |
| **SNOMED CT-AU** | Clinical terminology | Australian extension |
| **AMT** | Medication terminology | Australian Medicines Terminology |

---

## 4. AI Integration

### EHR Vendor AI Capabilities

| Vendor | AI Features | Status |
|--------|-------------|--------|
| **Oracle Health** | Clinical Digital Assistant, AI note generation | Available 2024 |
| **Epic** | Ambient documentation, clinical decision support | Available |
| **MEDITECH** | BotMD integration, decision support | Available |
| **Best Practice** | Partner integrations (MBSPro AI billing) | Third-party |
| **MedicalDirector** | Limited native AI | Emerging |
| **Genie Solutions** | Heidi ambient AI integration | Third-party |

---

### Third-Party AI Integration Approaches

**Ambient Documentation (Leading Category):**
- **Heidi Health** - Australian, integrates with Genie, Best Practice
- **T-Pro** - Powers Ramsay Scribe
- **Nuance DAX** - Microsoft-owned, limited Australian presence
- **Nabla** - European, expanding

**Clinical Decision Support:**
- **ANU AI systems** - Rare disease diagnosis assistance
- Various vendor-specific CDS modules

**Billing/Coding AI:**
- **MBSPro** - Medicare billing optimization for Best Practice
- AI-powered clinical coding solutions emerging

---

### API Availability

| System | API Type | Documentation |
|--------|----------|---------------|
| **My Health Record** | FHIR R4 REST | [Developer Portal](https://developer.digitalhealth.gov.au/) |
| **Best Practice** | Partner API program | Limited, requires partnership |
| **MedicalDirector** | Integration APIs | Selective availability |
| **Epic** | FHIR APIs, App Orchard | Comprehensive |
| **Oracle Health** | FHIR APIs | Available |
| **Genie** | Partner integrations | Case-by-case |

---

### Integration Challenges

1. **Data Standards Fragmentation**
   - Mix of HL7 v2, CDA, and emerging FHIR
   - Inconsistent terminology adoption

2. **Privacy/Security Requirements**
   - Australian Privacy Principles compliance
   - State-specific health records legislation
   - Data sovereignty requirements (Australian data centers)

3. **Vendor Lock-in**
   - Proprietary APIs and data formats
   - Limited export capabilities in some systems

4. **Workflow Integration**
   - Clinician resistance to new tools
   - EHR usability concerns (burnout)
   - Need for seamless embedding, not separate apps

5. **Regulatory Uncertainty**
   - TGA software as medical device requirements evolving
   - AI-specific regulations developing

---

## 5. Ramsay Health Care Systems

### Overview

**Scale:**
- 70+ hospitals, clinics, and surgical centres across Australia
- Part of global network (Europe, UK)
- ASX-listed (ASX: RHC)

---

### Current Clinical Systems

**EHR Partnership:**
- **MEDITECH** - Listed as key partner in Asia Pacific region
- Part of MEDITECH's notable Australian/NZ customer base

**Patient Administration:**
- Likely webPAS or similar for patient administration functions
- Specific PAS not publicly confirmed

---

### Digital Transformation Strategy

**2030 Digital Strategy (10-year plan):**

1. **Google Cloud Partnership** (2023)
   - Data and innovation partner
   - Central data hub on BigQuery
   - AI/ML capabilities platform

2. **Ramsay Data Hub**
   - Consolidated from 70+ on-premise data silos
   - Built with Kasna (Mantel Group)
   - Single source of truth for analytics

3. **Digital Front Door**
   - Single entry point for patients, clinicians, staff
   - Unified digital ecosystem

4. **EHR Investment**
   - Focus on deeper VMO (Visiting Medical Officer) integration
   - VMO involvement in EHR design

---

### AI Initiatives

**Ramsay Scribe:**
- AI-powered clinical documentation tool
- Developed with T-Pro (AI clinical documentation specialist)
- Pilot: St Andrew's Ipswich Private Hospital ED (Queensland)
- Planned expansion: Inpatient and mental health outpatient settings

**Other AI Applications (with Google Cloud):**
- Clinical notes analysis for pattern identification
- AI-optimized clinical coding
- Demand forecasting (medications, theatre utilization, staffing)

**Leadership:**
- Dr. Rachna Gandhi - Global Chief Digital and Data Officer
- Team won CIO 50 Team of the Year for customer value

---

### Standardization Status

**Current State:**
- Historically decentralized (70+ sites with separate data)
- Active consolidation via Ramsay Data Hub
- EHR standardization across network in progress

**Challenges:**
- Legacy system diversity across acquired facilities
- VMO (visiting doctor) workflow variation
- Integration with external health systems

---

### Sources

- [Ramsay Google Cloud Partnership](https://www.ramsayhealth.com.au/News/General-News/Ramsay-Health-Care-Joins-Forces-with-Google-Cloud-to-Help-Support-Its-2030-Digital-Strategy)
- [Ramsay Scribe AI](https://www.itnews.com.au/news/ramsay-health-care-pilots-ai-powered-clinical-documentation-tool-615061)
- [Ramsay Digital Transformation](https://www.hospitalhealth.com.au/content/technology/news/ramsay-to-set-up-central-data-hubs-use-ai-and-ml-for-transformation-301250413)
- [MEDITECH Asia Pacific](https://ehr.meditech.com/global/meditech-asia-pacific)

---

## Implications for AI Vendor Selection

### Integration Considerations

1. **FHIR-First Approach**
   - Australian healthcare moving toward FHIR
   - Vendors with strong FHIR support have advantage
   - My Health Record FHIR gateway is key integration point

2. **Australian Data Residency**
   - Requirement for Australian data centers
   - Compliance with Australian Privacy Principles
   - State-specific health records legislation

3. **Ramsay-Specific Integration**
   - Must integrate with MEDITECH (or current EHR)
   - Google Cloud/BigQuery compatibility advantageous
   - T-Pro relationship establishes precedent for AI documentation

4. **GP Ecosystem Connection**
   - Patients flow from GP to Ramsay facilities
   - Best Practice/MedicalDirector integration valuable
   - Referral and discharge summary workflows

### Recommended Vendor Evaluation Criteria

| Criterion | Weight | Rationale |
|-----------|--------|-----------|
| FHIR API capability | High | Australian standards direction |
| Australian data residency | High | Regulatory requirement |
| MEDITECH integration | High | Ramsay's current EHR |
| Ambient documentation | Medium | Ramsay Scribe precedent |
| Google Cloud compatibility | Medium | Ramsay's platform |
| My Health Record integration | Medium | National infrastructure |

---

## Key Sources Summary

### Government/Official
- [Australian Digital Health Agency](https://www.digitalhealth.gov.au/)
- [My Health Record Developer Portal](https://developer.digitalhealth.gov.au/)
- [HL7 Australia](https://www.hl7.org.au/)

### Industry Research
- [Black Book Research 2025 Rankings](https://www.newswire.com/news/australia-s-digital-health-transformation-black-book-research-reveals-22494342)
- [Pulse+IT](https://www.pulseit.news/) (Australian digital health news)
- [Healthcare IT News ANZ](https://www.healthcareitnews.com/anz)

### Vendor Sources
- [Best Practice Software](https://bpsoftware.net/)
- [MedicalDirector](https://www.medicaldirector.com/)
- [Genie Solutions / Magentus](https://www.geniesolutionssoftware.com.au/)
- [Cliniko](https://www.cliniko.com/)
- [Epic Systems](https://www.epic.com/)
- [Oracle Health](https://www.oracle.com/health/)
- [InterSystems TrakCare](https://www.intersystems.com/au/products/trakcare/)
- [Dedalus ANZ](https://www.dedalus.com/anz/)
- [MEDITECH](https://ehr.meditech.com/)
