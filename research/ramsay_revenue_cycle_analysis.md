# Ramsay Health Care: Revenue Cycle & Coding Analysis by Region

**Date**: November 2025
**Scope**: Australia, UK, France, Nordics
**Focus**: Billing systems, coding standards, AI opportunities

---

## Executive Summary

Ramsay Health Care operates across four distinct regulatory and reimbursement environments, each with unique coding systems, payer structures, and revenue cycle challenges. This analysis examines the billing infrastructure in each region and identifies AI opportunities for auto-coding, clinical documentation improvement (CDI), denial management, and revenue leakage prevention.

| Region | Revenue Mix | Coding System | DRG System | Primary Payer |
|--------|-------------|---------------|------------|---------------|
| Australia | ~50% of global | ICD-10-AM / ACHI | AR-DRG | PHI (45%) + Medicare (36%) |
| France | ~35% of EU ops | CIM-10 / CCAM | GHM/GHS (T2A) | Sécurité sociale + Mutuelle |
| UK | NHS + Private | ICD-10 / OPCS-4 | HRG4+ | NHS tariff + Private pay |
| Nordics | Capio network | ICD-10-SE / NordDRG | NordDRG | Regional government |

---

## 1. Australia Billing & Revenue Cycle

### 1.1 Market Position
- **70+ private hospitals** and day surgery units
- **4 public facilities** under contract (Joondalup, Mildura, Noosa, Peel)
- **~50% of Ramsay global revenue** (~A$8.3B of A$16.66B FY2024)
- FY2025 H1: 5% revenue increase, 3% rise in hospital admissions

### 1.2 Revenue Sources

| Payer | % of Private Hospital Funding | Billing Mechanism |
|-------|------------------------------|-------------------|
| Private Health Insurance (PHI) | 45% | Negotiated contracts with funds |
| Federal Government (Medicare) | 36% | MBS fee schedule (85% of MBS rate for inpatient) |
| Individual Out-of-Pocket | 11% | Gap payments, self-funded |
| Non-Government Sources | 6.9% | Workers comp, third-party |
| State/Territory | 1.2% | Public contract payments |

**Source**: [Ramsay Healthcare Australia Overview](https://www.ramsayhealth.com/en/investors/our-markets/australia-healthcare-overview/)

### 1.3 Medicare Billing (MBS)

**Medicare Benefits Schedule (MBS)** governs physician reimbursement:

- **Bulk-billing**: Medicare covers 100% of GP visits at published MBS rate
- **Inpatient specialist services**: 85% of MBS rate covered by Medicare
- **Gap payment**: Remaining 15% + hospital costs covered by PHI or patient
- **Hospital accommodation/theatre/nursing**: Not covered by Medicare - PHI or self-pay

**Key constraint**: Visiting Medical Officers (VMOs) are paid separately from hospital revenue - they bill Medicare and PHI directly.

**Source**: [MBS Online](https://www.mbsonline.gov.au/)

### 1.4 Private Health Insurance Billing

Ramsay uses **"one in, all in" negotiation approach** with insurers:
- If insurer doesn't agree to terms, members cannot access any Ramsay hospitals
- Creates strong leverage for rate negotiations
- H1 FY2025: Improved indexation rates from private health insurers noted as growth driver

**PHI contract structure**:
- Rates negotiated per episode type/DRG category
- Performance indicators and quality metrics often tied to contracts
- Annual indexation negotiations critical for margin protection

**Source**: [MatrixBCG Ramsay Analysis](https://matrixbcg.com/blogs/how-it-works/ramsayhealth)

### 1.5 Coding Standards

#### ICD-10-AM (Australian Modification)
- **Diagnosis coding** for all hospital episodes
- Australian modification of WHO ICD-10
- Current edition: 13th Edition (effective July 2025)
- Updated every 3 years in sync with AR-DRG updates

#### ACHI (Australian Classification of Health Interventions)
- **Procedure coding** aligned with MBS
- Originally based on MBS structure
- Used to report procedure codes for reimbursement

#### ACS (Australian Coding Standards)
- Rules governing correct application of ICD-10-AM and ACHI
- Mandatory for all public and private hospitals

**Sources**: [IHACPA ICD-10-AM](https://www.ihacpa.gov.au/health-care/classification/icd-10-amachiacs), [ACCD](https://www.accd.net.au/icd-10-am-achi-acs/)

### 1.6 AR-DRG System

**Australian Refined Diagnosis Related Groups** drive casemix funding:

- Administered by Independent Health and Aged Care Pricing Authority (IHACPA)
- Groups clinically similar treatments for activity-based funding
- Current: AR-DRG V11.0 (from July 2025), V12.0 anticipated July 2026
- Used for public hospital activity-based funding
- PHI contracts often reference AR-DRG for rate setting

**Classification process**:
1. Clinical coder reviews patient record at discharge
2. Assigns ICD-10-AM codes (principal + additional diagnoses)
3. Assigns ACHI codes for procedures
4. AR-DRG grouper software determines DRG assignment
5. DRG determines reimbursement rate

**Source**: [IHACPA AR-DRGs](https://www.ihacpa.gov.au/health-care/classification/admitted-acute-care/ar-drgs)

### 1.7 Revenue Cycle Pain Points

| Challenge | Impact | Root Cause |
|-----------|--------|------------|
| **Coding workforce shortage** | Delayed billing, quality issues | COVID impact, training pipeline |
| **Incomplete documentation** | DRG downcoding, revenue loss | Verbal care plans not documented |
| **Discharge summary delays** | Coding backlogs | Clinician workload |
| **Post-billing audits** | Missed errors before claim submission | Audit timing issues |
| **PHI contract complexity** | Administrative burden | Multiple fund relationships |
| **VMO billing fragmentation** | Revenue not captured at facility level | Separate billing streams |

**Source**: [Code Focus Australia](https://codefocus.com.au/clinical-coding-how-it-has-an-impact-on-your-hospitals-health/)

---

## 2. UK Billing & Revenue Cycle

### 2.1 Market Position
- Part of Ramsay Health Care UK Operations Limited
- Mix of NHS contract work and private pay patients
- Licensed by Monitor (NHS regulator for providers)
- Subject to CMA Private Healthcare Market Investigation Order 2014

### 2.2 NHS Tariff System

#### NHS Payment Scheme (NHSPS)
Replaced National Tariff Payment System under 2022 Health and Care Act:

- **Aligned Payment and Incentive (API)**: Covers almost all NHS provider activity
- **Variable element**: Elective activity paid at 100% of NHSPS unit prices
- **2023/25 NHSPS**: Two-year pricing period (2023/24 and 2024/25)

**Key principle**: All providers (public/private) paid at same fixed national tariff.

**Source**: [NHS England National Tariff](https://www.england.nhs.uk/pay-syst/national-tariff/)

#### Healthcare Resource Groups (HRG4+)
- UK equivalent of DRGs
- Uses ICD-10 (diagnosis) + OPCS-4 (procedures) to classify episodes
- NHS Digital grouper software performs classification
- Determines payment for NHS-funded activity

**Source**: [NHS England Payment by Results Guide](https://assets.publishing.service.gov.uk/government/uploads/system/uploads/attachment_data/file/213150/PbR-Simple-Guide-FINAL.pdf)

### 2.3 Private Pay Billing

**Key differences from NHS billing**:

| Aspect | NHS Billing | Private Pay |
|--------|-------------|-------------|
| Coding system | OPCS-4 / ICD-10 | CCSD (Clinical Coding and Schedule Development) |
| Payment basis | HRG tariff | Fee-for-service, negotiated rates |
| Consultant fees | Included in tariff | Billed separately |
| Outpatient coding | Limited | Full procedure coding |

**OPCS limitations for private sector**:
- Not designed for direct reimbursement
- Doesn't unbundle separately-billed elements (consultant time, anaesthetist)
- Doesn't cover non-procedural outpatient activity

**Source**: [Healthcode Clinical Coding White Paper](https://www.healthcode.co.uk/wp-content/uploads/2022/09/HC_ClinicalCoding_WhitePaper_PathtoICD-10-Final.pdf)

### 2.4 Coding Standards

#### ICD-10
- Mandatory for diagnosis coding across NHS
- NHS Fundamental Information Standard
- Part of NHS Standard Contracts

#### OPCS-4
- **Office of Population Censuses and Surveys Classification** (4th revision)
- Mandatory for procedure coding in NHS
- Current: OPCS-4.10 NCCS-2025
- All Consultant Episodes containing procedures must use OPCS-4

**Source**: [NHS Digital Clinical Classifications](https://digital.nhs.uk/services/terminology-and-classifications/clinical-classifications)

### 2.5 Insurance Billing

Private Medical Insurance (PMI) billing considerations:
- PHIN (Private Healthcare Information Network) data reporting requirements
- Healthcode as billing intermediary
- ICD-10 adoption in private sector still maturing
- Potential for dual OPCS + CCSD coding during transition

**CMA requirements**: Private hospital operators must publish certain pricing/quality information on websites.

### 2.6 Revenue Cycle Pain Points

| Challenge | Impact | Root Cause |
|-----------|--------|------------|
| **Dual coding systems** | Administrative complexity | NHS vs private sector standards |
| **Invoice timing pressure** | Quality vs speed trade-off | Commercial dynamics of private sector |
| **HRG4+ complexity** | Classification disputes | Grouper algorithm interpretation |
| **Mixed payer reconciliation** | AR complexity | NHS tariff + private rates |
| **PHIN compliance** | Additional reporting burden | Regulatory requirements |

---

## 3. France Billing & Revenue Cycle

### 3.1 Market Position
- **Ramsay Santé**: #1 private hospitalization in France by establishments
- **154 establishments** across France
- Established in France 2010 (formerly Générale de Santé)
- Primary competitor: Elsan

### 3.2 T2A (Tarification à l'Activité)

France's activity-based payment system since 2004:

**Key characteristics**:
- Unified billing framework for public and private hospitals
- Annual tariffs set by Minister of Health
- Based on Groupe Homogène de Séjours (GHS) classification
- €47.4 billion in tariff revenue (2019) = 24% of national health objective

**Revenue composition by hospital type**:
| Sector | T2A % of Total Revenue |
|--------|------------------------|
| Public hospitals | 59.2% |
| Private non-profit | 69.2% |
| **Private for-profit** | **81.4%** |

**Implication**: Ramsay Santé highly dependent on T2A optimization.

**Source**: [Ameli T2A Guide](https://www.ameli.fr/etablissement/textes-reference/tarifications/tarification-activite-t2a), [Cour des comptes](https://www.ccomptes.fr/fr/publications/la-tarification-lactivite)

### 3.3 GHM/GHS Classification

#### PMSI (Programme de Médicalisation des Systèmes d'Information)
- Hospital information system for activity classification
- Monthly data uploads to ATIH (Agence Technique de l'Information sur l'Hospitalisation)
- Drives activity-based payments

#### Classification hierarchy:
1. **CMD (Catégories Majeures Diagnostiques)**: Major diagnostic categories
2. **GHM (Groupe Homogène de Malades)**: Homogeneous patient groups (like DRGs)
3. **GHS (Groupe Homogène de Séjours)**: Payment categories linked to GHM

**Current versions** (2025):
- GHM v30 (June 2025)
- CIM-10 updated March 2025
- CCAM v79.10 (September 2025)

**Source**: [SNDS Documentation](https://documentation-snds.health-data-hub.fr/snds/glossaire/cim)

### 3.4 Coding Standards

#### CIM-10 (Classification Internationale des Maladies)
- French version of ICD-10 for diagnoses
- Codes: Principal diagnosis (DP), associated diagnoses (DAS), complications (CMA, CMAS)

#### CCAM (Classification Commune des Actes Médicaux)
- French procedure classification (since 2004)
- Regulatory tool for PMSI procedure coding
- Replaced Catalogue des actes médicaux (CdAM)

**Coding workflow**:
1. Clinical documentation captured during stay
2. Coder assigns CIM-10 codes for all diagnoses
3. CCAM codes assigned for all procedures
4. PMSI grouper determines GHM classification
5. GHS determines reimbursement amount

**Source**: [AideAuCodage.fr](https://www.aideaucodage.fr/cim), [ResearchGate CCAM Development](https://www.researchgate.net/publication/26239663_The_Development_of_CCAM_The_New_French_Coding_System_of_Clinical_Procedures)

### 3.5 Sécurité Sociale + Mutuelle Billing

**Dual-payer structure**:

| Payer | Coverage | Role |
|-------|----------|------|
| **Assurance Maladie** (Sécurité sociale) | ~60% | Statutory health insurance |
| **Mutuelle** (complementary) | ~40% | Private supplementary insurance |
| Patient | Variable | Co-pays, deductibles |

**Billing flow**:
1. Hospital submits PMSI data to ATIH
2. T2A payment calculated based on GHS
3. Assurance Maladie pays statutory portion
4. Mutuelle covers complementary portion
5. Patient responsible for any remainder

**Ramsay Services (home care)**: 60% Sécurité sociale / 40% mutuelle standard split

**Source**: [Ramsay Services FAQ](https://www.ramsayservices.fr/faq)

### 3.6 Emerging Payment Models

Ramsay Santé experimenting with **capitation pricing** in primary care centers:
- Lump sum based on patient panel characteristics (age, sex, comorbidities)
- Mirrors Capio's Swedish model
- Alternative to pure T2A volume-based payment

**Source**: [Politis Ramsay Analysis](https://www.politis.fr/articles/2022/09/sante-comment-le-mastodonte-ramsay-soigne-sa-rentabilite-44783/)

### 3.7 Revenue Cycle Pain Points

| Challenge | Impact | Root Cause |
|-----------|--------|------------|
| **T2A incentives for LOS reduction** | Quality vs revenue tension | Fixed payment regardless of stay length |
| **Prudential coefficient** | Revenue withheld by government | FY2024: 100% withheld (€14.7M prior year) |
| **PMSI coding complexity** | Training requirements | Multiple classification systems |
| **ATIH audit exposure** | Reimbursement clawbacks | Documentation/coding discrepancies |
| **Mutuelle fragmentation** | Multiple payer reconciliation | Hundreds of mutuelle organizations |

---

## 4. Nordics Billing & Revenue Cycle

### 4.1 Market Position (Capio)
Acquired by Ramsay in 2018, Capio operates:

| Country | Facilities | Focus Areas |
|---------|------------|-------------|
| **Sweden** | 100+ health centers, 30+ specialist clinics | Primary care, mental health, St. Göran Hospital |
| **Norway** | 10 health centers, 7 specialist centers | Outpatient, rehabilitation, ophthalmology |
| **Denmark** | Multiple clinics | Day patient services |

**Key contract**: St. Göran Hospital (Stockholm) - 8+ year contract from Jan 2026, ~€4.8B value

**Source**: [Ramsay Santé Sweden](https://www.ramsaysante.eu/countries/ramsay-sante-sweden), [Ramsay Santé Denmark](https://www.ramsaysante.eu/countries/ramsay-sante-denmark)

### 4.2 Swedish Healthcare Funding

**Decentralized structure**:
- **21 Regions**: Finance and organize healthcare
- **290 Municipalities**: Responsible for elderly/disability care
- **Private operators**: Publicly funded via competitive tenders (5-8 year contracts)

**Payment models**:
- Capitation-based contracts (per-patient funding)
- Activity-based components using NordDRG
- Global budgets for certain contracts

**Source**: [Ramsay Santé Universal Registration Document 2023](https://www.ramsayhealth.com/globalassets/global/investor-centre/investor-centre-pdfs/ramsay-sante-universal-registration-document-2023.pdf)

### 4.3 NordDRG System

**Nordic DRG classification**:
- Developed jointly by Nordic countries (Sweden, Norway, Denmark, Finland)
- Based on HCFA-DRG v12 structure
- First grouper completed 1996
- Updated annually via NordDRG maintenance process

**Input classifications**:
- **ICD-10**: Diagnosis codes (national modifications: ICD-10-SE for Sweden)
- **NCSP (NOMESCO Classification of Surgical Procedures)**: Procedure codes
- **KVÅ (Sweden)**: Swedish procedure nomenclature

**DRG determination**: Combination of procedure code (KVÅ) + diagnosis code (ICD-10)

**Source**: [NordCase Products](https://nordcase.org/products/), [NordDRG ICD+ and NCSP+](http://www.nordcase.org/eng/materials/basic-classification)

### 4.4 Country-Specific Coding

#### Sweden
- **ICD-10-SE**: Swedish translation/modification (1997 base, annual updates)
- **KVÅ**: National Board of Health and Welfare maintains
- Mandatory procedure reporting to National Patient Register (since 2007)
- Primary care procedure coding: Not mandatory for GPs

#### Norway
- ICD-10 Norwegian modification
- NCSP for procedures
- Activity-based funding in hospital sector

#### Denmark
- ICD-10 Danish modification
- NordDRG for hospital classification
- Mix of global budgets and activity-based payment

**Source**: [MTR Consult Sweden Market Access](https://mtrconsult.com/market-access-medical-technologies-sweden), [WHO ICD Implementation Sweden](https://apps.who.int/gho/data/view.whofic.SWE-icd?lang=en)

### 4.5 Revenue Cycle Pain Points

| Challenge | Impact | Root Cause |
|-----------|--------|------------|
| **Contract-based revenue** | Volume vs margin trade-offs | Fixed-price tender awards |
| **Regional variation** | Complex compliance | 21 regions with different requirements |
| **Primary care coding gaps** | Activity not captured | GP procedure coding not mandatory |
| **Specialty volume fluctuations** | Revenue volatility | Day patient demand changes (e.g., ophthalmology) |
| **Currency exposure** | P&L translation | SEK/NOK/DKK vs EUR reporting |

---

## 5. AI Opportunities by Region

### 5.1 Market Context

**Global CDI market**: USD 5.13B (2023) → USD 9.96B (2032), 7.66% CAGR

**AI adoption in revenue cycle**:
- 63% of healthcare organizations have integrated AI-powered automation
- 46% of hospitals use AI in RCM operations
- 74% have some form of revenue cycle automation (AI + RPA)

**Source**: [SNS Insider CDI Market Report](https://www.globenewswire.com/news-release/2024/10/24/2968811/0/en/Clinical-Documentation-Improvement-Market-Size-to-Reach-USD-9-96-Billion-by-2032-Driven-by-EHR-Adoption-and-Regulatory-Compliance-SNS-Insider.html)

### 5.2 Auto-Coding Opportunities

| Region | System | AI Readiness | Opportunity |
|--------|--------|--------------|-------------|
| **Australia** | ICD-10-AM/ACHI | HIGH | Mature coding standards, good training data |
| **France** | CIM-10/CCAM | HIGH | PMSI standardization enables automation |
| **UK** | ICD-10/OPCS-4 | MEDIUM | NHS standards clear; private sector fragmented |
| **Nordics** | ICD-10-SE/NordDRG | MEDIUM | Smaller market, multi-country complexity |

**Auto-coding capability**:
- Current AI platforms: 94%+ claims coded without human intervention
- Accuracy: 99%+ achievable with modern NLP
- XpertDox partnership example: 15% jump in charge capture, 60% improvement in quality code capture

**Source**: [XpertDox AI Medical Coding 2024](https://www.xpertdox.com/blog/ai-medical-coding-2024-guide/)

### 5.3 CDI Opportunities

**Revenue impact of CDI**:
- Up to **$4,900 per corrected inpatient claim** (US benchmark)
- Total "at-risk" revenue: ~$11.2M per healthcare organization
- Industry benchmark: 5-20% documentation improvement rate

**AI-assisted CDI capabilities**:
1. **Structuring data**: Organizing unstructured clinical notes
2. **Annotating notes**: Flagging coding-relevant documentation
3. **Error detection**: Identifying documentation gaps before billing
4. **CDI querying**: Automated alerts for incomplete documentation
5. **Trend identification**: Pattern analysis across patient populations

**Regional CDI priorities**:

| Region | Priority CDI Focus |
|--------|-------------------|
| Australia | Discharge summary completeness, DRG optimization |
| France | GHM accuracy, T2A tariff capture |
| UK | HRG classification, NHS contract compliance |
| Nordics | NordDRG accuracy, cross-country consistency |

**Source**: [PMC CDI AI Systematic Review](https://pmc.ncbi.nlm.nih.gov/articles/PMC11605373/), [MDClarity CDI Metrics](https://www.mdclarity.com/rcm-metrics/clinical-documentation-improvement-cdi-effectiveness)

### 5.4 Denial Management

**Current denial landscape**:
- Initial claim denials: **11.8% in 2024** (up from 10.2%)
- Medicare Advantage denials: +4.8% spike 2023-2024
- 15% of private payer claims rejected on first submission
- 60% of denied claims never resubmitted
- Cost to rework denials: $181/claim for hospitals

**AI denial management capabilities**:
- Prior authorization automation
- Document completeness checking
- Payer requirement matching
- Appeal generation

**Results from early adopters**:
- 22% decrease in prior-authorization denials
- 18% decrease in coverage denials
- 30-35 hours/week saved per organization
- 40% less manual work, 30% faster reimbursements

**Regional applicability**:

| Region | Denial Risk | AI Value |
|--------|-------------|----------|
| Australia | PHI claim disputes, MBS audit | HIGH - multiple payer complexity |
| France | T2A audit/clawback | MEDIUM - regulatory focus |
| UK | NHS tariff disputes | MEDIUM - standardized tariffs |
| Nordics | Contract compliance | LOW - contract-based model |

**Source**: [HFMA Denial Management](https://www.hfma.org/revenue-cycle/denials-management/health-systems-start-to-fight-back-against-ai-powered-robots-driving-denial-rates-higher/), [Healthcare IT Today Revenue Leakage](https://www.healthcareittoday.com/2024/02/23/three-ways-ai-is-preventing-revenue-leakage/)

### 5.5 Revenue Leakage Prevention

**Common leakage sources**:
1. Under-coding due to documentation gaps
2. Missed secondary diagnoses/complications
3. Procedure code omissions
4. Incorrect DRG assignment
5. Late charge capture

**AI leakage prevention strategies**:

| Strategy | Technology | Expected Impact |
|----------|------------|-----------------|
| Real-time CDI alerts | NLP on clinical notes | 5-20% documentation improvement |
| Pre-bill audit | ML classification | Catch errors before submission |
| Charge integrity | Rules + ML | Reduce under-billing |
| DRG validation | Grouper + AI review | Optimize case mix index |
| Contract compliance | Automated payer rules | Ensure rate accuracy |

**Source**: [AHA AI Revenue Cycle](https://www.aha.org/aha-center-health-innovation-market-scan/2024-06-04-3-ways-ai-can-improve-revenue-cycle-management)

### 5.6 Priority Matrix: AI Investment by Region

| Initiative | Australia | France | UK | Nordics | Investment Priority |
|------------|-----------|--------|----|---------|--------------------|
| **Auto-coding** | HIGH | HIGH | MEDIUM | MEDIUM | 1st |
| **CDI** | HIGH | HIGH | MEDIUM | LOW | 2nd |
| **Denial Management** | HIGH | MEDIUM | MEDIUM | LOW | 3rd |
| **Revenue Leakage** | HIGH | HIGH | MEDIUM | MEDIUM | 4th |

**Rationale**:
- **Australia first**: Largest revenue contribution, mature standards, multiple payer complexity
- **France second**: Heavy T2A dependence (81.4% of revenue), regulatory audit risk
- **UK third**: Mixed NHS/private creates complexity, but lower margin contribution
- **Nordics fourth**: Contract-based model limits RCM AI value; focus on operational efficiency

---

## 6. Recommendations

### 6.1 Near-Term (0-12 months)

1. **Australia CDI pilot**: Deploy AI-assisted CDI at 2-3 high-volume hospitals
   - Target: Improve discharge summary completion rates
   - KPI: 10% reduction in coding query volume

2. **France auto-coding PoC**: Evaluate NLP-based PMSI coding assistance
   - Target: Reduce coder turnaround time
   - KPI: 20% improvement in coding throughput

3. **Cross-regional coding analytics**: Unified dashboards for coding KPIs
   - Track: CMI trends, coding accuracy, documentation completeness
   - Enable: Benchmarking across regions

### 6.2 Medium-Term (12-24 months)

1. **Australia denial prevention**: AI-powered claim review before submission
   - Target: PHI claim acceptance rate improvement
   - KPI: 5% reduction in initial denials

2. **France T2A optimization**: GHM accuracy improvement through AI review
   - Target: Maximize appropriate T2A capture
   - KPI: 2% CMI improvement

3. **UK coding standardization**: Support ICD-10 adoption in private sector
   - Enable: Unified coding across NHS and private activity
   - KPI: Single coding workflow implementation

### 6.3 Long-Term (24+ months)

1. **Enterprise coding automation**: Centralized AI coding platform
   - Multi-classification support: ICD-10-AM, CIM-10, ICD-10, ICD-10-SE
   - Procedure mapping: ACHI, CCAM, OPCS-4, NCSP
   - DRG optimization: AR-DRG, GHM, HRG, NordDRG

2. **Real-time revenue intelligence**: Predictive analytics for revenue cycle
   - Contract performance monitoring
   - Payer behavior analysis
   - Margin optimization by service line

---

## 7. Key Sources

### Australia
- [Ramsay Health Care Australia Overview](https://www.ramsayhealth.com/en/investors/our-markets/australia-healthcare-overview/)
- [MBS Online](https://www.mbsonline.gov.au/)
- [IHACPA ICD-10-AM/ACHI/ACS](https://www.ihacpa.gov.au/health-care/classification/icd-10-amachiacs)
- [IHACPA AR-DRGs](https://www.ihacpa.gov.au/health-care/classification/admitted-acute-care/ar-drgs)
- [Code Focus Clinical Coding](https://codefocus.com.au/clinical-coding-how-it-has-an-impact-on-your-hospitals-health/)

### UK
- [Ramsay Health Care UK Overview](https://www.ramsayhealth.com/en/investors/our-markets/uk-healthcare-overview/)
- [NHS England National Tariff](https://www.england.nhs.uk/pay-syst/national-tariff/)
- [NHS Digital Clinical Classifications](https://digital.nhs.uk/services/terminology-and-classifications/clinical-classifications)
- [Healthcode Clinical Coding White Paper](https://www.healthcode.co.uk/wp-content/uploads/2022/09/HC_ClinicalCoding_WhitePaper_PathtoICD-10-Final.pdf)

### France
- [Ramsay Santé EU](https://www.ramsaysante.eu/)
- [Ameli T2A Guide](https://www.ameli.fr/etablissement/textes-reference/tarifications/tarification-activite-t2a)
- [SNDS/Health Data Hub Documentation](https://documentation-snds.health-data-hub.fr/snds/glossaire/cim)
- [AideAuCodage](https://www.aideaucodage.fr/cim)

### Nordics
- [Ramsay Santé Sweden](https://www.ramsaysante.eu/countries/ramsay-sante-sweden)
- [NordCase NordDRG](https://nordcase.org/products/)
- [WHO ICD Implementation Database - Sweden](https://apps.who.int/gho/data/view.whofic.SWE-icd?lang=en)

### AI & Revenue Cycle
- [PMC: AI in Clinical Documentation Improvement](https://pmc.ncbi.nlm.nih.gov/articles/PMC11605373/)
- [HFMA: AI in Revenue Cycle](https://www.hfma.org/technology/most-healthcare-organizations-are-adopting-ai-in-the-revenue-cycle-hfma-poll/)
- [Healthcare IT Today: AI Revenue Leakage](https://www.healthcareittoday.com/2024/02/23/three-ways-ai-is-preventing-revenue-leakage/)
- [SNS Insider: CDI Market Report](https://www.globenewswire.com/news-release/2024/10/24/2968811/0/en/Clinical-Documentation-Improvement-Market-Size-to-Reach-USD-9-96-Billion-by-2032-Driven-by-EHR-Adoption-and-Regulatory-Compliance-SNS-Insider.html)

---

*Analysis prepared for Healthcare AI Vendor Analysis project*
*November 2025*
