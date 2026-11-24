# Botium Toys — Security Controls & Compliance Assessment

**Academic cybersecurity audit case study**  
**Author:** Oscar Augusto Hernandez Romero  
**Portfolio edition:** November 2026

> This is an educational portfolio artifact based on the fictional Botium Toys case from the Google Cybersecurity Professional Certificate, not a live-company audit or legal compliance determination.

## Executive summary

The case scenario reports a security risk score of **8/10**. The completed course checklist indicates **6 of 14** security safeguards present and **8 of 14** absent. Significant areas of exposure include excessive employee access to sensitive data, absence of encryption for cardholder information, lack of disaster recovery and backups, and missing intrusion detection. Findings are derived from documented training artifacts; they were not verified by live technical tests.

## Assessment scope

The scenario covers employee devices, organizational equipment, internal networks, IT services and systems, legacy infrastructure, online and on-site retail operations, and sensitive company and customer data.

## Findings and proposed actions

| ID | Priority* | Finding | Evidence from training material | Proposed action |
| --- | --- | --- | --- | --- |
| F01 | High | Excessive sensitive-data access | Broad access to PII/SPII/cardholder data; least privilege and separation of duties are absent | Apply role-based restrictions and segregation of duties |
| F02 | High | Missing encryption | Credit-card data is processed or stored without encryption | Encrypt sensitive data in transit and at rest; establish key management |
| F03 | High | No backup/DR plan | No critical-data backups or disaster recovery plan | Deploy protected backups, restore testing and recovery procedures |
| F04 | High | Missing intrusion detection | IDS is not installed | Implement detection coverage and alert escalation |
| F05 | Medium | Weak password governance | Nominal password policy; no centralized password manager | Strengthen policy and centralize credential management |
| F06 | Medium | Inadequate asset and data inventory | Weak asset management and missing inventory/classification | Complete inventory and classify sensitive assets |
| F07 | Medium | Inconsistent control documentation | Brief and checklist disagree about some integrity/privacy controls | Validate evidence and reconcile record differences |

\* Priority levels are proposed for this portfolio case study, not scores from an independent assessment. The **8/10** overall risk score comes from the course brief.

## Control status overview

The checklist marks these safeguards **present**: firewall, antivirus, manual monitoring of legacy systems, physical locks, CCTV, and fire detection/prevention.

It marks these **absent**: least privilege, disaster recovery plans, effective password policies, separation of duties, IDS, backups, encryption and centralized password management.

The compliance-related checklist includes:

- **PCI DSS:** 0 of 4 course criteria marked Yes.
- **GDPR:** 1 of 4 criteria marked Yes (breach notification plan).
- **SOC type 1 / type 2:** 0 of 4 criteria marked Yes.

These scores summarize checklist answers, **not** actual conformance with regulations or audit attestation standards.

### Evidence quality notes

The course brief describes existing data-integrity and some privacy processes, while the completed checklist marks related SOC and GDPR criteria as absent. It also mentions a nominal password policy, whereas the checklist marks password policies as No. Without additional validation, the report does not resolve these contradictions into a single definitive control status.

## Proposed 90-day improvement roadmap

### Days 1–30 — Reduce immediate exposure

1. Restrict access to sensitive data according to job need; review privileged roles.
2. Plan encryption at rest and in transit for customer and payment information.
3. Assign ownership for the asset inventory and remediation actions.

### Days 31–60 — Improve resilience and detection

1. Implement backup schedules, protected storage and restore tests.
2. Pilot IDS monitoring, define alert triage, and document escalation steps.
3. Strengthen password standards and centralize credential management.

### Days 61–90 — Validate and sustain

1. Classify sensitive data, critical systems and assets.
2. Reassess controls and organize supporting evidence against applicable criteria.
3. Establish repeatable legacy-system maintenance reviews.

## Method, evidence, and limitations

This assessment used a documentation-only review of:

- **[S1]** *Botium Toys: Scope, goals, and risk assessment report* (provided training scenario, 3 pages).
- **[S2]** *Controls and compliance checklist* (completed academic assessment, 3 pages).

No live systems, user accounts, production logs, security devices, interviews or legal records were accessed or independently validated. The report's risk prioritization, remediation sequence and 90-day roadmap are proposals, not verified remediation work.

## Next practical steps

A future technical companion project could validate similar access controls, alert detection, log analysis and backup-restore processes in an isolated personal lab. Evidence could include test steps, sanitized log samples, screenshots and a lessons-learned record.
