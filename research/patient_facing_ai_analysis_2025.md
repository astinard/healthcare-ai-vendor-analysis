# Patient-Facing AI Outputs from Clinical Documentation
## 2025 Market Analysis

*Research Date: November 2025*

---

## Executive Summary

Patient-facing AI has evolved from a nascent capability to a core differentiator in clinical documentation platforms. In 2025, major vendors are competing not just on clinician efficiency but on patient engagement, health literacy, and multilingual accessibility. This analysis examines six key domains: after-visit summaries, patient education, patient messaging, referral communications, patient portals, and international considerations.

---

## 1. After-Visit Summaries

### Market Status

AI-generated after-visit summaries (AVS) have become standard across major ambient documentation platforms. These summaries transform clinician-patient conversations into patient-friendly documents that explain diagnoses, treatment plans, and follow-up steps.

### Vendor Capabilities

| Vendor | AVS Capability | Key Features |
|--------|---------------|--------------|
| **Nuance Dragon Copilot** | ✅ Generally Available | One-click generation from clinical notes; patient-friendly language conversion; integrated with Epic |
| **Abridge** | ✅ Generally Available | Contextual AI summaries for patients, families, caregivers; 28+ languages; part of core platform |
| **Ambience Healthcare** | ✅ Generally Available | "Patient Instructions" feature; customized to patient's medical knowledge level; deployed at Cleveland Clinic |
| **Suki AI** | ✅ Generally Available | Auto-generated patient instructions from ambient visits; multi-language support |
| **Epic (Native)** | 🔄 In Development | Part of "Emmie" patient AI assistant; expected November 2025 rollout |

### Language Simplification Approaches

**Reading Level Adaptation:**
- Ambience explicitly writes summaries "to the patient's level of medical knowledge"
- Vital's Doctor-to-Patient Translator transforms complex health record data into "easy-to-use, personalized interfaces"
- Google Translate and GPT-4 studies show 83-97.8% accuracy when translating medical text from English

**Challenges:**
- JMIR research (2025) found AI-generated plain language responses often remain at higher reading levels than recommended for general public
- Oversimplification can omit important clinical details
- Patient satisfaction (84-96.6%) exceeds clinician satisfaction (53.8-86.7%) with AI translations

### Multi-Language Translation

| Vendor | Languages Supported | Translation Method |
|--------|--------------------|--------------------|
| Abridge | 28+ | Native multi-language ambient AI |
| Nabla | 35+ | Proprietary LLM + fine-tuned Whisper |
| Suki | Multi-language (unspecified) | Conversation in any language → note in English |
| HealOs.ai/ScribeHealth | 150+ | Including Spanish, Chinese, Hindi, Russian, Tagalog, Vietnamese, Arabic |
| DeepScribe | Multi-language | EHR integration supports portal in patient's native language |

### Evidence Base

- **Mayo Clinic**: AI-drafted patient communications rated "more empathetic" than manually written versions
- **Patient Satisfaction**: 97% of patients reported physicians using DAX Copilot were "more focused, personable, and engaged"
- **Comprehension**: Studies show patients receiving visual education materials demonstrate 40% better medication adherence vs. text-only

---

## 2. Patient Education

### AI-Generated Educational Content

**Current Capabilities:**

| Type | AI Application | Vendor Examples |
|------|---------------|-----------------|
| **Condition-Specific** | Personalized explanations based on diagnosis | Oracle Patient Portal (2026), Epic Emmie |
| **Medication Instructions** | Dosing, interactions, side effects | Suki (staging orders), Chatbots in portals |
| **Procedure Prep** | Pre-procedure instructions, what to expect | Klara, Chat Data integrations |
| **Recovery Guidance** | Post-procedure care, warning signs | Ambience Patient Instructions, Vital |

### Conversational AI for Education

**John Snow Labs Research (2025):**
> "Conversational agents provide patients with accessible, interactive, and personalized information outside traditional clinical visits... offering continuous engagement, real-time support, and scalable education across diverse populations."

**Key Features:**
- 24/7 availability for patient questions
- Natural language processing for complex medical queries
- Personalization based on individual health data
- Integration with EHR for context-aware responses

### Medication Adherence Support

**Frontiers in Digital Health (2025):**
- Chatbots integrated into patient portals can guide medication instructions
- AI predicts patient adherence patterns based on clinical data
- Personalized treatment regimen recommendations
- Real-time adverse drug interaction warnings

**Iris Health AI** - AI-generated educational videos:
- Personalized avatar demonstrations (e.g., post-surgical movements)
- Evidence-based, provider-approved materials
- Potential to become "standard care"

### Personalization Approaches

| Personalization Type | Description | Implementation |
|---------------------|-------------|----------------|
| **Medical Knowledge Level** | Adjust complexity based on health literacy | Ambience, Vital |
| **Condition-Specific** | Tailored to diagnosis/treatment | All major vendors |
| **Language Preference** | Native language content | Abridge, Nabla, Suki |
| **Communication Style** | Adapt to patient preferences | Oracle Patient Portal (planned) |
| **Historical Context** | Reference past visits/results | Epic Emmie, Oracle |

---

## 3. Patient Messaging

### AI-Assisted Inbox Management

Patient message volumes have exploded—Johns Hopkins reports nearly **3X increase** from pre-COVID 2019 levels. AI is now essential for managing this burden.

### Epic In-Basket Solutions

**Epic ART (Augmented Response Technology):**
- Pre-drafts responses based on patient query + chart data
- Clinicians review, edit, and send
- **150+ organizations** using the technology
- Generates **1M+ drafts monthly**
- AI trained to adopt individual clinician's communication style

**Providence Provaria:**
- AI automatically categorizes MyChart messages
- Tags messages like ED triage for urgent prioritization
- **Results in 10 months:**
  - 300,000 messages screened across 264 clinics
  - **57% fewer messages** reaching doctors
  - **50% reduction** in patient response time

### Response Drafting Capabilities

| Health System | AI Tool | Results |
|--------------|---------|---------|
| **Mayo Clinic** | Epic GenAI drafts | Saves ~30 seconds per message; more empathetic responses |
| **Johns Hopkins** | LLM-based drafting | Clinicians can start with AI draft or blank message |
| **NYU Langone** | AI prioritization | High-acuity predictions deployed via Epic Nebula cloud |
| **Providence** | Provaria | AI categorization, routing, quick actions |

### Triage Automation

**NYU Langone Implementation:**
- AI system automatically prioritizes messages expected to warrant urgent response
- Detects acute problems: chest pain, difficulty breathing, confusion, altered mental status, syncopal episodes
- Deployed using Epic's Nebula cloud platform

**Future Capabilities (Epic 2025+):**
- GenAI will pull test results, medications, and other details needed when responding
- "Emmie" digital concierge will appear in MyChart
- Patients can ask Emmie questions including about test results

### Vendor Comparison: Patient Messaging

| Vendor | Inbox AI | Response Drafting | Triage | Integration |
|--------|----------|------------------|--------|-------------|
| **Epic (native)** | ✅ ART | ✅ LLM drafts | ✅ Prioritization | Native |
| **Nuance Dragon Copilot** | ❌ | 🔄 Indirect (via notes) | ❌ | Epic embedded |
| **Abridge** | ❌ | ❌ | ❌ | Epic "First Pal" |
| **Klara** | ✅ Automation | ✅ | ✅ | Multiple EHRs |

---

## 4. Referral Communications

### AI-Generated Referral Letters

**Status:** Referral letter generation is a key differentiator among ambient AI vendors.

### Nuance Dragon Copilot (Market Leader)

**Capabilities:**
- Automatically generates referral letters from encounter conversations
- Extracts medical history, requested services, test/imaging results
- One-click generation within EHR workflow
- Part of unified Dragon Copilot platform (March 2025)

**Availability:**
- US, Canada, UK: Generally Available
- Austria, France, Germany, Ireland: October 2025
- Belgium, Netherlands: Early 2026

### Ambience Healthcare

**Capabilities:**
- Referral letters included in automated documentation suite
- Generates from recorded visit + EHR data
- Deployed at Cleveland Clinic, Houston Methodist

### Abridge

**Gap Identified:** Based on competitive analysis, Abridge does NOT currently offer automated referral letter generation, focusing instead on:
- Clinical notes
- After-visit summaries
- Revenue cycle intelligence
- Prior authorization workflows

This represents a competitive disadvantage vs. Dragon Copilot and Ambience.

### Other Vendors

| Vendor | Referral Letters | Notes |
|--------|-----------------|-------|
| **Dragon Copilot (Nuance)** | ✅ Full automation | Market-leading; integrated with Epic |
| **Ambience Healthcare** | ✅ Automated | Part of documentation suite |
| **Abridge** | ❌ Not available | Focus on notes, coding, revenue cycle |
| **Suki** | ❌ Not mentioned | Expanding to orders, not referrals |
| **Epic (native)** | 🔄 In development | Part of "Art for Clinicians" |

---

## 5. Patient Portals

### AI Features in Patient Portals (2025)

Patient portals are evolving from passive information displays to AI-powered engagement platforms.

### Oracle Health Patient Portal (September 2025 Announcement)

**Planned Capabilities (GA 2026):**
- Conversational AI for plain-language explanations of diagnoses, test results, treatment options
- Direct questions about individual medical records ("What does this abbreviation mean?")
- Pre-appointment question assistance
- Message drafting help for care team communications
- Follow-up scheduling with alternative appointment suggestions
- Built on OpenAI's frontier models
- No personal medical data stored by OpenAI

### Epic MyChart + Emmie

**Emmie AI Assistant (November 2025):**
- 24/7 availability inside MyChart
- Answer questions about lab results
- Propose appointment times
- Suggest relevant screenings
- Explain results with personalized context
- Guide patients through healthcare decisions
- Take actions (scheduling, recommendations)

**Art + Emmie Integration:**
- AI agents work together to streamline patient outreach
- Respond to feedback in real-time during visits
- Autonomous task coordination

### Conversational AI Market

**Market Size:** Global conversational AI in healthcare expected to reach **$48.87 billion by 2030** (23.84% CAGR)

**Current Capabilities:**
- Appointment scheduling
- FAQs and intake forms
- Post-visit follow-ups
- Prescription status and refill reminders
- Lab results explanation
- Device readiness checks for telehealth

### Appointment Preparation

| Platform | Pre-Visit AI Features |
|----------|----------------------|
| **Oracle Portal** | Pre-appointment questions, medication interaction queries |
| **Epic Emmie** | Visit preparation, screening suggestions |
| **Klara** | Personalized pre-visit instructions |
| **Chat Data** | EHR integration for comprehensive history access |

### Follow-Up Automation

**Next-Generation Capabilities (2025+):**
- Autonomous, proactive digital agents
- Pre-visit paperwork management
- Eligibility checking
- Care milestone tracking
- Automated follow-up initiation
- Cross-system collaboration
- Anticipatory patient needs detection

---

## 6. International Considerations

### Language Requirements by Market

| Market | Primary Languages | AI Vendor Support |
|--------|------------------|-------------------|
| **Australia** | English | All vendors |
| **UK** | English | Nuance (GA), others expanding |
| **France** | French | Nabla (Paris HQ), Nuance (Oct 2025) |
| **Germany** | German | Nuance (Oct 2025) |
| **Netherlands/Belgium** | Dutch, French | Nuance (Early 2026) |
| **UAE/Middle East** | Arabic, English | Limited vendor coverage |
| **Asia-Pacific** | Mandarin, Hindi, others | Abridge (28+ languages), Nabla (35+) |

### Health Literacy Challenges

**Global Disparities:**
- AI-generated content often at higher reading level than recommended for general public
- Low health literacy populations at "perpetual disadvantage"
- AI oversimplification can omit critical content
- Cultural context frequently missing from translations

**FUTURE-AI International Guidelines:**
> "Developers should provide training materials in an accessible format and language, taking into account the diversity of end users (specialists, nurses, technicians, citizens, administrators)."

### Regulatory Requirements

#### European Union

**EU AI Act (2025):**
- Most healthcare AI classified as "high-risk"
- AI literacy requirements apply to ALL AI systems regardless of risk level
- Staff (technical and non-technical) must interpret AI outputs
- Code of Practice for general-purpose AI expected April 2025

**European Health Data Space (EHDS):**
- Entered into force 2025
- First common EU data space in healthcare
- Establishes framework for cross-border health data sharing

**GDPR Requirements:**
| Requirement | Implication for Patient-Facing AI |
|-------------|----------------------------------|
| Lawful processing | Clear legal basis required for all patient data use |
| Transparency | Patients must understand how AI uses their data |
| Right to access/correct/delete | Portal features must support patient data rights |
| Data security | Encryption, access controls mandatory |
| Article 22 | Right to human intervention in automated decisions |
| Consent fragility | Can be withdrawn; must be freely given |

#### United States

**HIPAA:**
- Consent for treatment covers many PHI uses
- Patients should be informed of AI interaction with their data

**AI Bill of Rights (Blueprint):**
- Right to notice and explanation of AI systems
- Easy-to-understand information about AI impacts
- Standards for informed consent

#### United Kingdom (NHS)

**NHS AI Guidance:**
- Healthcare workers must counsel patients about AI data use
- Explain AI tools and clinical decision-making impact
- Communicate risks and limitations
- Guide patients through health decisions

### Patient Consent Considerations

**JAMA Network Open (2025):**
Three normative functions of AI notice/explanation rights:
1. Notify patients about their care
2. Educate patients and promote trust
3. Meet standards for informed consent

**Barriers to Patient Understanding:**
- Algorithm interpretability/transparency issues
- Patient heterogeneity and varying AI/health literacy
- Clinician communication style variations
- "Black box" AI systems lacking explainability

**Regulatory Fragmentation:**
> "What constitutes adequate clinical validation in one country may not satisfy requirements in another. Privacy and data protection standards vary significantly, with the EU's GDPR setting a high bar that other jurisdictions may not match."

### Vendor International Availability

| Vendor | US | Canada | UK | EU | Australia | Asia |
|--------|----|----|----|----|-----------|------|
| **Nuance Dragon Copilot** | ✅ | ✅ | ✅ | 🔄 Oct 2025+ | 🔄 TBD | 🔄 TBD |
| **Abridge** | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Nabla** | ✅ | 🔄 | 🔄 | ✅ (Paris HQ) | ❌ | ❌ |
| **Ambience** | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Suki** | ✅ | ❌ | ❌ | ❌ | ❌ | ❌ |
| **Epic (native)** | ✅ | ✅ | ✅ | 🔄 | ✅ | 🔄 |

---

## Vendor Capability Matrix: Patient-Facing Features

| Capability | Nuance Dragon Copilot | Abridge | Ambience | Suki | Epic Native |
|-----------|----------------------|---------|----------|------|-------------|
| **After-Visit Summaries** | ✅ | ✅ | ✅ | ✅ | 🔄 Emmie |
| **Language Simplification** | ✅ | ✅ | ✅ Level-adaptive | ✅ | 🔄 |
| **Multi-Language** | 🔄 Expanding | ✅ 28+ | TBD | ✅ | 🔄 |
| **Patient Education** | ✅ Via summaries | ✅ Via summaries | ✅ Customized | ✅ | 🔄 Emmie |
| **Inbox Management** | ❌ | ❌ | ❌ | ❌ | ✅ ART |
| **Response Drafting** | ❌ | ❌ | ❌ | ❌ | ✅ LLM drafts |
| **Message Triage** | ❌ | ❌ | ❌ | ❌ | ✅ Prioritization |
| **Referral Letters** | ✅ Full automation | ❌ | ✅ | ❌ | 🔄 |
| **Portal AI** | ❌ | ❌ | ❌ | ❌ | ✅ Emmie |
| **Chat/Conversational** | ❌ | ❌ | ❌ | ❌ | ✅ Emmie |
| **International (EU)** | ✅ Expanding | ❌ | ❌ | ❌ | ✅ |
| **GDPR Compliance** | ✅ | ❌ | ❌ | ❌ | ✅ |

---

## Key Findings & Recommendations

### 1. Market Maturity

**Mature Capabilities (Standard across vendors):**
- After-visit summary generation
- Basic language simplification
- Multi-specialty documentation

**Emerging Capabilities (Differentiators):**
- Patient inbox AI (Epic-led)
- Portal conversational AI (Epic Emmie, Oracle)
- Referral letter automation (Nuance-led)
- Reading level adaptation (Ambience-led)

### 2. Epic's Growing Advantage

Epic is positioning to own the patient-facing AI experience through:
- **Emmie**: Patient-facing AI assistant (Nov 2025)
- **ART**: In-basket response drafting (150+ orgs)
- **Native integration**: Tighter than any third-party

Third-party vendors (Abridge, Ambience, Suki) remain focused on clinician-facing documentation, creating a gap in patient-facing capabilities.

### 3. International Deployment Gaps

For organizations operating globally:
- **Only Nuance** offers credible international expansion plan
- **Nabla** is EU-native but limited in patient-facing features
- **Epic native tools** available internationally but patient AI features US-first
- **US-only vendors** (Abridge, Ambience, Suki) present compliance and operational challenges

### 4. Health Literacy Challenges

AI patient content remains problematic:
- Reading levels often too high for general population
- Oversimplification risks omitting critical information
- Cultural/contextual nuance frequently missing
- Human oversight remains essential (per EU AI Act, FUTURE-AI guidelines)

### 5. Regulatory Trajectory

Expect increasing requirements for:
- Patient notification of AI use
- Explainability of AI-influenced decisions
- Human oversight mechanisms
- Data residency and protection compliance
- AI literacy training for all healthcare staff

---

## Sources

### After-Visit Summaries & Documentation
- [Microsoft Dragon Copilot](https://www.nuance.com/healthcare/dragon-ai-clinical-solutions/dax-copilot.html)
- [Epic EHR AI Trends 2025](https://spsoft.com/tech-insights/epic-ehr-ai-trends-in-2025-reshaping-care/)
- [Nuance DAX Copilot Epic Integration - Healthcare Dive](https://www.healthcaredive.com/news/nuance-dax-copilot-epic-available-artificial-intelligence-clinical-documentation/705026/)
- [Microsoft Blog: Year of DAX Copilot](https://blogs.microsoft.com/blog/2024/09/26/a-year-of-dax-copilot-healthcare-innovation-that-refocuses-on-the-clinician-patient-connection/)

### Language & Translation
- [JMIR AI: AI Translation Spanish Medical Text](https://ai.jmir.org/2025/1/e70222)
- [PMC: AI in Clinical Translation Systematic Review](https://pmc.ncbi.nlm.nih.gov/articles/PMC11729812/)
- [DeepScribe: Multilingual Patient Visits](https://www.deepscribe.ai/resources/enhancing-multilingual-patient-visits-with-ai)
- [Vital Doctor-to-Patient Translator](https://vital.io/newsroom/doctor-to-patient-announcement)

### Patient Education
- [Frontiers: AI Tools for Medication Adherence](https://www.frontiersin.org/journals/digital-health/articles/10.3389/fdgth.2025.1523070/full)
- [John Snow Labs: Conversational Agents in Patient Education](https://www.johnsnowlabs.com/the-role-of-conversational-agents-in-patient-education-programs/)
- [Iris Health AI: AI-Generated Videos](https://www.irishealthai.com/blog/from-confusion-to-compliance-how-ai-generated-videos-are-revolutionizing-patient-understanding)
- [Nature: AI Tools for Tailored Patient Care](https://www.nature.com/articles/s41746-025-01604-3)

### Patient Messaging & Inbox
- [Epic: AI for Patients](https://www.epic.com/software/ai-patients/)
- [EpicShare: Mayo AI Message Responses](https://www.epicshare.org/share-and-learn/mayo-ai-message-responses)
- [Providence: Provaria AI Message Management](https://blog.providence.org/blog/provaria-transforming-care-with-ai-patient-message-management)
- [PMC: AI Workflow for Patient Portal Message Prioritization](https://pmc.ncbi.nlm.nih.gov/articles/PMC11328532/)
- [Healthcare IT News: Epic AI Agents](https://www.healthcareitnews.com/news/epic-unveils-ai-agents-showcases-new-foundational-models)

### Vendor Capabilities
- [Abridge AI Platform](https://www.abridge.com/)
- [Contrary Research: Abridge Business Breakdown](https://research.contrary.com/company/abridge)
- [Ambience Healthcare Patient Recap](https://www.ambiencehealthcare.com/blog/ambience-healthcare-s-patient-recap-offers-clinicians-the-first-chart-summarization-technology-from-an-ambient-ai-platform)
- [Cleveland Clinic Ambience Rollout](https://newsroom.clevelandclinic.org/2025/02/19/cleveland-clinic-announces-the-rollout-of-ambience-healthcares-ai-platform)
- [Suki AI Platform](https://www.suki.ai/)
- [Fierce Healthcare: Suki Patient Summary](https://www.fiercehealthcare.com/ai-and-machine-learning/suki-launches-patient-summary-and-qa-features-its-ai-assistant-google-cloud)

### Patient Portals
- [Oracle Patient Portal AI Announcement](https://www.oracle.com/news/announcement/oracle-to-bring-new-ai-capabilities-to-its-patient-portal-2025-09-10/)
- [CNBC: Epic UGM 2025 AI Tools](https://www.cnbc.com/2025/08/20/epic-ugm-2025-epic-touts-new-ai-tools.html)
- [EMRFinder: Emmie AI Tool](https://emrfinder.com/blog/emmie-new-ai-tool-by-epic-emr-software/)
- [Master of Code: Conversational AI in Healthcare](https://masterofcode.com/blog/conversational-ai-in-healthcare)

### International & Regulatory
- [PMC: Ethical and Legal Considerations in Healthcare AI](https://pmc.ncbi.nlm.nih.gov/articles/PMC12076083/)
- [LegalNodes: EU & UK AI Healthcare Regulation Tracker 2025](https://www.legalnodes.com/article/ai-healthcare-regulation)
- [Chambers: Healthcare AI 2025 Global Guide](https://practiceguides.chambers.com/practice-guides/healthcare-ai-2025)
- [PMC: Patient Consent and Right to Notice](https://pmc.ncbi.nlm.nih.gov/articles/PMC12143229/)
- [HIMSS: AI Literacy Requirements Under EU AI Act](https://legacy.himss.org/news/ai-literacy-requirements-under-eu-ai-act-what-healthcare-leaders-need-know)
- [PMC: FUTURE-AI International Guidelines](https://pmc.ncbi.nlm.nih.gov/articles/PMC11795397/)
- [European Commission: AI in Healthcare](https://health.ec.europa.eu/ehealth-digital-health-and-care/artificial-intelligence-healthcare_en)

---

*Analysis compiled November 2025*
