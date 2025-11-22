# Suki AI: Technical Architecture & Platform Strategy Analysis

**Research Date:** November 2025
**Company:** Suki AI, Inc.
**Headquarters:** Redwood City, California
**Founded:** 2017
**Total Funding:** $168M (Series D-II January 2025)
**Valuation:** ~$500M (October 2024)

---

## Executive Summary

Suki AI has evolved from a voice-first clinical documentation tool into a comprehensive healthcare AI platform. Their dual strategy—operating both as a direct product (Suki Assistant) and as infrastructure for other healthcare vendors (Suki Platform)—creates a unique competitive moat. With first-mover advantage in MEDITECH Expanse ambient integration and aggressive expansion into nursing workflows, Suki is positioning itself as a full-stack clinical AI platform rather than a single-purpose ambient scribe.

---

## 1. LLM Stack & Technical Architecture

### Foundation Model Strategy

Suki employs a **multi-LLM orchestration approach** rather than relying on a single provider:

| Component | Technology |
|-----------|------------|
| **LLM Manager** | Proprietary orchestration layer that dynamically selects optimal models per task |
| **Model Portfolio** | Google Gemini (via Vertex AI) + OpenAI models |
| **Clinical Fine-tuning** | Proprietary clinical language model trained on 1M+ patient records across 99+ specialties |
| **Google Cloud Partnership** | Vertex AI platform for patient summaries and Q&A features (announced December 2024) |

**Key Technical Insight:** The LLM Manager allows Suki to abstract away model selection, enabling them to swap models as the market evolves without disrupting end-user experience. This provides insulation from vendor lock-in and allows optimization for cost/accuracy tradeoffs per use case.

### Voice-First Architecture

```
┌─────────────────────────────────────────────────────────────────┐
│                    SUKI VOICE ARCHITECTURE                      │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   ┌─────────────┐    ┌──────────────┐    ┌─────────────────┐  │
│   │   DUAL ASR   │    │    INTENT    │    │   LLM MANAGER   │  │
│   │   ENGINE     │───▶│   EXTRACTOR  │───▶│   ORCHESTRATOR  │  │
│   └─────────────┘    └──────────────┘    └─────────────────┘  │
│         │                    │                    │            │
│   ┌─────▼─────┐        ┌────▼────┐         ┌────▼────┐       │
│   │ Dictation │        │ Slot/   │         │ Gemini/ │       │
│   │    ASR    │        │ Param   │         │ OpenAI  │       │
│   │  (Voice)  │        │ Mapping │         │ Selection│      │
│   └───────────┘        └─────────┘         └──────────┘       │
│         │                                        │             │
│   ┌─────▼─────┐                            ┌────▼────┐        │
│   │ Command   │                            │  Note   │        │
│   │    ASR    │                            │ Output  │        │
│   │ (Actions) │                            │         │        │
│   └───────────┘                            └─────────┘        │
│                                                                │
└─────────────────────────────────────────────────────────────────┘
```

**Dual ASR Approach:**
- **Dictation ASR:** Optimized for continuous speech-to-text with medical terminology
- **Command ASR:** Optimized for intent recognition and action execution
- Both medically-tuned, trained on 8+ years of clinical audio data

**Backend Technology:**
- EMR services written in **Go** (data transformation, processing, database interactions)
- ML/AI team handles intent detection and slot mapping
- Real-time patient context integration (age, specialty, appointment type)

### Real-Time Processing Capabilities

| Capability | Implementation |
|------------|----------------|
| **Ambient Listening** | Continuous capture during patient encounter |
| **Dynamic Context** | Real-time EHR data pull during encounter |
| **Multi-language** | 80+ languages supported with English translation for EHR |
| **Noise Handling** | Optimized for clinical environments |

### Accuracy Benchmarks

| Metric | Performance |
|--------|-------------|
| **Notes with Evidence Links** | 97% of ambient notes linked to supporting transcript/EHR evidence |
| **Note Completion Speed** | 76% faster (average) |
| **Documentation Time Reduction** | 72% per note |
| **After-Hours Work Reduction** | 37% (WellSky partnership data) |
| **Specialty Coverage** | 99+ medical specialties |
| **Adoption Rate** | 70%+ industry-leading |

---

## 2. Platform Architecture

### Suki Assistant vs. Suki Platform

| Aspect | Suki Assistant | Suki Platform |
|--------|----------------|---------------|
| **Target** | Direct to health systems | Healthcare IT vendors (B2B2B) |
| **Delivery** | Standalone application | SDK + APIs for embedding |
| **Use Case** | End-user clinicians | Partners building AI into their products |
| **Revenue Model** | Per-provider subscription | Platform licensing + usage |
| **Customization** | Configuration | Full white-label capabilities |

### SDK & API Offerings

**SDK Capabilities (June 2024 Expansion):**
- **Platforms:** iOS, Android, Web
- **Core Features:**
  - Ambient documentation
  - Medical dictation
  - Voice command processing
  - Note personalization
  - Form-filling by voice
  - Multi-language support

**API Suite:**
- Direct access to AI features for custom UI development
- Ambient AI capabilities
- Speech-to-text processing
- EHR data integration

**Developer Resources:**
- Developer portal: developer.suki.ai
- SDK documentation: resources.suki.ai/platform/suki-sdk-overview
- Custom UI/branding support

### White-Label Capabilities

Partners can fully customize:
- User interface design
- Branding and styling
- Workflow integration
- Feature selection

**Eliminates** need for users to switch between applications—AI appears native to partner's platform.

### Partner Ecosystem

| Partner Type | Key Partners |
|--------------|-------------|
| **EHR Vendors** | athenahealth, MEDENT, Azalea Health |
| **Telehealth** | Zoom Video Communications (+ Zoom Ventures investor) |
| **Veterinary** | Bond Vet / Vetspire (first SDK customer) |
| **Post-Acute** | WellSky (behavioral health, rehab, LTAC) |
| **Health Systems** | MedStar Health, 350+ health systems and clinics |
| **Virtual Care** | AvaSure (bedside documentation) |
| **Cloud** | Google Cloud (Vertex AI platform) |

---

## 3. MEDITECH Leadership & Competitive Moat

### First-to-Market Ambient AI Integration

**Milestone:** July 1, 2025 — Suki became **first company to integrate Ambient AI with MEDITECH Expanse Documentation APIs**

### Integration Timeline

| Date | Milestone |
|------|-----------|
| **September 2024** | Initial MEDITECH partnership announced |
| **2024-2025** | Expanded to 20+ enterprise health systems |
| **July 2025** | Full Expanse Documentation API integration |
| **Planned** | Expanse Now mobile app integration |

### Integration Depth

| Capability | Status |
|------------|--------|
| **Ambient Note Generation** | ✅ Live |
| **Direct EHR Write-back** | ✅ Live (no copy/paste) |
| **In-Expanse Dictation** | ✅ Live |
| **Ambient Clinical Order Entry** | 🔜 Announced |
| **Expanse Now Mobile** | 🔜 Planned |
| **Nursing Workflows** | 🔜 In development |

### Usage Metrics (MEDITECH)

- **100,000+** patient encounters via Suki + MEDITECH
- **1,000+** providers actively using integration
- **20+** enterprise health systems deployed

### Competitive Moat Analysis

| Factor | Assessment |
|--------|------------|
| **First-Mover** | Only ambient AI fully integrated with MEDITECH Expanse APIs |
| **Exclusivity** | No formal exclusive arrangement announced, but significant head start |
| **Switching Cost** | Deep integration creates high switching costs for MEDITECH customers |
| **Expansion Path** | Mobile app, orders, nursing—extending the moat |
| **Market Share** | MEDITECH serves ~20% of US hospitals; significant addressable market |

**Strategic Value:** MEDITECH represents a market segment underserved by Epic-centric competitors like Abridge. Suki's MEDITECH leadership provides differentiated positioning and a path to customers that competitors cannot easily access.

---

## 4. EHR Integrations

### Integration Matrix

| EHR System | Integration Type | Write-back | Implementation Time |
|------------|------------------|------------|---------------------|
| **Epic** | Ambient API, bidirectional sync | ✅ Full | 4-8 weeks |
| **Oracle Health (Cerner)** | Bidirectional ambient sync | ✅ Full | 8-12 weeks |
| **MEDITECH Expanse** | Documentation APIs (first) | ✅ Full | 6-10 weeks |
| **athenahealth** | SDK embedded in athenaOne | ✅ Full | Marketplace instant |
| **MEDENT** | SDK integration | ✅ | 4-6 weeks |
| **Azalea Health** | SDK integration | ✅ | 4-6 weeks |

### Write-Back Capabilities

**Bidirectional Workflow:**
```
EHR → Suki: Patient context, pre-chart data, history
Suki → EHR: Completed notes, structured data, orders (staged)
```

**What Gets Written Back:**
- Clinical notes to appropriate sections
- Structured data fields
- Diagnosis codes (ICD-10)
- Staged orders (with new ambient orders feature)

**Single-Tap Sync:** Notes pushed to EHR with one tap; relevant sections updated in seconds.

### Integration Approach by EHR

**Epic:**
- Leverages Epic's Ambient API
- Available through Epic App Orchard
- Bidirectional data sync
- Real-time patient context pull

**Oracle Health (Cerner):**
- Direct consortium partner
- Suki leads implementation
- Full bidirectional ambient sync
- Pre-charting and note sync between systems
- Sign-off in Cerner workflow

**MEDITECH:**
- First ambient vendor with Documentation API access
- Direct note injection (no copy/paste)
- Tight integration with Expanse workflow

### Maintenance Approach

- Suki maintains all integrations centrally
- Updates deployed without customer action
- EHR version compatibility managed by Suki
- Single integration per EHR type (not per customer)

---

## 5. Expansion Beyond Ambient Documentation

### Current Product Roadmap

```
2024                          2025                          Future
  │                             │                             │
  ├─ Ambient Documentation      ├─ Ambient Order Staging      ├─ Full Order Entry
  │                             │  (April 2025)               │
  ├─ Clinical Dictation         ├─ Nursing Consortium         ├─ Clinical Decision
  │                             │  (October 2025)             │  Support
  ├─ Google Cloud Partnership   │                             │
  │  (December 2024)            ├─ WellSky Integration        ├─ Patient Messaging
  │                             │  (Post-acute care)          │
  ├─ MEDITECH Partnership       │                             ├─ Scheduling
  │  (September 2024)           ├─ Home Health Support        │
  │                             │                             │
  └─────────────────────────────┴─────────────────────────────┘
```

### Orders & Prescriptions

**Ambient Orders Staging (April 2025 — Industry First):**

| Feature | Description |
|---------|-------------|
| **How It Works** | Clinician speaks prescription intent during ambient encounter |
| **AI Processing** | Suki structures, codes, and stages the order |
| **Output** | Order ready for review and signature in EHR |
| **Time Saved** | Orders consume up to 1.4 hours per 8-hour shift |
| **Initial Launch** | athenahealth via Marketplace |
| **Expansion** | Additional EHRs planned |

### Nursing Workflows

**Suki for Nurses Initiative (October 2025):**

**Consortium Members:**
- McLeod Health (Epic)
- Citizens Memorial (MEDITECH)
- Boone Health (MEDITECH)
- Fisher-Titus

**Partnership:** AvaSure for bedside documentation

**Phase 1 Focus:**
- Patient assessments
- Admission/intake forms
- Discharge documentation
- Hands-free form completion

**Phase 2:**
- Bedside documentation without interruption
- Flowsheet integration
- Real-time charting

**Business Driver:** 1 in 4 nurses cite burnout/understaffing as reason for leaving profession.

### Home Care & Post-Acute

**WellSky Partnership (October 2025):**
- Behavioral health facilities
- Rehabilitation centers
- Long-term acute care (LTAC)
- Skilled nursing facilities

**Coverage Expansion:**
- Hospital inpatient
- Ambulatory/outpatient
- Telehealth
- Skilled nursing facilities
- Home health

### Coding Assistance

| Feature | Status |
|---------|--------|
| **Diagnosis Code Suggestion** | ✅ Live (ICD-10) |
| **Note-to-Code Extraction** | ✅ Live |
| **Claim Denial Reduction** | 19% improvement reported |
| **Full CDI Integration** | Not yet announced |

### Clinical Q&A & Patient Summaries (Google Cloud Partnership)

**New Capabilities:**
- One-click patient summaries (demographics, history, medications, conditions)
- Natural language Q&A about patient records
- Example queries: "Show A1C over last 3 months as graph", "When was last ECG?"
- Time savings: 15-30 minutes per patient previously spent searching

---

## 6. Financial & Market Position

### Funding History

| Round | Date | Amount | Lead Investor |
|-------|------|--------|---------------|
| Series A | 2018 | $20M | Venrock |
| Series B | 2020 | $20M | Flare Capital |
| Series C | 2021 | $55M | March Capital |
| Series D | Oct 2024 | $70M | Hedosophia |
| Series D-II | Jan 2025 | Undisclosed | — |
| **Total** | — | **$168M** | — |

**Key Investors:** Venrock, First Round, Flare Capital, March Capital, Breyer Capital, Hedosophia, Zoom Ventures

### Growth Metrics

| Metric | Value |
|--------|-------|
| **2023 Revenue Growth** | 4x (quadrupled) |
| **2024 Revenue Growth** | 3x (tripled) |
| **2025 Revenue Growth** | 3x expected |
| **Health System Partners** | 350+ |
| **Clinician Adoption Rate** | 70%+ |
| **Year 1 ROI** | 9x claimed |

### Competitive Positioning

| Competitor | Suki Differentiation |
|------------|---------------------|
| **Nuance DAX** | Fully automated (no human QA), lower cost, platform strategy |
| **Abridge** | MEDITECH leadership, nursing expansion, platform/SDK model |
| **Epic (Native)** | EHR-agnostic, platform model, broader specialty coverage |
| **Nabla** | Enterprise focus, deeper EHR integrations, US market maturity |

### Pricing Context

| Vendor | Estimated Monthly Cost (per provider) |
|--------|--------------------------------------|
| Nuance DAX | $400-600 |
| Suki | $400-600 |
| Abridge | ~$250 |
| Nabla | ~$120 |

---

## 7. Technical Risks & Considerations

### Strengths

- **Platform + Product dual model** creates multiple revenue streams
- **Multi-LLM architecture** provides model flexibility and vendor independence
- **MEDITECH first-mover** opens underserved market segment
- **Nursing expansion** addresses massive unmet need
- **8+ years of clinical voice data** provides training advantage

### Risks

| Risk | Mitigation |
|------|------------|
| **Epic/Microsoft alignment** | MEDITECH focus, platform strategy for EHR-embedded delivery |
| **Pricing pressure** | Platform model provides alternative revenue, ROI-based selling |
| **Nuance Microsoft resources** | Focus on speed, automation, EHR agnostic value |
| **EHR vendor native solutions** | SDK/API model lets Suki power native solutions |

### Integration Considerations

- Implementation ranges 4-12 weeks depending on EHR
- Suki-led implementation reduces customer IT burden
- Single integration maintained centrally
- All EHR version compatibility handled by Suki

---

## Sources

### Official Suki Resources
- [Suki AI Homepage](https://www.suki.ai/)
- [Suki Technology Overview](https://www.suki.ai/technology/)
- [Suki Partner Platform](https://www.suki.ai/partners/)
- [Suki EHR Integrations](https://www.suki.ai/ehr-integrations/)
- [Suki MEDITECH Integration](https://www.suki.ai/meditech-integration/)
- [Suki Cerner Integration](https://www.suki.ai/cerner-integration/)
- [Suki SDK Portal](https://developer.suki.ai/web-sdk)

### Press Releases & News
- [Suki MEDITECH Expanse First Integration (July 2025)](https://www.businesswire.com/news/home/20250701795662/en/Suki-Becomes-First-to-Integrate-Ambient-AI-with-MEDITECH-Expanse-Documentation-APIs)
- [Suki Series D Funding (October 2024)](https://www.suki.ai/news/suki-secures-70m-series-d-funding-as-demand-surges-expands-strategic-partnership-with-medstar-health/)
- [Suki SDK Launch (June 2024)](https://www.businesswire.com/news/home/20240604693899/en/Suki-Extends-the-Capabilities-of-its-Developer-Platform-With-SDK-and-APIs-to-Power-Voice-AI-Experiences)
- [Suki Nursing Consortium (October 2025)](https://www.businesswire.com/news/home/20251008550667/en/Suki-Launches-Nursing-Consortium-with-a-Broad-Coalition-of-Health-Systems-to-Support-Frontline-Nurses-Amid-Ongoing-Staffing-Crisis)
- [Suki Ambient Orders (April 2025)](https://www.businesswire.com/news/home/20250403618881/en/Suki-Unveils-Industry-First-Ambient-Orders-Staging-for-its-AI-Assistant)

### Industry Analysis
- [Suki Google Cloud Partnership (NBC New York)](https://www.nbcnewyork.com/news/business/money-report/health-ai-startup-suki-expands-partnership-with-google-cloud-to-deliver-more-assistive-tech-for-clinicians/6078337/)
- [Suki Epic Integration (Healthcare Dive)](https://www.healthcaredive.com/news/suki-integrates-generative-ai-assistant-in-epic-ehr-software/650668/)
- [Healthcare IT News - Suki Nursing](https://www.healthcareitnews.com/news/suki-launches-nursing-consortium-improve-ai-assistant-integration)
- [WellSky Ambient Launch](https://www.businesswire.com/news/home/20251030004012/en/WellSky-Launches-AI-Powered-Ambient-Listening-for-Specialty-Care-EHR)
- [Sacra - Suki Valuation](https://sacra.com/c/suki/)
- [Healthcare IT Today - Suki Differentiation](https://www.healthcareittoday.com/2023/10/27/the-evolution-of-sukis-ambient-clinical-voice-solution-and-what-differentiates-it-in-the-market/)
- [MobiHealth News - Series D](https://www.mobihealthnews.com/news/suki-secures-70m-enhance-its-ai-ambient-scribe-offerings)

### Technical Deep Dives
- [Engineering Voice Agent for Clinicians (Suki Blog)](https://www.suki.ai/blog/engineering-an-invisible-and-assistive-voice-agent-for-clinicians/)
- [Suki SDK Standards (Suki Blog)](https://www.suki.ai/blog/enhanced-efficiency-sukis-sdk-sets-new-standards-in-healthcare/)
- [AI-Generated Clinical Notes Standards (Suki Blog)](https://www.suki.ai/blog/setting-a-new-standard-for-ai-generated-clinical-notes/)

---

*Analysis completed November 2025*
