# 🤖 SYSTEM_INFO — Smart Contract Auditor

> **AI Governance Profile** · Last Updated: June 2026
> This document provides a comprehensive description of the **Smart Contract Auditor** AI system as assessed under the EU AI Act and GDPR framework. All fields are derived from the Full Assessment questionnaire.

---

## 1. System Identity & Ownership

| Field | Value |
|---|---|
| **System Name** | Smart Contract Auditor |
| **Owner / Contact** | sundarapandian****@gmail.com |
| **Department** | Legal |
| **Vendor** | AuditAI Corp |
| **Vendor Type** | SaaS (Software as a Service) |
| **Version** | 2.1 |
| **Lifecycle Stage** | Production |
| **Primary Language** | English |

### Explanation

The **Smart Contract Auditor** is a production-grade SaaS AI system deployed by the **Legal Department**, operated by **AuditAI Corp** (version 2.1). The system is actively in use — not a prototype or pilot — meaning all governance, compliance, and risk controls apply immediately and with full legal force.


---

## 2. AI Capabilities & Functionality

| Field | Value |
|---|---|
| **AI Type** | Generative AI |
| **AI Capabilities** | Generative AI, NLP (Natural Language Processing) |
| **Primary Purpose** | Security Auditing |
| **Output Type** | Text |

### Explanation

The system is classified as **Generative AI** and leverages **Natural Language Processing (NLP)** to perform automated security auditing of smart contracts. It reads, interprets, and generates detailed textual analysis and audit reports.

- **Generative AI** means the system can produce novel text, summaries, and recommendations — not just retrieve pre-written answers.
- **NLP** enables the system to understand legal and technical language in contracts and code.
- The **output is purely text-based**: audit findings, risk ratings, legal observations, and recommendations are all delivered as written reports.

This combination makes the system powerful for legal and security teams but also introduces risks of hallucination, bias in reasoning, and overconfidence in generated outputs.

---

## 3. Human Interaction & Decision-Making

| Field | Value |
|---|---|
| **Interacts with People** | ✅ Yes |
| **Decision Mode** | Fully Automated |
| **Human Oversight** | ❌ None |

### Explanation

The **Smart Contract Auditor interacts directly with people** — users receive AI-generated outputs that influence their actions. Critically, this system operates in **Fully Automated** mode with **no human oversight**, meaning:

- No human reviews the AI's output before it is delivered.
- No human can intervene to block, modify, or approve decisions.
- Users must rely entirely on the system's own accuracy and judgment.

> ⚠️ **This is a high-risk configuration.** Under the EU AI Act, systems making consequential automated decisions with no human oversight face strict obligations. The absence of any human-in-the-loop mechanism is a significant governance gap that must be addressed.

---

## 4. High-Risk Classification Areas

The system operates in the following **EU AI Act high-risk domains**:

| # | High-Risk Area | Implication |
|---|---|---|
| 1 | **Critical Infrastructure** | AI decisions could impact essential services or safety-critical systems |
| 2 | **Law Enforcement** | Outputs may influence legal proceedings, investigations, or enforcement actions |
| 3 | **Employee Monitoring** | System may process data about employees and impact their employment conditions |

### Explanation

All three of these areas are explicitly listed in **Annex III of the EU AI Act** as high-risk application domains. A system that falls under even one of these categories is subject to mandatory conformity assessments, technical documentation, transparency requirements, and human oversight obligations.

This system falls under **all three simultaneously**, which places it in the highest regulatory risk tier. Deployment without meeting these obligations exposes the organisation to enforcement action, fines, and legal liability.

---

## 5. Individual Profiling & Rights Impact

| Field | Value |
|---|---|
| **Profiles Individuals** | ✅ Yes |
| **Infers Emotions** | ✅ Yes |
| **Impacts Rights** | ✅ Yes |
| **Impact Type** | Legal impact |

### Explanation

- **Profiles Individuals**: The system builds or contributes to profiles about specific people, combining data points to draw inferences about their behaviour, attributes, or risk.
- **Infers Emotions**: The system attempts to interpret emotional states from data — a capability heavily regulated under GDPR Article 9 and flagged as high-risk under the EU AI Act when used in certain contexts (e.g., employment, law enforcement).
- **Impacts Rights**: The system's outputs carry **legal impact** — meaning its findings or classifications can directly affect legal rights, obligations, or outcomes for the individuals or entities it processes data about.

> ⚠️ Emotion inference and individual profiling in a legal context, combined with no human oversight, creates a significant fundamental rights risk. A Data Protection Impact Assessment (DPIA) is mandatory under GDPR Article 35.

---

## 6. Personal Data Processing

### 6a. Types of Personal Data Processed

| Category | Data Types |
|---|---|
| **Standard Personal Data** | Name, Email Address, IP Address |
| **Special Category (Sensitive) Data** | Health data, Biometric data |
| **Criminal & Offence Data** | Criminal records |

### Explanation

- **Standard personal data** (Name, Email, IP) is regulated under GDPR and requires a lawful basis for processing.
- **Health and Biometric data** are **Special Category data under GDPR Article 9**. Processing these requires explicit consent or another specific Article 9(2) exception, and carries much stricter obligations.
- **Criminal record data** falls under **GDPR Article 10**, which restricts its processing to official authority or specific legal basis. This is among the most sensitive data categories in EU law.

Processing all three tiers of data simultaneously demands a comprehensive legal basis framework, explicit privacy notices, and robust access controls.

---

### 6b. Data Subjects

The system processes data about the following categories of individuals:

| Data Subject | Notes |
|---|---|
| **Employees** | Employment-related data processing; heightened sensitivity in workplace context |
| **Customers** | Commercial relationship data; consent and contractual basis apply |
| **Children** | 🔴 **Highest risk** — GDPR Article 8 applies; parental consent required under 16 (or lower national threshold); prohibited for certain automated decision-making |

> 🔴 **Processing data about children** is the most regulated scenario under GDPR. Automated profiling or decision-making affecting children is prohibited or severely restricted. Immediate review is required.

---

### 6c. Data Sources

| Source | Risk Level |
|---|---|
| **Internal Systems** | Moderate — internal data flows, access control required |
| **Public Web** | High — unknown provenance, potential copyright/privacy issues, no consent from individuals whose data is scraped |

Sourcing data from the **public web** means the system may be ingesting personal data without the knowledge of the individuals concerned. This is particularly problematic when combined with profiling and special category data processing.

---

## 7. Data Processing Details

| Field | Value |
|---|---|
| **Data State** | Raw |
| **Processing Actions** | Analyse, Profile, Score |
| **Region** | Global |
| **Cross-Border Transfer** | ✅ Yes |
| **Used for Training** | ✅ Yes |
| **Retention Period** | Indefinite |

### Explanation

- **Raw data** is processed — meaning data is ingested without prior anonymisation or pseudonymisation, increasing privacy risk.
- **Analyse, Profile, Score** are all forms of automated processing that individually and collectively trigger GDPR obligations around automated decision-making (Article 22).
- **Global operations** with **cross-border data transfers** out of the EU/EEA require appropriate safeguards (Standard Contractual Clauses, Adequacy Decisions, or Binding Corporate Rules).
- **Used for training**: Personal data is fed back into model training — this must be disclosed in privacy notices and may require separate consent.
- **Indefinite retention** directly violates GDPR's **storage limitation principle (Article 5(1)(e))**, which requires data to be kept only as long as necessary. This must be remediated immediately with a defined retention schedule.

---

## 8. Technical Posture & Infrastructure

| Field | Value |
|---|---|
| **Hosting Location** | Vendor Cloud — Non-EU |
| **Model Documented** | ❌ No |
| **Explainability** | ❌ No |
| **Logging Enabled** | ❌ No |
| **Version Tracking** | ❌ No |

### Explanation

| Concern | Detail |
|---|---|
| **Non-EU Hosting** | Data is stored and processed outside the EU. This constitutes an international data transfer and requires legal safeguards under GDPR Chapter V. |
| **No Model Documentation** | The AI system lacks a model card or technical specification. This violates EU AI Act transparency requirements (Article 13) and makes independent auditing impossible. |
| **No Explainability** | The system cannot explain how it reaches its conclusions. Users cannot understand, contest, or verify decisions — violating GDPR Article 22(3) and EU AI Act Article 13. |
| **No Logging** | Without logs, there is no audit trail of inputs, outputs, or decisions. This prevents forensic investigation, regulatory audits, and accountability. |
| **No Version Tracking** | Changes to the model cannot be traced. There is no way to determine when behaviour changed, or to rollback to a prior state if issues are discovered. |

> 🔴 This combination — no documentation, no explainability, no logging, no version tracking, hosted outside the EU — represents a **critical technical governance failure**.

---

## 9. Compliance & Legal Controls

| Control | Status |
|---|---|
| Legal review completed | ❌ No |
| DPIA completed | ❌ No |
| Bias testing conducted | ❌ No |
| Incident response plan | ❌ No |
| Vendor Data Processing Agreement (DPA) | ❌ No |

### Explanation

**Every single compliance control is missing.** This is the most serious finding in this assessment:

- **No legal review**: There is no confirmation that the system's use is lawful under applicable regulations (GDPR, EU AI Act, national law).
- **No DPIA**: A DPIA is legally mandatory under GDPR Article 35 given the combination of high-risk processing (profiling, special category data, children's data, automated decision-making). Non-completion is an immediate regulatory violation.
- **No bias testing**: Without bias testing, the system may be making discriminatory decisions in legal and employment contexts — creating both ethical harm and legal liability.
- **No incident response**: There is no plan for what happens if the system produces harmful outputs, suffers a data breach, or is found to be non-compliant.
- **No Vendor DPA**: A Data Processing Agreement with the vendor (AuditAI Corp) is legally required under GDPR Article 28. Without it, the organisation is in breach of its controller obligations.

---

## 10. Shadow AI Usage

| Field | Value |
|---|---|
| **Shadow AI Tools in Use** | ChatGPT, GitHub Copilot |
| **Company Data Entered into Shadow Tools** | ✅ Yes |

### Explanation

In addition to the official Smart Contract Auditor system, employees are using **unauthorised AI tools (ChatGPT and GitHub Copilot)** — and are **entering company data into these tools**.

This represents a significant **data leakage risk**:
- Company confidential data, potentially including personal data and special category data, may be shared with third-party AI providers without legal basis, privacy notices, or data processing agreements.
- Outputs from these tools may be incorporated into work products without disclosure.
- These tools are beyond the organisation's control, consent framework, or security perimeter.

> ⚠️ An acceptable use policy for AI tools must be established and enforced. Employees must be trained. Shadow AI usage must be formally assessed and either approved with controls, or prohibited.

---

## 11. Business Impact & Criticality

| Field | Value |
|---|---|
| **Business Criticality** | Mission Critical |
| **Business Impact** | Safety impact |

### Explanation

The system is rated **Mission Critical**, meaning the organisation's core operations depend on it — failure or unavailability directly disrupts business continuity.

The **impact type is "Safety impact"** — the system's outputs can affect the safety of individuals. In a legal auditing context, an incorrect finding could:
- Lead to a legally flawed contract being approved.
- Result in wrongful accusations or missed criminal behaviour.
- Cause financial or physical harm to individuals whose data was misprocessed.

The combination of Mission Critical status and Safety impact means that any failure of this system carries both operational and human-safety consequences — elevating this to the **highest priority** for remediation.

---

## 12. Risk Summary

| Risk Domain | Rating | Reason |
|---|---|---|
| EU AI Act Compliance | 🔴 **Critical** | High-risk system with no conformity assessment, documentation, or oversight |
| GDPR Compliance | 🔴 **Critical** | No DPIA, no DPA, indefinite retention, special category + children's data |
| Technical Governance | 🔴 **Critical** | No logging, no explainability, no version tracking, non-EU hosting |
| Data Ethics | 🔴 **High** | Emotion inference, individual profiling, no bias testing |
| Operational Risk | 🟠 **High** | Mission critical with no incident response plan |
| Shadow AI Risk | 🟠 **High** | Uncontrolled tools with company data exposure |

---

## 13. Recommended Immediate Actions

1. **Halt automated decision-making** affecting children until legal basis is established and human oversight is implemented.
2. **Complete a DPIA** immediately — this is a legal requirement, not optional.
3. **Sign a Data Processing Agreement** with AuditAI Corp before any further personal data is shared.
4. **Implement logging and audit trails** across all system inputs and outputs.
5. **Define and enforce a data retention policy** — indefinite retention must be replaced with a justified schedule.
6. **Conduct a legal review** covering GDPR, EU AI Act Annex III, and any applicable national law.
7. **Implement human oversight** — introduce a human review step before AI audit findings are acted upon.
8. **Ban or control shadow AI usage** — establish an AI acceptable use policy and enforce it.
9. **Request model documentation and explainability reports** from AuditAI Corp.
10. **Develop an incident response plan** covering AI-specific failure scenarios.

---

*This document was generated from the AI Governance Full Assessment questionnaire. It should be reviewed by the Data Protection Officer (DPO), Legal Counsel, and the AI system owner.*
