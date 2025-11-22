# Freed AI - Healthcare Documentation Solution Research

**Research Date:** November 2025
**Vendor:** Freed (getfreed.ai)
**Category:** Ambient AI Medical Scribe
**Market Position:** SMB/Small Practice Disruptor

---

## Executive Summary

Freed is a fast-growing AI medical scribe targeting solo practitioners and small/mid-sized practices. With a simple $99/month pricing model and product-led growth strategy, Freed has achieved rapid adoption (25,000+ clinicians) while avoiding the lengthy enterprise sales cycles that competitors face. Backed by Sequoia Capital's $30M Series A, Freed represents the "bottom of market" play in ambient documentation, prioritizing simplicity and speed over deep EHR integration.

---

## 1. Company Profile

| Attribute | Details |
|-----------|---------|
| **Founded** | 2022 |
| **Headquarters** | Santa Rosa, California, USA |
| **Founders** | Erez Druk (CEO), Andrey Bannikov (CTO) |
| **Total Funding** | $34M |
| **Latest Round** | $30M Series A (March 2025) |
| **Lead Investor** | Sequoia Capital |
| **Other Investors** | Scale Venture Partners, Daniel Gross, Gokul Rajaram, Ted Zagat |
| **Valuation** | Not publicly disclosed |

### Founder Background

- **Erez Druk (CEO):** Former Facebook software engineer (2013-2017). Founded UrbanLeap (public procurement software), shuttered in 2022. Top of class at Israel Institute of Technology (Technion). Motivation: watching his wife, Dr. Gabi Meckler (family physician), spend nights on documentation.

- **Andrey Bannikov (CTO):** Decade at Facebook before co-founding Freed. Met Erez on his first day at Facebook.

### Y Combinator Status

**Note:** Despite some sources suggesting Y Combinator involvement, research could not confirm that Freed participated in any YC batch. The company is NOT listed in YC's official healthcare startup directory.

### Revenue Model

| Model | Details |
|-------|---------|
| **Pricing** | $99/month per clinician (flat rate) |
| **ACV** | ~$1,000/clinician (after student/trainee discounts) |
| **Model Type** | SaaS, per-provider subscription |
| **Free Trial** | 7 days |
| **Annual Option** | Available (likely discount) |

### Target Market

- Solo practitioners
- Small practices (1-10 providers)
- Mid-sized practices
- Independent practices (47% of US clinicians)
- **NOT targeting:** Enterprise health systems, large hospital networks

---

## 2. Growth Metrics & Traction

### ARR Growth

| Period | ARR | YoY Growth | Clinicians |
|--------|-----|------------|------------|
| August 2023 | ~$1.2M | - | 1,000 |
| March 2024 | $8M | - | - |
| August 2024 | $13M | 992% | 12,000 |
| March 2025 | $19M | 134% | 17,000 |
| April 2025 | $20M+ | - | 20,000+ |
| Current (Nov 2025) | Est. $25M+ | - | 25,000+ |

### Key Milestones

- Crossed $10M ARR in fewer than 12 months with only 4 salespeople
- 4x YoY ARR growth at scale
- 96 specialties supported
- 2.5M+ cumulative hours saved for clinicians
- Named to CB Insights Digital Health 50 (2025)

### Growth Strategy

- **Product-Led Growth (PLG):** Self-serve, direct-to-clinician
- **Bypasses enterprise procurement:** Clinicians buy directly
- **Word of mouth:** Viral growth in physician communities
- **Growth rate comparable to:** Slack, Zoom (consumer SaaS)

---

## 3. Technology Stack

### AI/LLM Infrastructure

| Component | Details |
|-----------|---------|
| **Primary LLM** | Not disclosed (likely proprietary + foundation models) |
| **OpenAI Partnership** | NOT confirmed (competitor Ambience has OpenAI backing) |
| **Cloud Infrastructure** | Microsoft Azure |
| **Speech Recognition** | Proprietary ambient listening |
| **Medical Terminology** | 27,000+ medications supported |
| **Languages** | 14+ languages |

### Architecture Features

- Real-time transcription during patient visits
- Self-learning system that adapts to clinician's documentation style
- Note generation in seconds (near real-time)
- No audio storage (privacy by design)
- Automatic deletion of notes after 30 days

### Technical Limitations

- No publicly disclosed agentic architecture
- No knowledge graph / ontology mapping mentioned
- No RAG implementation details available
- No on-premise option (cloud-only)

---

## 4. Clinical Capabilities

### Ambient Documentation

| Feature | Status |
|---------|--------|
| **Real-time generation** | Yes |
| **Specialties supported** | 96+ |
| **Note types** | SOAP, clinical notes, after-visit summaries |
| **Template customization** | Yes (learns clinician style) |
| **Multi-language** | 14+ languages |
| **Diarization** | Supported |

### Workflow Features

| Feature | Status |
|---------|--------|
| **Pre-visit summaries** | Yes |
| **During-visit capture** | Yes (real-time) |
| **Post-visit notes** | Yes |
| **ICD-10 coding** | Yes (auto-suggests) |
| **After-visit summaries** | Yes |

### Beyond Ambient (Limited)

| Capability | Status |
|------------|--------|
| **Auto-coding (CPT/HCPCS)** | Basic |
| **CDI (Clinical Documentation Integrity)** | No |
| **CDS (Clinical Decision Support)** | No |
| **Order suggestions** | No |
| **MDM calculation** | No |
| **Revenue cycle integration** | No |

---

## 5. EHR Integration

### Integration Approach: "EHR Push"

Freed takes a **lightweight, EHR-agnostic approach** vs. deep API integration:

| Feature | Details |
|---------|---------|
| **Method** | Chrome extension with "EHR Push" |
| **How it works** | One-click transfer into browser-based EHR fields |
| **Setup time** | Minutes (no IT required) |
| **API integration** | Not required |
| **FHIR support** | Limited |
| **Bi-directional** | Push only (not read) |

### Supported EHRs

Works with **any browser-based EHR**, including:
- athenahealth (marketplace listing)
- Epic (via browser, not deep integration)
- Cerner/Oracle Health
- NextGen
- eClinicalWorks
- Others (browser-based)

### Integration Comparison

| Vendor | Integration Depth | Setup Time |
|--------|-------------------|------------|
| **Freed** | Browser extension | Minutes |
| **Abridge** | Deep Epic API | Weeks-months |
| **Nuance** | Deep Epic embedded | Weeks-months |
| **Ambience** | Epic integration | Weeks-months |

### Limitations

- No Epic App Orchard certification
- No native Epic/Cerner integration
- "EHR write-back API" in development (no public ETA)
- High-volume practices may find browser-based workflow manual

---

## 6. Safety & Compliance

| Certification | Status |
|---------------|--------|
| **HIPAA** | Compliant |
| **HITECH** | Compliant |
| **SOC 2 Type II** | Certified |
| **HITRUST** | Not mentioned |
| **GDPR** | Not mentioned |
| **FDA** | N/A |

### Privacy Features

- BAA (Business Associate Agreement) published
- Data encrypted at rest and in transit
- No patient audio recordings stored
- Notes auto-deleted after 30 days
- Azure secure cloud infrastructure

### Safety Architecture

| Feature | Details |
|---------|---------|
| **Guardrails** | Not detailed |
| **Hallucination mitigation** | Clinician review required |
| **Red-teaming** | Not disclosed |
| **Audit trail** | Basic |

---

## 7. KLAS Research Status

### KLAS Ratings

**Freed is NOT rated in KLAS Best in KLAS awards for 2025.**

| Vendor | KLAS Status |
|--------|-------------|
| **Abridge** | 2025 Best in KLAS - Ambient AI |
| **Nuance DAX** | Rated, competitive |
| **Freed** | Not rated (SMB focus) |

KLAS primarily rates enterprise vendors; Freed's SMB focus likely excludes it from major KLAS evaluations.

---

## 8. Market Position & Competition

### Competitive Landscape

| Vendor | ARR | Target | Pricing | EHR Depth |
|--------|-----|--------|---------|-----------|
| **Abridge** | ~$100M | Enterprise | ~$500/mo | Deep Epic |
| **Ambience** | ~$30M | Enterprise | Custom | Deep Epic |
| **Nuance** | Microsoft | Enterprise | $500-700/mo | Deep Epic |
| **Freed** | ~$25M | SMB | $99/mo | Light |

### Competitive Advantages

1. **Price:** 5-7x cheaper than enterprise alternatives
2. **Setup speed:** Minutes vs. weeks/months
3. **No IT involvement:** Direct clinician purchase
4. **Simplicity:** No complex integrations
5. **Viral growth:** Strong word-of-mouth

### Competitive Disadvantages

1. **Limited EHR integration:** No deep API write-back
2. **No enterprise features:** No CDI, CDS, revenue cycle
3. **Scale limitations:** High-volume practices may outgrow
4. **No KLAS recognition:** Not validated by enterprise buyers
5. **Limited safety disclosures:** Less transparency than enterprise vendors

### Key Differentiator Quote

> "Freed is not designed to make you more productive, make you more money, or help you become a better clinician. The only purpose of Freed is to make clinicians happier." - CEO Erez Druk

---

## 9. Customer Testimonials

### Time Savings

- **Average reported:** 2+ hours saved per day
- **Cumulative:** 2.5M+ hours saved across all users

### Representative Quotes

**Mental Health Clinician:**
> "What used to take me hours now gets done in minutes; accurately and effortlessly. I can finally spend more time focusing on my clients."

**Direct Primary Care Doctor:**
> "A note that would normally take me 20 minutes to write is just done."

**Career Impact:**
> "Freed saved me from leaving medicine. The countless hours typing notes, feeling as if I was a bot rather than a doctor."

**Psychiatry NP (Natalie Desseyn):**
> "People feel really heard because I'm not focused on writing."

### Constructive Criticism

- Notes can be repetitive
- Proofreading still required
- Occasional medication spelling errors
- Some abbreviation inconsistencies

---

## 10. Pricing

### Standard Pricing

| Plan | Price | Billing |
|------|-------|---------|
| **Monthly** | $99/month | Per clinician |
| **Annual** | Likely discounted | Per clinician |
| **Free Trial** | 7 days | Full access |
| **Students/Trainees** | Discounted | - |

### ROI Metrics

| Metric | Claim |
|--------|-------|
| **Time saved** | 2+ hours/day |
| **Note generation** | Seconds |
| **Setup time** | Minutes |

### Pricing Comparison

| Vendor | Monthly Price | Annual Cost |
|--------|---------------|-------------|
| **Freed** | $99 | ~$1,200 |
| **Abridge** | ~$500 | ~$6,000 |
| **Nuance** | $500-700 | ~$7,200+ |

---

## 11. 2025-2026 Roadmap

### Confirmed Developments

| Feature | Status | Timeline |
|---------|--------|----------|
| **EHR Push** | Free beta | Through end of 2025 |
| **EHR Push GA** | Planned | 2026 |
| **EHR Write-back API** | In development | No public ETA |

### Strategic Direction

- **Beyond note writing:** Building "next-generation AI clinician assistant"
- **Series A funds allocated for:** Expansion beyond ambient documentation
- **Market expansion:** Likely to move upmarket toward mid-market practices

### Potential Threats

1. **Epic "Art for Clinicians":** Native Epic AI scribe (announced Aug 2025)
2. **Enterprise vendors moving downmarket:** Abridge, Nuance could target SMB
3. **EHR-native AI:** athenahealth, Cerner building native features
4. **Commoditization:** AI scribe becoming table stakes

---

## 12. Investment Thesis

### Bull Case

- Massive TAM in independent practice segment (47% of US clinicians)
- PLG model enables efficient growth without enterprise sales
- 992% YoY growth demonstrates product-market fit
- Sequoia backing provides credibility and resources
- Simple product beloved by users (strong NPS)

### Bear Case

- Limited moat (technology not differentiated)
- Enterprise vendors could easily move downmarket
- No deep EHR integration limits expansion
- KLAS absence hurts credibility with larger buyers
- Thin safety/compliance documentation

---

## Sources

### Primary Sources
- [Freed Official Website](https://www.getfreed.ai)
- [Sequoia Capital Partnership Announcement](https://sequoiacap.com/article/partnering-with-freed-an-ai-powered-clinicians-assistant/)
- [BusinessWire: $30M Series A Announcement](https://www.businesswire.com/news/home/20250305397400/en/Freed-Secures-30M-Series-A-Led-by-Sequoia-Capital-to-Free-Clinicians-from-Administrative-Burdens-with-AI-Assistant)

### Market Intelligence
- [Sacra: Freed at $19M ARR](https://sacra.com/research/freed-at-19m-arr/)
- [Sacra: Abridge vs Ambience vs Freed](https://sacra.com/research/abridge-vs-ambience-vs-freed/)
- [VentureBeat: 20,000 Clinicians](https://venturebeat.com/ai/freed-says-20000-clinicians-are-using-its-medical-ai-transcription-scribe-but-competition-is-rising-fast)

### News & Analysis
- [CNBC: Freed raises $30M led by Sequoia](https://www.cnbc.com/2025/03/05/freed-raises-30-million-led-by-sequoia-to-tackle-clinician-burnout.html)
- [Fierce Healthcare: Fundraising Tracker](https://www.fiercehealthcare.com/health-tech/fierce-healthcare-fundraising-tracker-freed-picks-30m-ai-clinician-assistant)
- [BusinessWire: EHR Push Announcement](https://www.businesswire.com/news/home/20251001257852/en/Freed-Unveils-EHR-Push-One-Click-AI-Note-Transfer-Into-Any-Web-Based-EHR)

### Reviews & Testimonials
- [Freed AI Reviews](https://love.getfreed.ai/b2xGQ1)
- [MSPowerUser Review](https://mspoweruser.com/freed-ai-review/)
- [Twofold Review](https://www.trytwofold.com/compare/freed-ai-scribe-review)
- [Global Healthcare Magazine: Erez Druk Interview](https://globalhealthcaremagazine.com/erez-druk/)

### Competitive Intelligence
- [S10.ai: AI Scribe Comparison](https://s10.ai/blog/which-is-better-for-healthcare-organizations-sullyai-heidi-health-freed-ai-abridge-dragon-ambient-experience-ambience-healthcare-or-deepscribe)
- [KLAS Research: Healthcare AI 2025](https://klasresearch.com/report/healthcare-ai-2025-are-you-keeping-pace-with-industry-adoption/3749)

---

*Research compiled November 2025*
