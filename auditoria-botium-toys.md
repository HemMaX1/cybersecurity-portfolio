# Portfolio — Security Audit: Botium Toys

**Author:** Jassiel Romano Gonzalez
**Course:** Google Cybersecurity Certificate (INROADS scholarship), Course 2: Play It Safe — Manage Security Risks, Module 2
**Framework:** NIST Cybersecurity Framework (CSF)
**Completed:** November 2026
**Original file:** `Auditor_a_Botium_Toys_-_Jassiel_Romano_Gonzalezpliance_checklist_0_9rhm.pdf` (keep as backup — this entry is the portfolio version)

---

## Security Audit — Botium Toys

**Role:** Student auditor (Google Cybersecurity Certificate, Course 2, Module 2)
**Framework:** NIST Cybersecurity Framework (CSF)
**Scope:** Controls assessment and compliance check for Botium Toys' environment — office, storefront, warehouse, and online store — covering customer payment data, customer personal data (PII/SPII), and business with customers in the European Union.

### Overview

Botium Toys is a small U.S. business that develops and sells toys. It has one physical location (office, storefront, and warehouse) and a growing online store with customers in the U.S. and abroad. The IT department asked for an internal audit to improve its security posture, identify risks to critical assets, and check compliance for online payments and business in the European Union.

### Goals of the audit

- Improve Botium Toys' security posture using the NIST Cybersecurity Framework.
- Give mitigation recommendations for the risks found.
- Identify the compliance regulations Botium Toys must follow (PCI DSS, GDPR, SOC 1 / SOC 2).

### Framework used — NIST CSF, 5 functions

Identify · Protect · Detect · Respond · Recover

### Controls assessment

For each control, I checked: does Botium Toys currently have this control in place? (Yes / No)

| Control | In place? | What I found |
|---|---|---|
| Least privilege | No | All employees have access to internal data, including credit card data and customers' PII/SPII. |
| Disaster recovery plans | No | There are no disaster recovery plans. |
| Password policies | Partial | The current password policy is minimal. |
| Separation of duties | No | All employees have access to internal data; duties are not separated. |
| Firewall | Yes | Botium Toys has a firewall in place. |
| Intrusion detection system (IDS) | No | There is a firewall and antivirus, but no IDS. |
| Backups | No | There are currently no backups. |
| Antivirus software | Yes | Botium Toys has antivirus software in place. |
| Manual monitoring, maintenance, and intervention for legacy systems | Partial | Legacy systems are monitored, but without a regular schedule. |
| Encryption | No | Credit card data is not encrypted when stored, processed, or transmitted. |
| Password management system | No | There is no centralized password management system. |
| Locks (offices, storefront, warehouse) | Not specified in my audit | — |
| Closed-circuit television (CCTV) surveillance | Not specified in my audit | — |
| Fire detection / prevention (fire alarm, sprinkler system) | Not specified in my audit | — |

### Compliance checklist

| Regulation | Best practice | Does Botium Toys follow it? |
|---|---|---|
| PCI DSS | Only authorized users have access to customers' credit card information. | No — all employees have access to it. |
| PCI DSS | Credit card information is stored, accepted, processed, and transmitted internally, in a secure environment. | No — card data is not encrypted. |
| PCI DSS | Implement data encryption procedures to better secure credit card transaction touchpoints and data. | No — no encryption procedures in place. |
| PCI DSS | Adopt secure password management policies. | No — password policy is minimal, no centralized system. |
| GDPR | E.U. customers' data is kept private/secured. | No — all employees can access customers' PII/SPII. |
| GDPR | There is a plan in place to notify E.U. customers within 72 hours if their data is compromised / there is a breach. | Not specified in my audit |
| GDPR | Ensure data is properly classified and inventoried. | Not specified in my audit |
| GDPR | Enforce privacy policies, procedures, and processes to properly document and maintain data. | Not specified in my audit |
| SOC 1 / SOC 2 | User access policies are established. | No — no least privilege; all employees have access. |
| SOC 1 / SOC 2 | Sensitive data (PII/SPII) is confidential/private. | No — all employees can access it. |
| SOC 1 / SOC 2 | Data integrity ensures the data is consistent, complete, accurate, and has been validated. | Not specified in my audit |
| SOC 1 / SOC 2 | Data is available to individuals authorized to access it. | Not specified in my audit |

### Key findings and recommendations

**Risk score: 8/10 (high).** Botium Toys has a high risk score because it does not have adequate controls in place and is not fully compliant with PCI DSS and GDPR. Each finding below contributes to that overall score.

| # | Finding | Recommendation |
|---|---|---|
| 1 | All employees have access to internal data, including credit card data and customers' PII/SPII. No least privilege, no separation of duties. | Implement least privilege and separation of duties (administrative / technical). Only authorized users should have access to sensitive data. This will help comply with PCI DSS and SOC. |
| 2 | Credit card data is not encrypted when stored, processed, or transmitted. | Implement encryption (technical). Implement data encryption protocols to protect confidentiality and comply with PCI DSS. |
| 3 | Botium Toys has a firewall and antivirus, but no intrusion detection system. | Install an intrusion detection system (IDS) (technical — detective). An IDS will help detect intrusions and suspicious activity. |
| 4 | There are currently no backups or disaster recovery plans. | Implement backups and disaster recovery plans (technical — corrective). Implement regular backups and a disaster recovery plan to ensure business continuity if critical operations are interrupted. |
| 5 | The current password policy is minimal and there is no centralized password management system. | Implement a centralized password management system and enforce strong password policies (technical / administrative). Enforce strong passwords (at least 8 characters, combination of letters, numbers, and special characters) and implement a centralized system to reduce password reset tickets and improve security. |
| 6 | Legacy systems are monitored, but without a regular schedule. | Implement a regular schedule for legacy system maintenance (administrative). Create a regular schedule for monitoring, maintenance, and intervention. |

These actions will reduce the risk score, improve the security posture, and help Botium Toys comply with PCI DSS, GDPR, and SOC Type 1 and Type 2.

**Prepared by: Jassiel Romano Gonzalez — Google Cybersecurity Certificate**

---

### What this shows

- I can run a security audit with a real framework (NIST CSF), not just describe it.
- I can evaluate controls, check compliance (PCI DSS, GDPR, SOC), and write findings with recommendations.
- I did this audit in English.
