# DeepScribe Oncology Specialization & Clinical AI Analysis

## Executive Summary

DeepScribe has established itself as the dominant ambient AI solution for oncology, with its technology now capturing 3.1 million cancer care visits annually—representing approximately 40% of all U.S. cancer visits. Founded in 2017 with oncologists specifically in mind, the company has developed a proprietary clinical LLM (HealAI) trained on over 3 million labeled medical conversations, purpose-built to handle the complex, longitudinal nature of cancer care documentation.

---

## 1. Oncology Focus

### Why Oncology Specialization

DeepScribe was founded with oncology as a core focus from inception. According to CEO Matthew Ko:

> "We started DeepScribe in 2017 with oncologists in mind, to help them bring humanity back to cancer care by taking on their most time-consuming administrative work."

**Strategic rationale for oncology focus:**
- **Complexity advantage**: Cancer care involves intricate, longitudinal workflows that generic AI solutions struggle to handle
- **Terminology depth**: Oncology requires understanding of specialized nomenclature, staging systems, and treatment protocols
- **Documentation burden**: Oncologists face particularly heavy documentation requirements due to complex treatment regimens
- **Value-based care alignment**: Cancer care increasingly involves risk-based contracts requiring detailed documentation

### 3.1 Million Oncology Visits Annually

As of November 2025, DeepScribe announced a major milestone:

| Metric | Value |
|--------|-------|
| Annual oncology visits captured | 3.1 million |
| Share of U.S. cancer visits | ~40% |
| Community oncologist coverage | 60% practice at DeepScribe-enabled organizations |
| Monthly volume growth | Doubled since August 2025; quadrupled since January 2025 |
| Daily active oncologists | ~1,000 |

**Growth trajectory:**
- Near-exponential growth in oncology documentation volume
- Adoption rates exceeding 95% in latest enterprise deployments
- 91% of providers rate platform as "easy to use"

### Oncology-Specific Features

**Cancer care workflow understanding:**
- Tailored to unique intricacies of cancer care
- Understands staging, treatment cycles, and progression monitoring
- Captures oncology-specific terminology, medication names, and care plan details
- Handles complex multi-system diagnoses common in oncology

**Structured note generation:**
- Automatically creates structured clinical notes optimized for oncology
- Organizes note plans with relevant ICD-10 diagnosis codes
- Captures HCC codes across multiple organ systems
- Differentiates between cancer and non-cancer diagnoses

**Oncology EHR integrations:**
- **Flatiron Health OncoEMR®**: First ambient AI solution partner; serves 4,200+ providers across 800+ locations
- **Ontada IKnowMed**: Direct data integration with oncology-specific EHR
- Custom workflows for oncology documentation requirements

### Longitudinal Care Handling

DeepScribe's platform is specifically designed for the longitudinal nature of cancer care:

**Multi-visit context intelligence:**
- Synthesizes information from disparate sources across patient journey
- Pulls key contextual information from previous visits
- Understands interval history based on current conversation
- Produces AI pre-charting summaries tailored to visit type

**Visit-type differentiation:**
- **New patient consult**: Full clinical narrative capturing cancer origin, staging evaluations, genetic/molecular analyses, previous therapies, multidisciplinary perspectives
- **Follow-up visits**: Focused on progression since last visit, relevant imaging, and labs
- **Treatment visits**: Captures regimen details, response assessments, side effect monitoring

---

## 2. Technology

### Proprietary LLM: HealAI

DeepScribe's core technology is HealAI, a purpose-built clinical large language model:

**Training data:**
- 3+ million labeled medical conversations
- Largest clinical dataset in the world for this application
- Healthcare-specific training beyond general LLM foundations

**Architecture & capabilities:**
- Specialty-specific training for oncology, cardiology, and other complex specialties
- Fine-tuned for complex workflows and provider preferences
- Configured to run hundreds of inferences live during visits
- Industry-leading note accuracy in clinical documentation

**Performance:**
- Surpassed GPT-4 in clinical documentation accuracy (per DeepScribe claims)
- 98.8 overall performance score from KLAS Research (2025)
- Three KLAS Top 5 positions in 2025 Emerging Solutions

### AWS Partnership

DeepScribe announced its strategic partnership with AWS in February 2024:

**Infrastructure:**
- Uses 30+ AWS services for machine learning, compute, and storage
- AWS SageMaker for secure training and hosting of HealAI
- Distributed GPUs via Amazon SageMaker for advanced training
- AWS HealthScribe (HIPAA-eligible) integrated for improved accuracy

**AWS Marketplace availability (April 2024):**
- Available through private offers
- Enables consolidated purchasing and billing
- Supports deeper integration with other AWS partners
- Allows maximization of AWS committed resources

**AWS endorsement** (Dr. Jared Saul, AWS Chief Medical Officer):
> "Reducing documentation burden is a prime example of how generative AI can be applied to positively impact clinician and patient experiences."

### "Ambient Operating System" Vision

DeepScribe positions itself not as a simple scribe but as an "Ambient Operating System" for clinical care:

**Core concept:**
- 100% ambient documentation (no dictation or wake words required)
- Real-time intelligence at point of care
- Beyond documentation to clinical insights and decision support

**Future roadmap (CEO Matthew Ko):**
> "The next frontier for DeepScribe is not just about documentation, but about transforming the clinical conversation into a rich source of insights."

**Planned capabilities:**
- Real-time trial matching
- Biomarker identification
- Treatment planning support
- Value-based care performance optimization

### Multi-Visit Context

**Context awareness architecture:**
- Incorporates relevant information from previous visits
- Creates comprehensive patient charts with historical context
- Tailors information relevance based on patient journey stage

**Data synthesis:**
- Structured EHR fields
- Unstructured PDFs (referrals, outside records)
- Labs and imaging results
- Prior visit summaries
- Clinical notes from multiple sources

---

## 3. Clinical Capabilities

### Pre-Visit: AI Pre-Charting

**Functionality:**
- Extracts and structures clinical details from EHR and outside sources
- Creates concise, contextual view tailored to clinician and patient needs
- Flags items requiring follow-up before visit
- Sharable with care team for preparation

**Data sources synthesized:**
- Referrals and outside records
- Clinical notes
- Labs and imaging
- Prior visit summaries
- Unstructured PDFs

**Visit-type optimization:**
- New patient consults: Comprehensive clinical narrative
- Follow-ups: Focused progression summaries
- Treatment visits: Regimen-specific preparation

### During-Visit: Real-Time Documentation

**DeepScribe Real-Time (launched March 2024 at HIMSS):**
- AI-generated clinical notes as visit unfolds
- Zero latency—instantaneous note generation
- Live feedback allows mid-visit corrections and clarifications
- No dictation or wake words required (100% ambient)

**Ambient capture:**
- Natural conversation flow preserved
- All clinically relevant details captured
- Oncology terminology automatically recognized
- Treatment discussions accurately documented

### Post-Visit: Note Completion & Coding

**Automated note generation:**
- Complete structured clinical note
- Auto-populates patient chart in EHR
- Clinician review and signoff workflow
- Significant reduction in after-hours documentation

**Time savings validated:**
- Texas Oncology pilot: 1.5 hours saved per provider per week
- Enables clinicians to leave work on time
- Reduces documentation burden and burnout

### Treatment Plan Documentation

**Cancer treatment capture:**
- Regimen details and modifications
- Response assessments
- Progression documentation
- Side effect monitoring
- Supportive care requirements

**Oncology-specific structuring:**
- Treatment cycle tracking
- Dose modifications
- Staging updates
- Tumor marker trends

### Clinical Trial Matching (Future)

**Planned capability:**
- Activating clinically structured datasets
- Real-time insights for trial eligibility
- Biomarker identification for trial matching
- Integration with research databases

**Strategic importance:**
> "Empower clinicians to deliver more personalized care, identify clinical trial opportunities and, ultimately, improve patient outcomes in a way that wasn't possible before."

### Coding for Oncology

**Automated code suggestions:**
- HCC (Hierarchical Condition Category) codes
- CPT (Current Procedural Terminology) codes
- ICD-10 diagnosis codes

**Texas Oncology pilot results:**
| Metric | Without DeepScribe | With DeepScribe |
|--------|-------------------|-----------------|
| Average billed diagnoses per patient | 3.0 | 4.1 |
| Non-cancer HCC code capture | Baseline | Significantly improved |
| Endocrine system codes | Lower | Higher |
| Cardiovascular system codes | Lower | Higher |

**Quality findings:**
- Cancer diagnosis codes: Manual coding slightly better
- Non-cancer HCC codes: DeepScribe significantly better
- Overall code completeness: Improved with AI

---

## 4. Customers

### Pearl Health Partnership (January 2025)

**Scope:**
- 3,500+ primary care providers
- Preferred ambient AI partner designation
- Focus on value-based care documentation

**Use case:**
- ACO REACH and risk-bearing model participants
- Point-of-care intelligence for proactive patient identification
- Complete clinical notes including details for accurate billing

**Strategic fit:**
- Pearl Health provides physician enablement and risk management
- DeepScribe enables time savings for patient care focus
- Combined solution optimizes value-based care performance

### New York Cancer & Blood Specialists (April 2025)

**Organization profile:**
- Premier oncology practice
- ASCO Quality Oncology Practice Initiative (QOPI®) certified
- 30+ locations across New York metro area
- 35 hospital affiliations
- Coverage: Nassau, Suffolk, Bronx, Manhattan, Queens, Staten Island, Brooklyn, Upstate NY

**Implementation:**
- DeepScribe Ambient Operating System for Oncology
- Direct integration with Flatiron Health OncoEMR®

**Leadership endorsement** (Dr. Jeff Vacirca, Oncologist and CEO):
> "Bringing our doctors automated documentation and intelligent insights means they can devote more quality time to our patients, and give them the personalized attention and care they deserve."

### Other Major Oncology Customers

**Large oncology networks:**
| Organization | Notes |
|--------------|-------|
| Texas Oncology | ~1,000 clinicians, 280+ locations, statewide coverage |
| Florida Cancer Specialists & Research Institute | Major community oncology practice |
| U.S. Oncology Network (USON) | Largest community oncology network |
| American Oncology Network (AON) | National oncology partnership |
| OneOncology | Major oncology management company |
| OnCare | Oncology practice network |
| Sarah Cannon Research Institute (SCRI) | Leading cancer research organization |
| CARTI | Arkansas cancer center |

**Texas Oncology collaboration details:**
- Pilot: November 2023–April 2024
- 49 physicians participated
- Full rollout: All locations by fall 2024
- Results presented at 2024 ASCO Quality Care Symposium

### Health System Oncology Departments

**Ochsner Health (July 2024):**
- Enterprise-wide agreement
- Leading nonprofit healthcare provider in Gulf South
- 4,700 clinicians gaining access
- 75% clinician adoption during initial launch
- Multi-specialty deployment including oncology

**Key metrics across deployments:**
- 95%+ adoption rates in enterprise deployments
- 91% rate platform as easy to use
- 80%+ adoption within large oncology groups
- 81% average satisfaction score (Texas Oncology pilot)

---

## 5. Expansion Strategy

### Beyond Oncology: Specialty Expansion

**Current specialty coverage:**
- **Primary**: Oncology (core focus)
- **Expanding**: Cardiology, urology, orthopedics, neurology
- **Broad**: Primary care and chronic disease management

**CardioOne Partnership (October 2024):**
- Cardiology-specific ambient AI
- Initial rollout: Cardiovascular Specialists of New England
- 100% adoption achieved
- ~75% of patient visits use DeepScribe

**Specialty-specific approach:**
- Terminology understanding per specialty
- Workflow-specific templates
- Fine-tuned AI models for each specialty
- Custom integrations with specialty EHRs

### Value-Based Care Focus

**Strategic positioning:**
- Strong support for value-based care initiatives
- Pearl Health partnership validates VBC commitment
- HCC code capture critical for risk adjustment

**Ambient OS for value-based care:**
- Parse subtle indicators in real-time (adherence challenges, SDOH)
- Real-time prompts for follow-up labs or care manager referrals
- Earlier intervention with greater precision
- Reduce avoidable hospitalizations
- Elevate quality scores

**Supported programs:**
- ACO REACH
- Risk-bearing models
- Medicare Advantage HCC coding
- Quality measure documentation

### AWS Marketplace Strategy

**Go-to-market advantages:**
- Streamlined procurement for health systems
- Consolidated billing with AWS services
- Integration with AWS healthcare ecosystem
- Leverage existing AWS committed spend

**Enterprise positioning:**
- Private offer model for health systems
- IT-friendly deployment and compliance
- HIPAA-eligible infrastructure
- Scalable across large organizations

**Market reach:**
- 1,500+ healthcare organizations deployed
- Enterprise-wide agreements (e.g., Ochsner Health)
- Community oncology network coverage

---

## 6. Competitive Positioning

### Market Leadership Claims

**KLAS Research recognition (2025):**
- 98.8 overall performance score
- Top 5: Improve Outcomes
- Top 5: Improve Clinician Experience
- Top 5: Improve Patient Experience

**Oncology dominance:**
- 60% of community oncologists at DeepScribe-enabled organizations
- 40% of all U.S. cancer visits
- First ambient AI partner for Flatiron Health
- Leading platform for oncology-specific EHRs

### Differentiation Factors

| Factor | DeepScribe Approach |
|--------|---------------------|
| Specialty focus | Purpose-built for complex specialties (vs. general-purpose) |
| LLM | Proprietary HealAI trained on 3M+ clinical conversations |
| Ambient capture | 100% ambient (no dictation/wake words) |
| Longitudinal care | Multi-visit context and pre-charting |
| Real-time | Notes generated during visit (not after) |
| Oncology EHRs | Native integrations with OncoEMR, IKnowMed |
| Adoption | 95%+ in enterprise; 91% ease of use rating |

---

## Sources

### Primary Sources
- [DeepScribe Oncology Momentum (November 2025)](https://www.prnewswire.com/news-releases/deepscribes-oncology-momentum-accelerates-ambient-ai-set-to-capture-3-1-million-cancer-care-visits-annually-302610937.html)
- [DeepScribe Solidifies Ambient AI Leadership (September 2025)](https://www.prnewswire.com/news-releases/deepscribe-solidifies-ambient-ai-leadership-in-oncology-with-new-study-and-accelerated-growth-302557045.html)
- [DeepScribe and Flatiron Health Partnership (January 2025)](https://www.prnewswire.com/news-releases/deepscribe-and-flatiron-health-announce-partnership-to-bring-oncology-specific-ambient-ai-to-flatirons-4-200-providers-302356795.html)
- [DeepScribe and Pearl Health Partnership (January 2025)](https://www.prnewswire.com/news-releases/deepscribe-and-pearl-health-announce-partnership-to-bring-ambient-ai-documentation-to-value-based-care-providers-302348410.html)
- [NY Cancer & Blood Specialists Adoption (April 2025)](https://www.prnewswire.com/news-releases/new-york-cancer--blood-specialists-adopt-the-deepscribe-ambient-operating-system-for-oncology-302433548.html)
- [Texas Oncology Collaboration (June 2024)](https://www.prnewswire.com/news-releases/deepscribe-collaborates-with-texas-oncology-to-provide-ai-solution-for-complex-patient-documentation-302167533.html)
- [DeepScribe and AWS Partnership (February 2024)](https://www.prnewswire.com/news-releases/deepscribe-and-aws-to-scale-generative-ai-in-healthcare-302070488.html)
- [DeepScribe on AWS Marketplace (April 2024)](https://www.prnewswire.com/news-releases/deepscribes-ambient-ai-for-clinical-documentation-now-available-on-the-aws-marketplace-302114672.html)
- [Ochsner Health Selection (July 2024)](https://www.prnewswire.com/news-releases/ochsner-health-selects-deepscribe-to-bring-ambient-ai-to-their-4-700-clinicians-302209853.html)
- [CardioOne Partnership (October 2024)](https://www.prnewswire.com/news-releases/cardioone-partners-with-deepscribe-to-bring-cardiology-specific-ambient-ai-to-practices-302275931.html)
- [DeepScribe Real-Time at HIMSS (March 2024)](https://www.prnewswire.com/news-releases/deepscribe-unveils-real-time-feature-at-himss-ai-generated-clinical-notes-as-the-visit-unfolds-302086744.html)

### Research & Academic
- [ASCO JCO Oncology Practice: Texas Oncology Pilot Study](https://ascopubs.org/doi/10.1200/OP.2024.20.10_suppl.418)
- [HealAI Paper: ACM WSDM 2024](https://dl.acm.org/doi/10.1145/3616855.3635739)

### Company Resources
- [DeepScribe Oncology Page](https://www.deepscribe.ai/oncology)
- [DeepScribe Pre-Charting](https://www.deepscribe.ai/pre-charting)
- [DeepScribe Customer Stories](https://www.deepscribe.ai/categories/customers)
- [AWS Marketplace Listing](https://aws.amazon.com/marketplace/pp/prodview-dbzumpxmtnqvu)

### Industry Coverage
- [AJMC: Flatiron-DeepScribe Partnership](https://www.ajmc.com/view/flatiron-health-deepscribe-unveil-partnership-to-provide-oncology-specific-ambient-ai)
- [MobiHealthNews: Flatiron Partnership](https://www.mobihealthnews.com/news/deepscribe-partners-flatiron-health-oncology-focused-ambient-ai)
- [HIT Consultant: Real-Time Feature](https://hitconsultant.net/2024/03/12/deepscribe-unveils-real-time-ai-generated-clinical-notes/)

---

*Analysis compiled: November 2025*
*Research focus: DeepScribe oncology specialization and clinical AI approach*
