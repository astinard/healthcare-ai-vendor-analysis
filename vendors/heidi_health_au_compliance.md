# Heidi Health - Australian Regulatory Compliance Analysis

**Company:** Heidi Health (Heidi Health Trading Pty Ltd)
**Headquarters:** Melbourne, Australia
**Founded:** 2019
**Product:** AI Medical Scribe (ambient documentation)
**Analysis Date:** November 2025

---

## 1. TGA STATUS

### Classification

| Aspect | Status |
|--------|--------|
| TGA Registration | **Not registered as medical device** |
| ARTG Listing | Not required (currently) |
| Device Classification | Not classified as SaMD |
| Regulatory Position | Administrative documentation tool |

### Detailed Assessment

**Current Position:** Heidi Health explicitly states it is **not classified as a medical device** under Therapeutic Goods Administration (TGA) regulations. The company positions its AI scribe as an administrative documentation tool rather than software intended for diagnosis or treatment decisions.

**Rationale:** AI medical scribes are generally exempt from TGA regulation because they are considered administrative documentation tools, not software that supports diagnosis, treatment, or clinical decision-making.

**Future Considerations:**
- If features are added that give Heidi a "therapeutic purpose," reclassification as Software as a Medical Device (SaMD) may be required
- The TGA has announced it is "stepping up its efforts" to regulate digital scribes, including AI-based solutions
- Features that could trigger reclassification include: diagnostic suggestions, treatment recommendations, clinical decision support

**Company Statement:** CEO Dr. Thomas Kelly stated the company would "engage with the regulator if we ever introduce features that give Heidi a therapeutic purpose."

### Clinical Claims Allowed

| Claim Type | Permitted |
|------------|-----------|
| Documentation accuracy | Yes |
| Time savings | Yes |
| Administrative efficiency | Yes |
| Diagnostic recommendations | No |
| Treatment suggestions | No |
| Clinical decision support | No (would trigger SaMD) |

**Note:** In the UK, Heidi is registered as a Class I medical device under MHRA guidance for summarisation functionality, demonstrating awareness of regulatory pathways when needed.

---

## 2. PRIVACY COMPLIANCE

### Australian Privacy Principles (APPs)

| APP | Compliance Status | Implementation |
|-----|-------------------|----------------|
| APP 1 - Open and transparent management | Compliant | Published privacy policy and compliance documentation |
| APP 2 - Anonymity and pseudonymity | Compliant | Automatic de-identification with "Jane Doe" substitution |
| APP 3 - Collection of solicited information | Compliant | Purpose-limited collection |
| APP 4 - Dealing with unsolicited information | Compliant | Strict data handling protocols |
| APP 5 - Notification of collection | Compliant | Clear disclosure to users |
| APP 6 - Use or disclosure | Compliant | Purpose limitation enforced |
| APP 7 - Direct marketing | Compliant | Opt-out mechanisms available |
| APP 8 - Cross-border disclosure | Compliant | Pre-disclosure safeguards |
| APP 9 - Government identifiers | Compliant | Not used as internal identifiers |
| APP 10 - Quality of personal information | Compliant | Data quality controls |
| APP 11 - Security of personal information | Compliant | ISO 27001, SOC 2 Type II |
| APP 12 - Access to personal information | Compliant | Access request procedures |
| APP 13 - Correction of personal information | Compliant | Correction mechanisms |

### Health Records Act Compliance

**Approach:** Heidi achieves compliance with state and territory health records laws through:
- Pseudonymization of all patient data
- Non-retention policies (configurable)
- Use of compliant local storage solutions (Australian data residency)
- End-to-end encryption

### State-Level Health Privacy Laws

| State/Territory | Relevant Law | Compliance Approach |
|-----------------|--------------|---------------------|
| Victoria | Health Records Act 2001 | Data localization + pseudonymization |
| NSW | Health Records and Information Privacy Act 2002 | Local storage + access controls |
| ACT | Health Records (Privacy and Access) Act 1997 | Compliant data handling |
| All states | Privacy Act 1988 (Cth) | Full APP compliance |

### My Health Record Integration

**Current Status:** No direct integration with Australia's My Health Record (operated by Australian Digital Health Agency) identified.

**EHR Integrations Available:**
- Best Practice Software (Australian market leader)
- MediRecords (cloud-based Australian EHR)
- MedicalDirector

These practice management systems may independently connect to My Health Record, but Heidi does not directly write to or read from the national health record.

---

## 3. DATA HANDLING

### Data Storage Location

| Region | Storage Location | Compliance |
|--------|------------------|------------|
| Australia | Australian servers | Data sovereignty maintained |
| UK | UK servers | UK GDPR compliant |
| US | US servers | HIPAA compliant |
| Canada | Canadian servers | PIPEDA compliant |
| EU | EU servers | GDPR compliant |

**Key Commitment:** "All data is locally hosted within Australia" for Australian users.

### Data Retention Policies

| Setting | Description |
|---------|-------------|
| Default | "Never delete" (to preserve documentation) |
| Minimum | 1 day |
| Maximum | Unlimited |
| Control | Fully customizable by user/organization |

**Rationale for Default:** Transcripts may be valuable for documentation or evidence of consultations and should not be unintentionally lost.

### De-identification Approach

**Technique:** Automatic pseudonymization

| Process | Implementation |
|---------|----------------|
| Personal identifiers | Replaced with "Jane Doe" / "John Doe" equivalents |
| Timing | Before transcript processing |
| PHI handling | De-identified and processed separately |
| Re-identification risk | Processes ensure no reasonable likelihood |

**Architecture:**
1. Audio captured during consultation
2. Personal identifiers stripped before AI processing
3. Special category health data pseudonymized before note generation
4. Protected Health Information (PHI) de-identified and stored separately

### Cross-Border Data Transfers

| Safeguard | Implementation |
|-----------|----------------|
| Pre-transfer assessment | Reasonable steps to ensure overseas recipients comply with APPs |
| Data localization | Regional servers available (AU, UK, US, CA, EU) |
| Third-party sharing | No PHI shared with third-party analytics tools |
| Model training | Customer data NOT used to train AI models |

**Explicit Statement:** "No patient data from users is used to train, develop, or improve any of Heidi's AI models."

---

## 4. CLINICAL GOVERNANCE

### Medical Oversight

| Role | Personnel |
|------|-----------|
| CEO/Co-Founder | Dr. Thomas Kelly (former vascular surgeon) |
| UK Chief Medical Officer | Dr. Hannah Allen (practicing GP, NHS Clinical Safety Officer) |
| Clinical Safety Officers | Dr. Samuel Adedero, Dr. Kieran McLeod |
| Clinical Content | Dr. Ben Condon (Clinical Content Editor) |
| Clinical Team Size | 20+ clinicians stress-testing and training AI |

### Clinical Safety Framework

**UK DCB Standards:** Three NHS-accredited Clinical Safety Officers with responsibility under:
- DCB0129 (Clinical Risk Management for Manufacturers)
- DCB0160 (Clinical Risk Management for Healthcare Organizations)

**Documentation:**
- Clinical Safety Case Report maintained
- Hazard log kept current
- Regular governance and quality process reviews

### Quality Assurance

| Process | Description |
|---------|-------------|
| Clinical validation | Internal healthcare professionals review outputs |
| Technical accuracy | Rigorous QA on all outputs |
| Real-world testing | Testing before deployment |
| Post-deployment monitoring | Continuous monitoring and updates |
| Bias monitoring | QA team monitors for model bias |
| Performance metric | <1 negative rating per 1,000 notes |

### Error Reporting

**Incident Response Protocol:**

| Stage | Action |
|-------|--------|
| 1. Detection | Employees, contractors, users report to Compliance Lead or CTO |
| 2. Triage | Event reported, triage and analysis |
| 3. Investigation | Root cause analysis |
| 4. Containment | Short-term neutralization |
| 5. Recovery | System recovery and vulnerability remediation |
| 6. Notification | Users notified via email and in-app |
| 7. Regulatory | Assistance with regulatory body reporting |
| 8. Post-mortem | Lessons learned documentation |

**Compliance Framework:** Incident response follows ISO 27001 and SOC 2 obligations.

### Clinical Advisory Board

**Structure:** Integrated medical team rather than formal external advisory board.

**Medical Leadership:**
- Founded by practicing clinician (Dr. Thomas Kelly - vascular surgery)
- Multiple medical doctors on staff team
- 20+ clinicians involved in product development and testing
- Described as "a team of medicos (active and ex-), and folks who've felt what healthcare is like"

---

## 5. CERTIFICATIONS

### Security Certifications

| Certification | Status | Scope |
|---------------|--------|-------|
| ISO 27001:2022 | Certified | Information security management |
| SOC 2 Type II | Certified | Security, availability, confidentiality |
| ISO 9001 | Certified | Quality management |
| Cyber Essentials | Certified | UK cybersecurity baseline |

**Achievement Timeline:** All major certifications (GDPR, HIPAA, ISO 27001:2022, SOC 2) achieved within 10 months.

### Privacy/Regulatory Compliance

| Framework | Region | Status |
|-----------|--------|--------|
| Australian Privacy Principles (APPs) | Australia | Compliant |
| NZ Information Privacy Principles | New Zealand | Compliant |
| HIPAA | United States | Compliant |
| GDPR | European Union | Compliant |
| UK GDPR + DPA 2018 | United Kingdom | Compliant |
| PIPEDA | Canada | Compliant |
| NHS DCB0129/DCB0160 | UK | Compliant (3 accredited CSOs) |

### Technical Security Controls

| Control | Implementation |
|---------|----------------|
| Encryption in transit | TLS 1.2+ |
| Encryption at rest | AES-256 |
| Penetration testing | Annual |
| Access control | Clinician-controlled, explicit patient consent required |
| Audio storage | No audio stored during transcription |

---

## Risk Assessment Summary

### Strengths

| Area | Assessment |
|------|------------|
| Privacy compliance | Strong - comprehensive APP compliance with documentation |
| Data sovereignty | Strong - Australian data stored in Australia |
| Security certifications | Strong - ISO 27001, SOC 2 Type II |
| Clinical oversight | Moderate-Strong - founder is physician, integrated clinical team |
| Transparency | Strong - clear documentation of compliance posture |

### Areas to Monitor

| Area | Consideration |
|------|---------------|
| TGA regulation | TGA increasing scrutiny of AI scribes; may affect classification |
| My Health Record | No direct integration - may limit use cases |
| Feature expansion | Any diagnostic/treatment features would require regulatory review |
| External advisory | No formal external clinical advisory board identified |

### Recommendations for Due Diligence

1. **Request SOC 2 Type II report** - Verify current certification and scope
2. **Review clinical safety documentation** - Request hazard log summary
3. **Clarify data retention** - Confirm organizational settings meet requirements
4. **Evaluate TGA roadmap** - Understand plans if regulation changes
5. **Assess integration depth** - Evaluate PMS/EHR integration for specific workflows

---

## Sources

- [Heidi Health APP Compliance](https://www.heidihealth.com/en-au/compliance/app)
- [Heidi Health Privacy Policy](https://www.heidihealth.com/en-au/legal/privacy-policy)
- [Heidi Health Wikipedia](https://en.wikipedia.org/wiki/Heidi_Health)
- [TGA 'stepping up' regulation of AI scribes - Information Age](https://ia.acs.org.au/article/2025/tga--stepping-up--regulation-of-ai-scribes-in-healthcare.html)
- [Heidi Compliance FAQs](https://www.heidihealth.com/blog/heidi-compliance-lightning-faqs)
- [Heidi Safety Information](https://www.heidihealth.com/en-ca/safety)
- [Heidi Best Practice Integration](https://www.heidihealth.com/en-au/blog/best-practice-integration)
- [MediRecords Heidi Integration](https://www.pulseit.news/australian-digital-health/medirecords-integrates-heidi-health-ai-medical-scribe/)
- [UK NHS Guidance Compliance](https://www.heidihealth.com/uk/blog/uk-clinicians-using-heidi-satisfy-nhs-guidance)
- [Heidi Health Company Information](https://www.heidihealth.com/company)
- [Compliance Roadmap Article](https://www.heidihealth.com/blog/compliance-roadmap-as-differentiator)
- [Using AI Medical Scribes Safely](https://www.heidihealth.com/blog/using-ai-medical-scribes-safely)
- [Legally Healthy - Heidi Privacy Analysis](https://legallyhealthy.com.au/resources/protect-your-practice-patient-privacy/)
- [NHS DPIA for Heidi Health](https://highfieldsurgeryblackpool.nhs.uk/wp-content/uploads/2025/07/Heidi-Health-DPIA.pdf)

---

*Analysis compiled November 2025*
