# DeepScribe Healthcare AI - Comprehensive Vendor Analysis

*Research Date: November 2025*

---

## Executive Summary

DeepScribe is a healthcare AI company specializing in ambient clinical documentation, with a strong focus on oncology. The company has achieved notable recognition with a **98.8 KLAS Research score** (highest in the ambient AI category) and is positioning itself as an "Ambient Operating System" provider rather than just a documentation tool. DeepScribe differentiates through its proprietary HealAI LLM, which outperforms GPT-4 by 59% in clinical accuracy benchmarks.

---

## 1. Company Profile

### Founding & Leadership
| Attribute | Details |
|-----------|---------|
| **Founded** | 2017 |
| **Headquarters** | San Francisco, CA |
| **Founders** | Akilesh Bapu (CEO), Matthew Ko (Co-Founder), Kairui Zeng |
| **Chief Medical Officer** | Dr. Dean Dalili (appointed May 2024) |

### Funding History

| Round | Date | Amount | Lead Investor | Valuation |
|-------|------|--------|---------------|-----------|
| Seed/Early | 2017-2021 | ~$7M | Various | - |
| Series A | 2022 | $30M | Index Ventures | $180M (WSJ reported) |
| Series B | January 2024 | $30M | Index Ventures | - |
| **Total Raised** | - | **~$60M** | - | - |

**Notable Investors:** Index Ventures, 1984 Ventures, Bee Partners, Stage 2 Capital, Dylan Field (Figma CEO), Alex Wang (Scale AI CEO)

---

## 2. Product Offerings & Features

### Core Platform: Ambient Operating System

DeepScribe positions its platform as an "Ambient Operating System" - not just documentation, but an ecosystem of intelligent applications and automated workflows powered by ambient AI patient data.

#### Key Capabilities

| Feature | Description |
|---------|-------------|
| **Ambient AI Scribe** | Real-time transcription and documentation during patient visits |
| **Pre-Visit Intelligence** | AI pre-charting summaries synthesizing information from multiple sources |
| **During-Visit Documentation** | Live processing with "Real-Time" feature (launched HIMSS 2024) |
| **Post-Visit Automation** | Complete note generation within seconds of visit completion |
| **Customization Studio** | Build custom models for specialty/organizational needs |
| **ICD-10 Coding** | Automated diagnosis coding assistance |
| **HCC Coding** | Hierarchical Condition Category capture for risk adjustment |
| **E/M Coding** | Automated Evaluation & Management level suggestions (launched March 2025) |

#### Real-Time Documentation
Unlike conventional methods that process notes post-visit, DeepScribe's HealAI operates live during consultations, conducting hundreds of inferences while maintaining note accuracy. "Real-Time represents the biggest breakthrough in ambient clinical documentation since large language models." - Akilesh Bapu, CEO

### Product Adoption Metrics
- **100% adoption** for ambient AI scribe, automated ICD-10 coding, and Customization Studio (per KLAS)
- Platform deployed in **1,500+ healthcare organizations**
- **3.1 million** oncology visits captured annually (as of November 2025)

---

## 3. Oncology Specialization

DeepScribe has established itself as the **leading ambient AI solution for oncology**, with significant market penetration and specialty-specific capabilities.

### Oncology Market Position
| Metric | Value |
|--------|-------|
| Community oncologists using DeepScribe | **60%** practice at organizations using DeepScribe |
| Annual oncology visits captured | **3.1 million** (projected) |
| Monthly volume growth | **4x since January 2025**, 2x since August 2025 |

### Why Oncology Focus?
- Cancer care involves complex, longitudinal documentation requirements
- Multiple treatment modalities and evolving care plans
- Documentation is a major cause of oncologist burnout
- Complex coding requirements (ICD-10 oncology codes, treatment regimens)

### Oncology-Specific Features
- Understanding of complex, longitudinal oncology workflows
- Clinical trial recruitment acceleration and patient matching
- Information synthesis from disparate sources across care continuum
- Cancer-specific terminology and treatment documentation
- QOPI (Quality Oncology Practice Initiative) compliance support

### Key Oncology Partnerships

| Organization | Details | Date |
|-------------|---------|------|
| **Flatiron Health** | First ambient AI partner for OncoEMR; 4,200+ providers, 800+ locations | January 2025 |
| **Texas Oncology** | ~1,000 clinicians across 280+ locations | June 2024 |
| **New York Cancer & Blood Specialists** | QOPI-certified oncology practice | April 2025 |
| **CARTI Cancer Center** | 18 locations in Arkansas | April 2025 |
| **U.S. Oncology Network (USON)** | Network partner | 2024-2025 |
| **American Oncology Network (AON)** | Network partner | 2024-2025 |
| **OneOncology** | Network partner | 2024-2025 |
| **Sarah Cannon Research Institute (SCRI)** | Research partner | 2024-2025 |

---

## 4. Technology Stack

### Proprietary LLM: HealAI

DeepScribe developed **HealAI**, a purpose-built clinical large language model that is central to their differentiation strategy.

#### Training Data & Development
| Aspect | Details |
|--------|---------|
| Training conversations | **4+ million** de-identified patient conversations |
| Labeled data | **3+ million** conversations processed and labeled with AWS |
| Base architecture | LLaMA2-based 13B parameter model (HEAL) |
| Development | Continued pre-training + healthcare-specific fine-tuning |

#### Performance Benchmarks

| Benchmark | HealAI/DeepScribe | GPT-4 | Result |
|-----------|-------------------|-------|--------|
| Clinical Documentation Accuracy | - | - | **DeepScribe 59% more accurate** |
| PubMedQA | 78.4% | Lower | Outperforms |
| Medical Concept Identification | Superior | - | Surpasses GPT-4 and Med-PaLM 2 |
| Medical Note Generation | Parity | - | Equivalent quality |

#### Why HealAI Outperforms General LLMs
- Domain-specific training on largest clinical conversation dataset
- Healthcare-specific fine-tuning prevents hallucinations
- Specialty-customized models for different practice types
- Reduced biases through targeted training
- Enhanced note-writing style matching clinical expectations

### AWS Partnership (February 2024)

DeepScribe announced a strategic collaboration with AWS to scale generative AI in healthcare:

| Component | Description |
|-----------|-------------|
| **Amazon SageMaker** | Distributed GPU training for HealAI |
| **AWS HealthScribe** | HIPAA-eligible service integration via Amazon Bedrock |
| **AWS Marketplace** | DeepScribe available to AWS health system partners |
| **Data Processing** | 3M+ conversations processed and labeled on AWS |

> "Reducing documentation burden is a prime example of how generative AI can be applied to positively impact clinician and patient experiences. We're excited to be supporting DeepScribe's work in scaling adoption of clinical AI and purpose-built LLMs." - Jared Saul, Chief Medical Officer, AWS

### Security & Compliance
- **HIPAA compliant** (100%)
- **AES-256 encryption** (end-to-end)
- **HL7 compliant**
- **FHIR compliant**
- Trust & Safety initiatives for responsible AI deployment

---

## 5. EHR Integrations

### Epic Integration (Deepened January 2024)

DeepScribe has invested significantly in Epic integration, making it a strong option for Epic shops:

| Feature | Capability |
|---------|------------|
| **SmartData Integration** | Direct push to Epic's SmartData elements |
| **Customization Studio Sync** | Preferences mirror in Epic within seconds via API |
| **Visit Type Templating** | Notes configured based on Epic schedule visit types |
| **Epic Connection Hub** | Available and certified |
| **Platforms** | Workstation, browser, and mobile |
| **Discrete Field Population** | Personalized documentation directly into chart fields |
| **Partnership Start** | 2022 |

**Customer Result:** Covenant HealthCare reduced after-hours documentation by **75%** with Epic integration.

### Supported EHR Systems

| EHR | Integration Type |
|-----|-----------------|
| Epic | Deep integration, SmartData, Connection Hub |
| Oracle Cerner | Direct pipeline |
| athenahealth | Direct pipeline |
| Flatiron OncoEMR | First ambient AI partner |
| Other specialty platforms | Bi-directional sync |

### AWS Marketplace Availability
DeepScribe is available on the **AWS Marketplace**, providing simplified procurement for AWS health system partners and standardized deployment options.

---

## 6. Pricing Information

DeepScribe uses **custom, quote-based pricing** rather than transparent published rates.

### Estimated Pricing

| Metric | Estimate |
|--------|----------|
| Starting Price | ~$8,000/year |
| Pricing Model | Annual, quote-based |
| EHR Integration Add-on | ~$100/month per provider |

### Factors Affecting Price
- Practice/organization size
- Medical specialty complexity
- Required EHR integration depth
- Custom template and specialty field requirements
- Contract length (annual deals may reduce monthly cost ~20%)
- Enterprise setup fees for large hospital systems

### Subscription Options
- Monthly or annual subscriptions available
- Flexible scaling based on number of users
- Group discounts for large practices

*Note: Contact DeepScribe directly for accurate, current pricing.*

---

## 7. KLAS Research Performance

### Overall Scores

| Metric | Score | Context |
|--------|-------|---------|
| **KLAS Spotlight Score** | **98.8/100** | January 2025 report |
| **Overall Score (2024-2025)** | **98.9** | KLAS system rating |
| **Category Comparison** | +5.5 points | Above average 2024 Best in KLAS Ambient Speech vendor |

### KLAS Grades (All A+)

DeepScribe received **15 grades of A+** across six categories:
1. **Product** - A+
2. **Value** - A+
3. **Operations** - A+
4. **Relationship** - A+
5. **Loyalty** - A+
6. **Culture** - A+

### 2025 KLAS Emerging Solutions Top 20 Awards (October 2025)

DeepScribe earned **Top 5 placements** in three "Quadruple Aim" categories:
- **Improving Outcomes** - Top 5
- **Improving Patient Experience** - Top 5
- **Improving Clinician Experience** - Top 5

*Awards announced at HLTH USA 2025 Conference, Las Vegas*

### Customer Feedback Highlights (KLAS)
> "DeepScribe clients cited significantly improved physician experience as well as responsiveness from the vendor as factors that drove their extremely high satisfaction overall." - Mac Boyter, Research Director, Documentation Solutions, KLAS Research

### Differentiators Noted by KLAS Evaluators
- Greater emphasis on coding assistance
- Individual user customization capabilities
- Specialty-specific workflow adaptation

### Competitor Comparison

| Vendor | KLAS Score |
|--------|------------|
| **DeepScribe** | **98.8** |
| Commure (formerly Augmedix) | 93.3 |

---

## 8. Customer Case Studies

### Ochsner Health (July 2024)

**Scope:** Enterprise-wide agreement for 46-hospital system

| Metric | Result |
|--------|--------|
| Clinicians | 4,700 employed and affiliated physicians |
| Patient Satisfaction | 96% (likely to recommend provider) |
| Clinician Adoption | 75% during initial launch |
| Time Savings | 2-3 hours/day reduced to 3-4 minutes/note |

> "Before using DeepScribe, I spent at least two to three hours a day preparing for visits and then going back and editing notes based on patient conversations. Now, I have been able to streamline that into three to four minutes per note." - Dr. Terrance Wickman, Ochsner Nephrologist

**Why Ochsner Chose DeepScribe:**
- Customization capabilities
- Deep Epic integration
- Specialty-specific workflows
- Ability to accommodate physician preferences while aligning with system requirements

### Texas Oncology (June 2024)

| Metric | Details |
|--------|---------|
| Clinicians | ~1,000 |
| Locations | 280+ across Texas |
| Use Case | Complex oncology documentation, coding automation |

> "Documentation is one of the major causes of burnout, specifically with oncologists, as cancer care has become increasingly more complex. I thought 'there's got to be a better way.'" - Dr. Gury K. Doshi, Medical Director, Texas Oncology

### Covenant HealthCare

| Metric | Result |
|--------|--------|
| After-Hours Documentation Reduction | **75%** |
| Integration | Epic SmartData |

> "DeepScribe brings tremendous potential to our health system. It's empowering us to alleviate the documentation burden, deliver exceptional patient care, and make good on our commitment to prioritize clinician well-being."

### Pearl Health (January 2025)

| Metric | Details |
|--------|---------|
| Providers | 3,500+ primary care providers |
| Focus | Value-based care, ACO REACH, risk-bearing models |
| Status | DeepScribe named preferred ambient AI partner |

### Additional Customers
- CardioOne (cardiology-specific, October 2024)
- Commons Clinic (patient experience focus, August 2024)
- Rockville Internal Medicine Group
- New York Cancer & Blood Specialists
- CARTI Cancer Center

---

## 9. "Ambient Operating System" Vision

### Strategic Direction

DeepScribe's CEO Matthew Ko articulates the company's vision beyond documentation:

> "If we think about ambient documentation as the technology on-ramp, the real highway is what I like to call the ambient operating system. Once conversations are consistently recorded and transformed into actionable data, you unlock an entire ecosystem of intelligent applications and 'agentic' workflows that can reshape care delivery."

### Current Ambient Operating System Components

| Component | Status |
|-----------|--------|
| Ambient Documentation | GA |
| ICD-10 Coding | GA |
| HCC Coding | GA |
| E/M Coding | GA (March 2025) |
| Pre-Visit Intelligence | GA |
| Customization Studio | GA |

### Future Vision: Agentic Workflows

The Ambient Operating System roadmap includes:
- **Automated care orchestration** - Moving beyond documentation to workflow automation
- **Real-time alerts and analyses** - Clinical and administrative decision augmentation
- **Clinical trial recruitment** - Accelerating patient matching to therapies (oncology focus)
- **Specialty-specific applications** - Different manifestations for different use cases

### Key Enabler: High Clinician Adoption
> "The leap from note documentation to an operating system capable of automated care orchestration might appear substantial, but the bridge is high clinician adoption. Without it, the system's most transformative capabilities remain locked away."

---

## 10. 2025-2026 Roadmap & Recent Developments

### 2025 Milestones Achieved

| Date | Development |
|------|-------------|
| January 2025 | Flatiron Health partnership announced |
| January 2025 | Pearl Health partnership announced |
| January 2025 | 98.8 KLAS Spotlight Score published |
| March 2025 | Automated E/M Coding launched |
| March 2025 | "Real-Time" feature expanded |
| April 2025 | NYCBS and CARTI deployments |
| October 2025 | KLAS Emerging Solutions Top 20 (3 awards) |
| November 2025 | 3.1M annual oncology visits milestone |

### Growth Trajectory
- Monthly oncology volume **doubled** since August 2025
- Monthly oncology volume **quadrupled** since January 2025
- 60% of community oncologists now at organizations using DeepScribe

### 2026 Outlook (Inferred)

Based on company statements and market positioning:
- Continued oncology market expansion
- Deeper Ambient Operating System capabilities
- Enhanced agentic workflow features
- Potential additional specialty expansions
- Further EHR integration depth

*Note: Specific 2026 roadmap details not publicly disclosed as of research date.*

---

## 11. Competitive Positioning

### Strengths

| Strength | Evidence |
|----------|----------|
| **Highest KLAS Score** | 98.8 vs. 93.3 for nearest competitor |
| **Oncology Leadership** | 60% community oncologist market coverage |
| **Proprietary AI** | HealAI outperforms GPT-4 by 59% |
| **Deep Epic Integration** | SmartData, Connection Hub, Customization Studio sync |
| **Coding Intelligence** | ICD-10, HCC, E/M all automated |
| **Platform Vision** | Ambient Operating System beyond documentation |
| **AWS Partnership** | Infrastructure and marketplace access |

### Potential Limitations

| Factor | Consideration |
|--------|---------------|
| **Funding** | $60M total vs. Abridge's $800M+ |
| **Valuation** | ~$180M (2022) vs. Abridge's $5.3B |
| **Market Share** | Niche/specialty vs. broad market leaders |
| **Global Presence** | US-focused (no EU/APAC presence noted) |
| **Pricing Transparency** | Quote-based, no public pricing |
| **EHR Breadth** | Strong Epic, but less multi-EHR than Nabla |

### Market Position vs. Competitors

| Factor | DeepScribe | Nuance | Abridge | Nabla |
|--------|------------|--------|---------|-------|
| KLAS Score | 98.8 | - | Best in KLAS | - |
| Funding | $60M | Microsoft-backed | $800M+ | $120M |
| Specialty Focus | Oncology leader | Broad | Broad | Broad |
| Proprietary LLM | HealAI | Yes | Yes | Yes |
| Global | US only | Yes | US | EU + US |
| Beyond Ambient | Coding, OS vision | Coding, CDS, Nursing | Revenue cycle, Prior auth | Coding, Agentic |

---

## 12. Sources

### Primary Sources
- [DeepScribe 98.8 KLAS Score Announcement](https://www.prnewswire.com/news-releases/deepscribe-receives-98-8-overall-performance-score-in-klas-research-report-with-top-grades-in-every-category-302344580.html)
- [KLAS Research - DeepScribe Ambient AI 2025 Report](https://klasresearch.com/report/deepscribe-ambient-ai-2025-enhancing-clinician-experience-and-efficiency-through-ambient-speech-ai/3402)
- [DeepScribe KLAS Emerging Solutions Top 20 Awards](https://www.prnewswire.com/news-releases/deepscribe-wins-three-awards-at-2025-klas-emerging-solutions-top-20-event-302589514.html)

### Company & Funding
- [Crunchbase - DeepScribe Profile](https://www.crunchbase.com/organization/deepscribe)
- [DeepScribe Series B Funding](https://menahunt.com/event/2285-deepscribe-secures-30m-series-b-to-combat-physician-burnout-with-aipowered-medical-scribing)
- [PitchBook - DeepScribe Profile](https://pitchbook.com/profiles/company/264826-18)

### AWS Partnership
- [DeepScribe and AWS Partnership Announcement](https://www.prnewswire.com/news-releases/deepscribe-and-aws-to-scale-generative-ai-in-healthcare-302070488.html)
- [AWS Marketplace - DeepScribe](https://aws.amazon.com/marketplace/pp/prodview-dbzumpxmtnqvu)
- [HIT Consultant - DeepScribe AWS Partnership](https://hitconsultant.net/2024/02/26/deepscribe-and-aws-partner-to-advance-ai-powered-medical-documentation/)

### Oncology
- [DeepScribe Oncology Momentum - 3.1M Visits](https://www.prnewswire.com/news-releases/deepscribes-oncology-momentum-accelerates-ambient-ai-set-to-capture-3-1-million-cancer-care-visits-annually-302610937.html)
- [DeepScribe Oncology Leadership Study](https://www.prnewswire.com/news-releases/deepscribe-solidifies-ambient-ai-leadership-in-oncology-with-new-study-and-accelerated-growth-302557045.html)
- [Flatiron Health Partnership](https://www.prnewswire.com/news-releases/deepscribe-and-flatiron-health-announce-partnership-to-bring-oncology-specific-ambient-ai-to-flatirons-4-200-providers-302356795.html)
- [Texas Oncology Collaboration](https://www.deepscribe.ai/resources/deepscribe-collaborates-with-texas-oncology-to-provide-ai-solution-for-complex-patient-documentation)
- [NYCBS Deployment](https://www.prnewswire.com/news-releases/new-york-cancer--blood-specialists-adopt-the-deepscribe-ambient-operating-system-for-oncology-302433548.html)
- [CARTI Cancer Center](https://www.prnewswire.com/news-releases/carti-cancer-center-deploys-deepscribes-ambient-operating-system-for-oncology-302426878.html)

### Technology
- [DeepScribe Outperforms GPT-4 by 59%](https://www.deepscribe.ai/resources/deepscribe-outperforms-gpt-4-by-59-percent-on-ai-medical-scribing)
- [HealAI Research Paper (ACM)](https://dl.acm.org/doi/10.1145/3616855.3635739)
- [HEAL LLM arXiv Paper](https://arxiv.org/html/2403.09057)
- [DeepScribe Real-Time Feature](https://www.prnewswire.com/news-releases/deepscribe-unveils-real-time-feature-at-himss-ai-generated-clinical-notes-as-the-visit-unfolds-302086744.html)

### Customers & Case Studies
- [Ochsner Health Partnership](https://www.deepscribe.ai/resources/ochsner-health-selects-deepscribe-to-bring-ambient-ai-to-their-4-700-clinicians)
- [Fierce Healthcare - Ochsner DeepScribe](https://www.fiercehealthcare.com/ai-and-machine-learning/ochsner-health-going-all-ambient-ai-clinical-tech-taps-deepscribe-4700)
- [Pearl Health Partnership](https://www.prnewswire.com/news-releases/deepscribe-and-pearl-health-announce-partnership-to-bring-ambient-ai-documentation-to-value-based-care-providers-302348410.html)

### EHR Integration
- [DeepScribe Epic Integration](https://www.prnewswire.com/news-releases/deepscribe-deepens-integration-with-epic-laying-groundwork-for-future-ambient-solutions-302032062.html)
- [HIT Consultant - Epic Integration](https://hitconsultant.net/2024/01/11/epic-ehr-integrates-with-deepscribes-ai-scribe-to-reduce-after-hours-work-by-75/)

### Ambient Operating System
- [E/M Coding Launch](https://www.prnewswire.com/news-releases/deepscribe-unveils-automated-em-coding-the-latest-ai-addition-to-its-ambient-operating-system-302389112.html)
- [Ambient AI 2025 Vision](https://www.deepscribe.ai/resources/ambient-ai-in-healthcare-2025-from-commoditization-to-transformation)

### Pricing
- [Healos - DeepScribe Pricing Analysis](https://www.healos.ai/blog/deepscribe-pricing-features-cost-and-the-best-alternatives-in-2025)
- [TrustRadius - DeepScribe Pricing](https://www.trustradius.com/products/deepscribe/pricing)

---

*Research compiled November 2025*
