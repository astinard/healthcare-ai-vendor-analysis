# Australian Healthcare AI Regulatory Environment
## Comprehensive Regulatory Analysis

**Date:** November 2025
**Scope:** TGA Framework, Privacy Laws, Medical Board Guidance, Government Initiatives, International Comparisons

---

## Executive Summary

Australia's healthcare AI regulatory landscape is rapidly evolving, characterized by a **technology-agnostic, risk-based approach** rather than AI-specific legislation. Key regulatory bodies include the Therapeutic Goods Administration (TGA), Office of the Australian Information Commissioner (OAIC), Australian Health Practitioner Regulation Agency (AHPRA), and Australian Digital Health Agency (ADHA). The framework emphasizes practitioner accountability, patient safety, and alignment with international standards while maintaining flexibility for emerging technologies.

---

## 1. TGA Framework for AI Medical Devices

### 1.1 Software as Medical Device (SaMD) Classification

The TGA regulates AI and machine learning in healthcare through its **Software as Medical Device (SaMD) framework**, which underwent significant changes effective **November 1, 2024**.

#### Classification System

| Class | Risk Level | Examples | Regulatory Pathway |
|-------|------------|----------|-------------------|
| **Class I** | Low | General wellness apps, simple data logging | Self-certification |
| **Class IIa** | Low-Moderate | Diagnostic decision support, clinical monitoring | Conformity assessment |
| **Class IIb** | Moderate-High | Digital therapeutics with potential patient harm | Notified body certification |
| **Class III** | High | Life-threatening screening/diagnosis/dosing decisions | Full TGA assessment |

**Key Classification Principles:**
- SaMD is classified according to its **potential to cause harm** through provision of incorrect information
- AI as a "means to an end" (lower risk) vs. AI providing "final output" (higher risk)
- Human clinical judgment remains the gold standard—TGA does not currently approve AI that cannot be verified by users

### 1.2 AI/ML Specific Guidance

The TGA published its landmark **"Report: Clarifying and strengthening the regulation of Medical Device Software including Artificial Intelligence"** on July 25, 2025.

#### Evidence Requirements for AI Software

Manufacturers must provide evidence demonstrating:

1. **Algorithm Transparency**
   - Description of algorithm and model design
   - Information on training and testing phases
   - Explanation of how AI/ML contributes to intended purpose

2. **Data Generalizability**
   - Justification that training data is appropriate for Australian population
   - Consideration of sub-populations and demographic variations

3. **AI-Specific Risk Management**
   - Overfitting mitigation strategies
   - Bias identification and management
   - Performance degradation monitoring (data drift)

4. **Lifecycle Evidence**
   - Pre-market validation
   - Robust post-market monitoring practices
   - Change control documentation

#### Generative AI and LLMs

Software incorporating **generative AI, LLMs, text generators, and multimodal AI** is explicitly regulated as medical devices. Key requirements:
- Clinical and technical evidence must demonstrate safety, reliability, and performance to **same standard as other medical devices**
- Where developers adapt, build on, or incorporate an LLM, they are deemed the **manufacturer** with full regulatory obligations under Section 41BD of the Therapeutic Goods Act 1989

### 1.3 Clinical AI Requirements

#### ARTG Registration

All AI-enabled medical devices supplied in Australia must be included in the **Australian Register of Therapeutic Goods (ARTG)**, regardless of where the manufacturer is based. The TGA maintains a [public list of AI-enabled medical devices in the ARTG](https://www.tga.gov.au/news/news/list-ai-enabled-medical-devices-artg).

#### Essential Principles Compliance

AI medical devices must comply with the **Essential Principles** covering:
- Safety and performance throughout expected lifetime
- Risk management proportionate to benefits
- Information to be provided with device
- Clinical evidence requirements

### 1.4 Recent Regulatory Changes & Future Direction

#### November 2024 Transition
- Grace period ended November 1, 2024
- Full implementation of February 2021 classification rule changes
- Mandatory conformity assessment with TGA for applicable devices

#### 2025 AI Review Outcomes
- **$39.9 million** over 5 years allocated for Safe and Responsible AI development
- Increased education and guidance for technology sector
- Targeted compliance action to remove unapproved devices from market
- Review of software exclusions, particularly digital mental health tools and consumer health products

#### Emerging Regulatory Concerns
- **Adaptive AI**: Systems that change functionality post-deployment require new approaches to change control, validation, and monitoring
- **Open datasets**: Scrutiny of training data provenance and quality
- **Laboratory information management systems**: Urgent review of exclusions

#### Future Consultations (2025-2026)
- Targeted consultations on regulatory reform
- Addressing gaps in adaptive AI regulation
- Clarification of exclusion criteria

---

## 2. Privacy Framework

### 2.1 Privacy Act 1988 Overview

The **Privacy Act 1988** establishes the national framework for privacy protection in Australia, administered by the **Office of the Australian Information Commissioner (OAIC)**.

#### Scope of Application

| Category | Covered | Notes |
|----------|---------|-------|
| Businesses >$3M turnover | Yes | Standard threshold |
| Health service providers | **Always** | Regardless of turnover |
| Businesses trading in personal information | **Always** | Including data brokers |
| Australian Government contractors | **Always** | If handling personal information |

**Critical for Healthcare AI:** All organizations providing health services and holding health information are covered, **regardless of business size**.

### 2.2 Australian Privacy Principles (APPs)

The **13 Australian Privacy Principles** in Schedule 1 of the Privacy Act govern:

| APP | Principle | Healthcare AI Relevance |
|-----|-----------|------------------------|
| 1 | Open and transparent management | Privacy policies must address AI use |
| 2 | Anonymity and pseudonymity | Options for de-identified data in AI training |
| 3 | Collection of solicited personal information | Limits on health data collection for AI |
| 4 | Dealing with unsolicited information | Managing incidental AI data collection |
| 5 | Notification of collection | Informing patients of AI data use |
| 6 | Use or disclosure | Restricting AI access to necessary data |
| 7 | Direct marketing | Prohibitions on using health AI for marketing |
| 8 | Cross-border disclosure | International AI processing restrictions |
| 9 | Adoption, use, or disclosure of identifiers | Healthcare identifier protection |
| 10 | Quality of personal information | AI training data accuracy requirements |
| 11 | Security of personal information | AI system security obligations |
| 12 | Access to personal information | Patient access to AI-derived information |
| 13 | Correction of personal information | Correcting AI-processed records |

### 2.3 Health-Specific Privacy Rules

#### Definition of Health Information

Section 6 of the Privacy Act defines health information to include:
- Information about physical, mental, or psychological health
- Disability information
- Health service provision records
- **Genetic information** (predictive of health of individual or genetic relatives)
- Organ donor information

#### Special Protections

Health information receives **enhanced protection** as one of the most sensitive types of personal information:
- More restrictive collection conditions
- Heightened consent requirements
- Additional security obligations
- Stricter cross-border transfer rules

#### Research Guidelines

The **NHMRC Guidelines** under Sections 95 and 95A of the Privacy Act provide frameworks for:
- Using health information for research without consent
- Human Research Ethics Committee (HREC) assessment requirements
- Balancing public interest in research against privacy protection

### 2.4 AI-Specific Privacy Considerations

#### Dynamic Privacy Protection

Unlike traditional static privacy controls, AI systems require **dynamic protection** because:
- AI systems evolve through updates and retraining
- Integration with new data sources creates new risks
- Continuous learning may inadvertently capture personal information

#### Data Minimization

**Cornerstone principle** for privacy-preserving AI:
- Configure systems to use **minimum personal information** necessary
- Example: Fall detection using anonymized movement patterns rather than identified video
- Prefer de-identification and aggregation where possible

#### Cybersecurity Risks

The **Australian Signals Directorate** identifies healthcare AI as facing heightened risks:
- Data poisoning attacks on training data
- Adversarial inputs to AI systems
- Aged care sector specifically identified as **HIGH-RISK** for cyberattacks

### 2.5 State and Territory Variations

Australia has a **patchwork** of state-level health privacy legislation:

#### New South Wales (NSW)

**Legislation:** Health Records and Information Privacy Act 2002 (HRIP Act)

| Aspect | Requirement |
|--------|-------------|
| Coverage | Public and private sector |
| Principles | 15 Health Privacy Principles (HPPs) |
| Retention | 7 years from last service (adults); Until age 25 (children) |
| Oversight | NSW Information and Privacy Commission |

#### Victoria

**Legislation:** Health Records Act 2001

| Aspect | Requirement |
|--------|-------------|
| Coverage | Public and private sector |
| Principles | 11 Health Privacy Principles |
| Retention | 7 years from last service; Until age 25 (children) |
| Cross-border | Only to jurisdictions with substantially similar laws |
| Oversight | Office of the Victorian Information Commissioner |

#### Queensland

**Legislation:** Information Privacy Act 2009 (public sector only)

| Aspect | Requirement |
|--------|-------------|
| Coverage | Public sector only |
| Health specific | Part 7, Health Services Act 1991 (public sector confidentiality) |
| Private sector | Federal Privacy Act applies |
| Oversight | Queensland Office of the Information Commissioner |

#### Other Jurisdictions

| State/Territory | Health-Specific Privacy Law |
|-----------------|----------------------------|
| Western Australia | **None** - Federal Privacy Act applies |
| South Australia | **None** - Federal Privacy Act applies |
| Tasmania | Personal Information Protection Act 2004 (public sector) |
| ACT | Health Records (Privacy and Access) Act 1997 |
| Northern Territory | Information Act 2002 (public sector) |

#### Implications for AI Vendors

- **Multi-state compliance** required for national deployment
- Victoria's **cross-border restrictions** impact cloud-hosted AI
- NSW and Victoria require **dedicated compliance programs** for health information
- Queensland private sector defaults to **federal framework**

---

## 3. Medical Board & AHPRA Guidance

### 3.1 AHPRA Guidance on AI in Healthcare

The Australian Health Practitioner Regulation Agency (AHPRA) and National Boards have published guidance on **"Meeting your professional obligations when using Artificial Intelligence in healthcare."**

#### Position Statement

AHPRA **welcomes** the use of AI in healthcare, citing potential to:
- Improve health outcomes
- Create more person-centered health systems
- Enhance clinical decision-making

However, the guidance emphasizes that **existing professional obligations apply** when using AI.

### 3.2 Five Key Principles

#### Principle 1: Accountability

> "Practitioners must meet professional obligations and apply human judgment to any output of AI"

- Individual health practitioners are **responsible for any and all AI** used in their practice
- Ultimate responsibility for patient care remains with the human professional
- AI assistance does not transfer or dilute practitioner accountability

#### Principle 2: Understanding

> "Practitioners should understand enough about AI intended for use, including how it is trained, tested, and its limitations"

Requirements include understanding:
- How the AI system was trained and validated
- Known limitations and failure modes
- Appropriate use cases and contraindications
- Population the AI was designed for

#### Principle 3: Transparency

> "Practitioners are expected to inform patients about AI use and address concerns"

- Proactive disclosure of AI involvement in care
- Clear explanation of AI's role in clinical decisions
- Addressing patient questions and concerns

#### Principle 4: Informed Consent

> "Practitioners should involve patients in AI use and obtain informed consent"

- AI use is part of informed consent discussions
- Patients can decline AI involvement in their care
- Documentation of consent for AI-assisted decisions

#### Principle 5: Ethical and Legal Compliance

Practitioners must ensure:
- Compliance with applicable legislation (especially privacy)
- Understanding of employer governance arrangements
- **Appropriate professional indemnity insurance** covering AI use

### 3.3 Practitioner Liability with AI

#### Medical Negligence Framework

When AI is involved in adverse outcomes, liability analysis considers:

| Scenario | Liability Analysis |
|----------|-------------------|
| Relying on incorrect AI diagnosis | Was the error detectable by a competent clinician? |
| Rejecting correct AI recommendation | Did rejection meet reasonable standard of care? |
| Failing to use available AI | Would a competent practitioner have used it? |
| Using unapproved AI system | Likely breach regardless of AI accuracy |

#### Key Legal Principles

- **Breach of duty**: Did conduct fall below expected standard of care?
- **Reasonable detection**: If AI error was so obscure no reasonable clinician could detect it, may not be negligent
- **TGA approval**: Does not insulate practitioners from liability
- **Reputation**: AI system reputation/approval status doesn't determine practitioner negligence

### 3.4 Informed Consent Requirements

#### Enhanced Consent Elements for AI

Beyond standard consent requirements, AI use requires:

1. **Disclosure of AI involvement** in diagnosis/treatment
2. **Explanation of AI's role** and level of autonomy
3. **Known limitations** relevant to patient's situation
4. **Alternative options** without AI assistance
5. **Data use implications** for privacy

#### Documentation Requirements

- Record AI tools used in clinical decision-making
- Document patient consent for AI-assisted care
- Note any patient requests to exclude AI involvement

### 3.5 Government Response to Liability Concerns

The **2025 Final Report on Safe and Responsible AI in Health Care** acknowledges:
- Existing legislation not fully equipped for AI risks in clinical environments
- Calls for national policy leadership
- Recommends tailored regulatory frameworks
- Proposes mandatory guardrails for high-risk AI applications

---

## 4. Government Initiatives

### 4.1 National Digital Health Strategy 2023-2028

Australia's federal, state, and territory governments have agreed to a **5-year digital health plan** administered by the Australian Digital Health Agency.

#### Strategic Priorities

1. **Safe, secure, and trustworthy digital health**
2. **Empowered individuals** managing their health digitally
3. **Enhanced health services** through digital transformation
4. **Data-driven insights** for better outcomes

#### AI Integration Vision

The Strategy acknowledges AI and emerging technologies will support:
- Increased staff efficiency
- Improved service delivery
- Personalized health management
- Predictive analytics for population health

### 4.2 Australian Digital Health Agency (ADHA) Role

#### Key Responsibilities

| Function | Description |
|----------|-------------|
| My Health Record | National digital health record system |
| Healthcare Identifiers | Managing HI Service |
| Interoperability | FHIR standards and integration |
| Policy Development | Digital health policy and guidelines |
| AI Governance | AI transparency and responsible use |

#### AI Transparency

ADHA published an **Artificial Intelligence Transparency Statement** detailing:
- Internal AI use policies
- Microsoft 365 Copilot trial participation
- Future AI adoption roadmap

### 4.3 Funding for AI Adoption

#### 2023 Federal Budget

**Over $1 billion** allocated for digital health initiatives including:
- Modernizing My Health Record
- Renewing Intergovernmental Agreement on National Digital Health
- Enhancing electronic prescribing capabilities

#### 2024-25 Federal Budget

**$39.9 million** over 5 years for:
- Safe and Responsible AI policy development
- Clarifying and strengthening existing laws
- Addressing AI risks in health and aged care regulation

#### National Policy Roadmap for AI in Healthcare

**Vision:** AI-enabled healthcare system delivering personalized, effective healthcare safely, ethically, and sustainably

**Mission:** Fully funded national plan by 2025 for AI-enabled Australian healthcare

**Key Gaps Identified:**
- Capability to translate AI into safe clinical services
- Regulatory clarity for adaptive AI
- Workforce skills and education
- Infrastructure for AI deployment

### 4.4 Telehealth Regulations

#### MBS Telehealth Framework

Post-COVID, Australia has **permanent telehealth arrangements** under the Medicare Benefits Schedule:

| Provider Type | Telehealth Access |
|---------------|------------------|
| GPs | Video and phone items |
| Specialists | Video and phone items |
| Allied Health | Video and phone items |
| Mental Health | Better Access telehealth items |
| Nurse Practitioners | Video and phone items |

#### Clinical Requirements

- **Video preferred** as face-to-face substitute
- Audio-only where clinically appropriate
- Same clinical requirements as in-person consultations
- **Safety and clinical appropriateness** determination required

#### MyMedicare Requirements

General practice telehealth items require:
- Patient registered with practice under MyMedicare
- Prior phone attendance (items 91900/91910) at that practice
- OR patient in COVID isolation/quarantine

#### Compliance Safeguards

- **80/20 Rule**: >80 services/day on >20 days in 12 months triggers PSR referral
- **30/20 Rule** (from July 2022): For consultant physicians and GP telephone attendances
- Geographic restrictions for some group therapy items

### 4.5 Health Connect Australia Strategy

In 2025, ADHA launched the **Health Connect Australia Strategy, Architecture and Roadmap** focused on:
- National digital health interoperability
- 13 strategic intents over 2025-2030+
- Architecture standards alignment
- Cross-jurisdictional data sharing

---

## 5. Comparison to US/EU Regulations

### 5.1 Australia vs. FDA (United States)

#### Regulatory Philosophy

| Aspect | Australia (TGA) | United States (FDA) |
|--------|-----------------|---------------------|
| **Primary Approach** | Risk-based, strengthening oversight | Risk-based, preventing overregulation |
| **AI-Specific Rules** | Technology-agnostic framework | Specific AI/ML guidance documents |
| **Adaptive AI** | Under development | PCCP (Predetermined Change Control Plan) pathway |
| **CDS Exclusions** | Narrow exclusions under review | Broader exclusions under 21st Century Cures Act |

#### Classification Comparison

| Device Type | TGA Classification | FDA Classification |
|-------------|-------------------|-------------------|
| Diagnostic decision support | Class IIa | Often excluded under Cures Act |
| Life-threatening screening | Class III | Class III (PMA) |
| Digital therapeutics (harm potential) | Class IIb | Class II (510(k)) |
| General wellness | Excluded | Excluded |

#### Key Differences

1. **Clinical Decision Support (CDS)**
   - FDA: 21st Century Cures Act **excludes** software providing recommendations for prevention, diagnosis, or treatment
   - TGA: Plans to **include** diagnostic decision support as Class IIa

2. **Regulatory Burden**
   - FDA: Generally seeks ways to prevent overregulation
   - TGA: Focus on strengthening oversight and compliance

3. **LLM/Generative AI**
   - Both regulate as medical devices when used for clinical purposes
   - TGA: Explicit guidance on developer-as-manufacturer for adapted LLMs

4. **Post-Market Surveillance**
   - FDA: PCCP for planned AI changes
   - TGA: Developing approach for adaptive AI

### 5.2 Australia vs. EU MDR/AI Act

#### Regulatory Structure

| Aspect | Australia | European Union |
|--------|-----------|----------------|
| **Device Regulation** | TGA (single regulator) | EU MDR (notified bodies) |
| **AI-Specific Law** | None (using existing framework) | EU AI Act (horizontal legislation) |
| **Dual Compliance** | Single framework | MDR/IVDR + AI Act overlap |
| **Risk Classification** | Device-focused | AI system + device classification |

#### EU's Dual Regulatory Burden

The EU requires compliance with **both**:

1. **EU MDR/IVDR** (Medical Device/IVD Regulations)
   - Device-specific requirements
   - Clinical evidence and QMS
   - CE marking

2. **EU AI Act** (Horizontal AI Legislation)
   - AI-specific requirements
   - Quality management
   - Transparency and human oversight
   - Considered "high-risk" for medical AI

**Implication:** Even **low-risk medical devices** under MDR are **high-risk** under AI Act if they involve notified body assessment.

#### Australia's Simpler Approach

- **Single framework** (TGA) covers both device and AI aspects
- No separate AI-specific legislation
- Considering Safe and Responsible AI framework (not yet legislated)
- Lower compliance complexity for manufacturers

#### Classification Alignment

Australia's SaMD classification rules are **broadly aligned with EU MDR** classifications, facilitating:
- Recognition of EU certifications
- Streamlined market access for EU-certified devices
- Harmonized evidence requirements

### 5.3 Implications for Vendors Entering Australia

#### Market Access Pathways

| Origin | Pathway | Notes |
|--------|---------|-------|
| **EU-Certified** | Recognized since 2018 | Streamlined entry |
| **FDA-Cleared** | Recognized since 2018 | Streamlined entry |
| **Singapore HSA** | Recognized since 2022 | Streamlined entry |
| **Other** | Full TGA assessment | Complete dossier required |

#### Strategic Considerations for US Vendors

**Advantages:**
- FDA recognition provides streamlined pathway
- Similar risk-based approach
- Lower regulatory burden than EU

**Challenges:**
- CDS excluded under FDA may be **Class IIa in Australia**
- Must demonstrate data generalizability for Australian population
- Stricter privacy framework than US (closer to GDPR)
- State-level health privacy compliance in NSW/Victoria

#### Strategic Considerations for EU Vendors

**Advantages:**
- Strong classification alignment
- EU MDR certification recognized
- Similar evidence requirements

**Challenges:**
- No AI Act compliance required (simpler)
- Must address Australia-specific data considerations
- Different post-market surveillance requirements

#### Key Compliance Requirements for All Vendors

1. **ARTG Registration**: Mandatory for market access
2. **Australian Sponsor**: Required local representative
3. **Data Generalizability**: Evidence for Australian population
4. **Privacy Compliance**: Federal + relevant state laws
5. **Post-Market Surveillance**: Australian-specific adverse event reporting
6. **Advertising Compliance**: TGA advertising code

---

## 6. Key Recommendations for Vendors

### 6.1 Regulatory Strategy

1. **Assess Classification Early**
   - TGA may classify CDS tools differently than FDA
   - Plan for potential Class IIa classification of decision support

2. **Prepare Australian Evidence Package**
   - Demographic appropriateness for Australian population
   - Sub-population considerations (Indigenous, rural)
   - Local clinical validation studies if required

3. **Establish Local Presence**
   - Appoint Australian sponsor
   - Consider local partnership for market access

### 6.2 Privacy Compliance

1. **Federal Compliance**
   - Full APP compliance regardless of business size
   - Data minimization in AI design
   - Cross-border transfer controls

2. **State Compliance**
   - NSW and Victoria require additional compliance
   - Consider data localization requirements
   - Cross-jurisdictional data sharing frameworks

### 6.3 Clinical Integration

1. **Practitioner Support Materials**
   - Clear documentation of AI limitations
   - Training materials for clinical users
   - Consent templates for AI-assisted care

2. **Liability Considerations**
   - Professional indemnity coverage for AI use
   - Clear allocation of responsibility
   - Transparency about AI role in clinical decisions

### 6.4 Ongoing Compliance

1. **Monitor Regulatory Evolution**
   - TGA consultations 2025-2026
   - Safe and Responsible AI developments
   - State privacy law changes

2. **Post-Market Requirements**
   - Australian adverse event reporting
   - Performance monitoring for data drift
   - Bias monitoring in Australian population

---

## Sources

### TGA & Medical Device Regulation
- [TGA: Artificial Intelligence (AI) and medical device software](https://www.tga.gov.au/how-we-regulate/manufacturing/manufacture-medical-device/manufacture-specific-types-medical-devices/artificial-intelligence-ai-and-medical-device-software)
- [TGA: Evidence requirements for software using AI](https://www.tga.gov.au/how-we-regulate/manufacturing/manufacture-medical-device/manufacture-specific-types-medical-devices/evidence-requirements-software-using-ai)
- [TGA: Understanding regulation of software-based medical devices](https://www.tga.gov.au/resources/guidance/understanding-regulation-software-based-medical-devices)
- [TGA: List of AI-enabled medical devices in the ARTG](https://www.tga.gov.au/news/news/list-ai-enabled-medical-devices-artg)
- [TGA: AI Review Outcomes Report Published](https://www.tga.gov.au/news/news/tga-ai-review-outcomes-report-published)
- [TGA: Technical Reference Group for SaMD and AI](https://www.tga.gov.au/about-tga/advisory-bodies-and-committees/technical-reference-group-software-medical-device-samd-and-artificial-intelligence-ai)
- [Freyr Solutions: SaMDs Regulation in Australia 2024 Updates](https://www.freyrsolutions.com/blog/australia-updates-regulation-of-software-as-medical-devices-samds)
- [MinterEllison: Innovation meets regulation - Medical devices and AI](https://www.minterellison.com/articles/innovation-meets-regulation-medical-devices-and-artificial-intelligence)
- [Lexology: TGA's 2025 AI Review Updates](https://www.lexology.com/library/detail.aspx?g=7511fc5f-84aa-4d0f-8f3b-8ce8345e2d7a)

### Privacy Framework
- [OAIC: The Privacy Act](https://www.oaic.gov.au/privacy/privacy-legislation/the-privacy-act)
- [OAIC: Guide to Health Privacy](https://www.oaic.gov.au/privacy/privacy-guidance-for-organisations-and-government-agencies/health-service-providers/guide-to-health-privacy)
- [OAIC: Health and Medical Research](https://www.oaic.gov.au/privacy/privacy-legislation/the-privacy-act/health-and-and-medical-research)
- [OAIC: State and Territory Privacy Legislation](https://www.oaic.gov.au/privacy/privacy-legislation/state-and-territory-privacy-legislation)
- [NSW Legislation: Health Records and Information Privacy Act 2002](https://legislation.nsw.gov.au/view/whole/html/inforce/current/act-2002-071)
- [Victoria Health: Health Records Act](https://www.health.vic.gov.au/legislation/health-records-act)
- [Ausmed: AI and Privacy in Healthcare](https://www.ausmed.com.au/organisations/toolbox/guides/ai-privacy)

### AHPRA & Medical Board
- [AHPRA: Meeting professional obligations when using AI in healthcare](https://www.ahpra.gov.au/Resources/Artificial-Intelligence-in-healthcare)
- [AHPRA: Further information about AI](https://www.ahpra.gov.au/Resources/Artificial-Intelligence-in-healthcare/Further-information-about-AI.aspx)
- [MinterEllison: AHPRA introduces AI guidance for health practitioners](https://www.minterellison.com/articles/ahpra-introduces-ai-guidelines-for-health-practitioners)
- [Meridian Lawyers: AHPRA issues guidance on using AI](https://www.meridianlawyers.com.au/insights/ahpra-issues-guidance-on-using-artificial-intelligence/)
- [Lexology: When machines malpractice - Liability for AI and robotic healthcare](https://www.lexology.com/library/detail.aspx?g=71725d27-2e84-4bd8-ba2a-8b6708458974)

### Government Initiatives
- [Australian Digital Health Agency: National Digital Health Strategy](https://www.digitalhealth.gov.au/national-digital-health-strategy)
- [ADHA: AI Transparency Statement](https://www.digitalhealth.gov.au/about-us/policies-privacy-and-reporting/artificial-intelligence-transparency-statement)
- [Department of Health: Health Technologies and Digital Health](https://www.health.gov.au/topics/health-technologies-and-digital-health/what-we-do)
- [AIHW: Digital Health in Australia](https://www.aihw.gov.au/reports/australias-health/digital-health)
- [Services Australia: Telehealth Services](https://www.servicesaustralia.gov.au/mbs-and-telehealth)
- [MBS Online: Telehealth Factsheets](https://www.mbsonline.gov.au/internet/mbsonline/publishing.nsf/Content/Factsheet-TempBB)

### International Comparisons
- [Mayo Clinic Proceedings: Global Harmonization of AI-SaMD Regulation](https://www.mcpdigitalhealth.org/article/S2949-7612(24)00124-X/fulltext)
- [PharmaLex: EU AI Act's Impact on Medical Devices](https://www.pharmalex.com/thought-leadership/blogs/what-global-ai-regulations-mean-for-medical-device-manufacturers/)
- [Taylor Wessing: Medical Devices and the EU AI Act](https://www.taylorwessing.com/en/interface/2024/ai-act-sector-focus/medical-devices-and-the-eu-ai-act-ai-act)
- [King & Spalding: EU AI Act and Medical Device Regulations](https://www.kslaw.com/news-and-insights/europe-navigating-the-interplay-between-eu-ai-act-and-medical-device-regulations-strategic-update-for-the-healthcare-sectors)
- [IntuitionLabs: AI Medical Devices 2025 Regulation](https://intuitionlabs.ai/articles/ai-medical-devices-regulation-2025)

---

*Last Updated: November 2025*
