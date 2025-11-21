# Healthcare AI Vendor Analysis

Comprehensive research and evaluation framework for clinical AI solutions (ambient documentation, CDS, CDI, coding) for enterprise health system procurement decisions.

## Repository Structure

```
├── framework/           # Evaluation frameworks and templates
├── vendors/            # Completed vendor research profiles
├── prompts/            # Research prompts for Claude Code agents
├── research-queue/     # Vendors queued for research
├── completed/          # Archived/completed research tasks
```

## How to Use

### 1. Vendor Research (Claude Code Web Agents)

Use the prompts in `/prompts/` to research individual vendors. Each prompt is designed to be copy-pasted into Claude Code Research Preview.

### 2. Evaluation Framework

See `/framework/evaluation_framework.md` for the complete evaluation criteria.

### 3. Contributing Research

1. Pick a vendor from `/research-queue/`
2. Use the appropriate prompt template
3. Save output to `/vendors/[vendor-name].md`
4. Move the queue file to `/completed/`

## Vendor Coverage

### Tier 1 (Major Players)
- [ ] Microsoft Nuance / Dragon Copilot
- [ ] Abridge
- [ ] Nabla
- [ ] Commure / Augmedix
- [ ] Suki
- [ ] Ambience Healthcare

### Tier 2 (Emerging)
- [ ] DeepScribe
- [ ] Freed
- [ ] Heidi Health
- [ ] Tali AI
- [ ] Sunoh.ai

### Tier 3 (Niche/Regional)
- [ ] Notable Health
- [ ] Regard
- [ ] Corti
- [ ] Saykara (acquired by Nuance)
- [ ] Robin Healthcare

### EHR Native
- [ ] Epic (Art for Clinicians)
- [ ] Oracle Cerner
- [ ] Meditech
- [ ] athenahealth

---

*Author: Alex Stinard, MD*
*Created: November 2025*
