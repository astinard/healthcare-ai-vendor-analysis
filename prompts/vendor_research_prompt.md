# Vendor Research Prompt Template

Copy and paste this prompt into Claude Code Research Preview, replacing `[VENDOR_NAME]` with the target vendor.

---

## Prompt

```
Research [VENDOR_NAME] healthcare AI solution. Gather comprehensive, current information (2025) on:

## 1. Company Profile
- Founded, HQ, valuation, funding rounds, total raised
- Employee count, clinical team size (MDs, RNs on staff)
- Key investors (especially strategic: health systems, EHR vendors, cloud providers)
- Revenue model (per-provider, per-encounter, enterprise license)
- Target market (SMB, mid-market, enterprise, academic)

## 2. Technology Stack
- Primary LLM (GPT-4, Claude, Gemini, proprietary, open-source)
- ASR provider (Deepgram, Whisper, Nuance, proprietary)
- Agentic architecture (single-shot vs. multi-agent)
- Tool use capabilities (EHR read/write, coding lookup, order entry)
- Memory/context (stateless vs. persistent across encounters)
- Knowledge graph / ontology mapping (SNOMED, LOINC, RxNorm)
- RAG implementation details
- On-prem option available?

## 3. Clinical Capabilities
### Ambient Documentation
- Real-time vs. post-visit generation
- Specialties supported (count and which ones)
- Note types (SOAP, H&P, procedure notes, consults)
- Template customization options
- Multi-language support
- Diarization accuracy

### Beyond Ambient
- Auto-coding (ICD-10, CPT/HCPCS)
- CDI (real-time documentation integrity)
- CDS (care gaps, risk scores, alerts)
- Pre-charting / patient summaries
- After-visit summaries
- Orders suggestion
- MDM calculation / E&M support

## 4. EHR Integration
- Which EHRs supported (Epic, Cerner, Meditech, Athena, etc.)
- Integration depth (SMART on FHIR, API write-back, RPA)
- Epic App Orchard status
- Bi-directional (read AND write)?
- Time to go-live

## 5. Safety & Compliance
- Guardrails architecture
- Hallucination mitigation approach
- Red-teaming program
- PHI/PII controls
- Audit trail capabilities
- HIPAA, SOC 2, HITRUST, GDPR, FDA status
- Data residency options

## 6. Market Position
- Key customers (health systems by name)
- Partnerships (cloud, LLM, EHR vendors)
- Geographic focus
- Competitive differentiation
- Recent news (last 6 months)

## 7. Pricing
- List price if available
- Pricing model details
- ROI metrics claimed

## 8. Roadmap
- 2025-2026 planned features
- Expansion plans

Format the output as a structured markdown document suitable for comparison with other vendors.
```

---

## Quick Prompts (Copy-Paste Ready)

### Nuance/Microsoft
```
Research Microsoft Nuance Dragon Copilot / DAX Copilot healthcare AI solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Abridge
```
Research Abridge AI healthcare solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Nabla
```
Research Nabla AI healthcare solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Suki
```
Research Suki AI healthcare solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### DeepScribe
```
Research DeepScribe healthcare AI solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Freed
```
Research Freed AI healthcare documentation solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Ambience Healthcare
```
Research Ambience Healthcare AI solution. Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Heidi Health
```
Research Heidi Health AI healthcare solution (Australia-based). Gather comprehensive, current information (2025) on company profile, technology stack, clinical capabilities, EHR integration, safety & compliance, market position, pricing, and roadmap. Format as structured markdown.
```

### Epic Art for Clinicians
```
Research Epic's native AI scribe "Art for Clinicians" announced at UGM 2025. Gather comprehensive, current information on capabilities, rollout timeline, integration with Epic workflows, and competitive implications for third-party ambient AI vendors. Format as structured markdown.
```

### Oracle Cerner AI
```
Research Oracle Cerner / Oracle Health AI documentation and clinical AI capabilities. Gather comprehensive, current information (2025) on native AI features, partnerships, and competitive positioning. Format as structured markdown.
```
