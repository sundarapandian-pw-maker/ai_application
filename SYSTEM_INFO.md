# 🚗 SYSTEM_INFO — Autonomous Driver Monitoring System

> **AI Governance Profile** · Last Updated: June 2026
> This document provides a comprehensive description of the **Autonomous Driver Monitoring System** as assessed under the EU AI Act and GDPR framework. All fields are derived from the Full Assessment questionnaire (Discovery API dummy data).

---

## 1. System Identity & Ownership

| Field | Value |
|---|---|
| **System Name** | Autonomous Driver Monitoring System |
| **Owner / Contact** | [EMAIL_ADDRESS] |
| **Department** | Operations |
| **Vendor** | AutoSafe Technologies |
| **Vendor Type** | Third-Party |
| **Version** | 3.0 |
| **Lifecycle Stage** | Production |
| **Primary Language** | English |

### Explanation

The **Autonomous Driver Monitoring System** is a production-grade, third-party AI system deployed by the **Operations Department**, supplied by **AutoSafe Technologies** (version 3.0). The system is live and actively used in fleet or vehicle operations — not a prototype or pilot — meaning all governance, compliance, and risk controls apply with immediate and full legal force.

The system owner (`EMAIL ID`) bears responsibility for ensuring the system remains compliant with applicable regulations, maintaining documentation, and coordinating any incident response or audit requests.

---

## 2. AI Capabilities & Functionality

| Field | Value |
|---|---|
| **AI Type** | Computer Vision |
| **AI Capabilities** | Computer Vision, Biometric Recognition |
| **Primary Purpose** | Real-time driver fatigue detection and autonomous vehicle safety monitoring |
| **Output Type** | Automated Decisions, Risk Scores |

### Explanation

The system is classified as **Computer Vision AI** and employs **Biometric Recognition** technology to perform continuous, real-time monitoring of drivers while operating vehicles.

- **Computer Vision** enables the system to analyse live camera feeds and detect visual signals — including facial expressions, eye closure patterns, head position, and micro-gestures associated with fatigue or distraction.
- **Biometric Recognition** processes unique physiological characteristics of individual drivers, which is a highly regulated data category under GDPR Article 9.
- The system produces **Automated Decisions** (e.g., triggering alerts, restricting vehicle operation, escalating incidents) and **Risk Scores** (continuous fatigue or attentiveness ratings) without human review.

This combination makes the system safety-critical but also introduces high risks of discriminatory profiling, privacy violations, and overreach in workplace surveillance.

---

## 3. Human Interaction & Decision-Making

| Field | Value |
|---|---|
| **Interacts with People** | ✅ Yes |
| **Decision Mode** | Fully Automated |
| **Human Oversight** | ❌ None |

### Explanation

The **Autonomous Driver Monitoring System interacts directly with drivers** in real time. Critically, this system operates in **Fully Automated** mode with **no human oversight**, meaning:

- No human reviews the AI's assessments before they are acted upon.
- Automated risk scores and fatigue alerts can trigger operational consequences (e.g., vehicle slow-down, route changes, incident reports) without human approval.
- Drivers have no mechanism to contest or override decisions in real time.

> ⚠️ **This is a high-risk configuration.** Under the EU AI Act, fully automated systems operating in employment and critical infrastructure contexts with no human oversight are subject to the strictest obligations. The absence of any human-in-the-loop mechanism is a critical governance gap that must be remediated urgently.

---

## 4. High-Risk Classification Areas

The system operates in the following **EU AI Act high-risk domains**:

| # | High-Risk Area | Implication |
|---|---|---|
| 1 | **Critical Infrastructure** | Monitors vehicle operations; failures or errors could directly endanger lives on public roads |
| 2 | **Employee Monitoring** | Continuously tracks and scores employees (drivers) in their working environment; impacts employment conditions and dignity |

### Explanation

Both areas are explicitly listed in **Annex III of the EU AI Act** as high-risk application domains. Operating under even one of these categories mandates conformity assessments, technical documentation, human oversight, transparency obligations, and registration in the EU AI Act database.

This system falls under **both simultaneously**, which places it in the highest regulatory risk tier. Deployment without meeting these obligations exposes the organisation to enforcement action, regulatory fines, and civil liability.

---

## 5. Individual Profiling & Rights Impact

| Field | Value |
|---|---|
| **Profiles Individuals** | ✅ Yes |
| **Infers Emotions** | ✅ Yes |
| **Impacts Rights** | ✅ Yes |
| **Impact Type** | Safety impact |

### Explanation

- **Profiles Individuals**: The system continuously builds profiles of each driver — tracking fatigue patterns, reaction times, and behavioural trends over time. This is ongoing automated profiling in an employment context.
- **Infers Emotions**: The system infers cognitive and emotional states (alertness, drowsiness, stress) from biometric signals. Emotion inference in an employment/transport context is explicitly flagged as high-risk under the EU AI Act.
- **Impacts Rights**: The system's decisions carry **direct safety impact** — incorrect classifications could result in wrongful disciplinary action, unjustified operational restrictions, or — critically — failure to intervene when a driver is genuinely impaired, leading to accidents.

> ⚠️ Continuous biometric emotion inference of employees with no human oversight, in a safety-critical context, creates severe fundamental rights and occupational safety risks. A Data Protection Impact Assessment (DPIA) is legally mandatory under GDPR Article 35.

---

## 6. Personal Data Processing

### 6a. Types of Personal Data Processed

| Category | Data Types |
|---|---|
| **Standard Personal Data** | Name, Employee ID, Location |
| **Special Category (Sensitive) Data** | Biometric data, Health data |
| **Criminal & Offence Data** | Criminal records |

### Explanation

- **Standard personal data** (Name, Employee ID, Location) is regulated under GDPR Article 6 and requires a lawful basis (e.g., legitimate interest or contractual necessity in an employment context).
- **Biometric and Health data** are **Special Category data under GDPR Article 9**. Processing requires explicit consent or another Article 9(2) exception. In an employment context, consent is rarely freely given — meaning another specific exception must apply.
- **Criminal record data** falls under **GDPR Article 10**, which restricts processing to official authority or a specific legal basis. Including criminal history in a driver monitoring system requires a clear, documented legal mandate.

Processing all three tiers of data simultaneously — including biometric and criminal data about employees in a real-time monitoring system — demands the highest level of legal scrutiny, explicit privacy notices, and robust access controls.

---

### 6b. Data Subjects

The system processes data about the following categories of individuals:

| Data Subject | Notes |
|---|---|
| **Employees (Drivers)** | 🔴 **Heightened sensitivity** — employment context; power imbalance makes freely given consent legally questionable; occupational privacy rights apply |

> 🔴 **Processing biometric, health, and criminal data about employees in a workplace monitoring context** is one of the most heavily regulated scenarios under GDPR and national employment law. Workers' councils, trade unions, and national data protection authorities must typically be consulted before such systems are deployed.

---

### 6c. Data Sources

| Source | Risk Level |
|---|---|
| **Internal Systems** | Moderate — internal data flows, access control required |
| **Vehicle Sensors** | High — continuous real-time biometric capture; data minimisation principle requires careful scoping |

Sourcing data directly from **vehicle sensors** means the system is performing **continuous, non-consensual biometric surveillance** of employees while they work. This is a particularly sensitive collection mechanism — the driver cannot opt out while performing their job duties.

---

## 7. Data Processing Details

| Field | Value |
|---|---|
| **Data State** | Raw |
| **Processing Actions** | Analyse, Profile, Score |
| **Region** | EU |
| **Cross-Border Transfer** | ❌ No |
| **Used for Training** | ✅ Yes |
| **Retention Period** | 2 Years |

### Explanation

- **Raw data** is processed — biometric data is ingested directly from sensors without prior anonymisation or pseudonymisation, maximising privacy risk.
- **Analyse, Profile, Score** are all forms of automated processing that individually and collectively trigger GDPR Article 22 obligations around automated decision-making.
- **EU region** with **no cross-border transfer** is a positive finding — data does not leave the EU, reducing international transfer compliance burden.
- **Used for training**: Driver biometric and behavioural data is fed back into model training — this must be explicitly disclosed in privacy notices and is unlikely to be covered by the employment contract alone. A separate lawful basis is required.
- **2-year retention**: While defined (better than indefinite), 2 years for biometric and health data in an employment context may still exceed what is proportionate. Legal justification is required.

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
| **Non-EU Hosting** | Despite data being collected in the EU, it is hosted on a vendor cloud outside the EU. This constitutes an international data transfer under GDPR Chapter V and requires Standard Contractual Clauses or equivalent safeguards — despite no active cross-border transfer being declared. |
| **No Model Documentation** | The AI system lacks a model card or technical specification. This directly violates EU AI Act transparency requirements (Article 13) and makes independent safety auditing impossible for a system making real-time safety-critical decisions. |
| **No Explainability** | When a system scores a driver as "High Fatigue Risk", there is no mechanism to explain why. Drivers, unions, and regulators cannot understand, contest, or verify decisions — violating GDPR Article 22(3) and EU AI Act Article 13. |
| **No Logging** | Without logs, there is no audit trail of decisions made. In the event of an accident linked to a monitoring failure, forensic investigation is impossible. |
| **No Version Tracking** | Changes to the model cannot be traced. Safety regressions introduced by model updates cannot be detected or rolled back. |

> 🔴 In a **safety-critical, real-time biometric monitoring system** operating in an employment context, the absence of documentation, explainability, logging, and version tracking is not merely a compliance gap — it is an **operational safety risk**.

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

- **No legal review**: There is no documented confirmation that continuous biometric monitoring of employees is lawful under GDPR, national employment law, or applicable transport/safety regulations.
- **No DPIA**: A DPIA is legally mandatory under GDPR Article 35 given the combination of: biometric data, health data, criminal data, profiling, automated decisions, and employment context. Non-completion is an immediate regulatory violation.
- **No bias testing**: Computer Vision systems are well-documented to perform unequally across different demographic groups (particularly based on skin tone, age, gender). Without bias testing, the system may be systematically penalising certain driver groups — creating discrimination liability.
- **No incident response**: There is no plan for what happens if the system malfunctions during a critical driving situation, produces a false positive that grounds a driver, or suffers a data breach exposing biometric records.
- **No Vendor DPA**: A Data Processing Agreement with AutoSafe Technologies is legally required under GDPR Article 28. Without it, the organisation is in breach of its data controller obligations and bears full liability for any data misuse by the vendor.

---

## 10. Shadow AI Usage

| Field | Value |
|---|---|
| **Shadow AI Tools in Use** | None |
| **Company Data Entered into Shadow Tools** | ✅ Yes |

### Explanation

No additional unauthorised AI tools have been identified in use alongside this system. However, **company data has been entered into public AI tools** — indicating that employees are using external AI services (even if not specifically named) to process information related to their work.

This requires investigation to determine which tools are involved and what categories of data (potentially including driver records or operational data) have been shared with third-party AI providers outside the organisation's control.

> ⚠️ An acceptable use policy for AI tools must be established and enforced. Any external AI tool handling company operational or personal data must be assessed, contracted, and controlled.

---

## 11. Business Impact & Criticality

| Field | Value |
|---|---|
| **Business Criticality** | Mission Critical |
| **Business Impact if Fails** | Safety impact |

### Explanation

The system is rated **Mission Critical** — the organisation's fleet operations depend on it and failure directly disrupts business continuity.

The **impact type is "Safety impact"** — this is the most severe category. In an autonomous driver monitoring context, system failures can have direct physical safety consequences:

- A **false negative** (failing to detect an impaired driver) could result in a road accident causing injury or death.
- A **false positive** (wrongly scoring an alert driver as fatigued) could ground vehicles unnecessarily, impacting both business operations and driver livelihoods.
- A **data breach** exposing biometric and health data of drivers creates immediate regulatory, legal, and reputational consequences.

The combination of Mission Critical status and Safety impact means that any failure of this system carries both operational and human-safety consequences — placing this in the **absolute highest priority** category for risk remediation.

---

## 12. Risk Summary

| Risk Domain | Rating | Reason |
|---|---|---|
| EU AI Act Compliance | 🔴 **Critical** | High-risk system (Critical Infra + Employee Monitoring) with no conformity assessment, documentation, or oversight |
| GDPR Compliance | 🔴 **Critical** | Biometric + health + criminal data; no DPIA, no vendor DPA; employment context with continuous surveillance |
| Technical Governance | 🔴 **Critical** | No logging, no explainability, no version tracking, non-EU hosting for safety-critical biometric system |
| Data Ethics | 🔴 **Critical** | Emotion inference + biometric profiling of employees with no bias testing or contestation mechanism |
| Operational / Safety Risk | 🔴 **Critical** | Mission Critical + Safety Impact + no incident response plan |
| Shadow AI Risk | 🟠 **Medium** | No named tools, but company data confirmed entering public AI — requires investigation |

### Weighted Risk Score

| Component | Score | Weight | Contribution |
|---|---|---|---|
| AI Act Risk — `High Risk` | 4/5 | × 0.45 | 1.80 |
| GDPR Classification — `Criminal Data` | 5/5 | × 0.35 | 1.75 |
| Business Impact — `Safety impact` | 5/5 | × 0.20 | 1.00 |
| **Final Score** | | | **4.55 / 5.00 🔴 Red** |

**Combined Priority: CRITICAL**

---

## 13. Recommended Immediate Actions

1. **Halt or suspend deployment** until a legal basis for biometric and criminal data processing of employees is formally established and documented.
2. **Complete a DPIA** immediately — legally mandatory under GDPR Article 35 for this system profile. Must include a worker/union consultation step.
3. **Sign a Data Processing Agreement** with AutoSafe Technologies before any further personal data is processed under their system.
4. **Implement logging and audit trails** — especially for all automated decisions and risk score outputs that affect drivers.
5. **Conduct bias testing** of the Computer Vision model across all relevant driver demographic groups (skin tone, age, gender) before continued use.
6. **Implement explainability** — drivers must be able to understand why they received a particular score or alert, and must have a right to contest it.
7. **Conduct a legal review** covering GDPR Article 9 & 10, EU AI Act Annex III, national employment law, and transport safety regulations.
8. **Implement human oversight** — introduce a human review step before automated scores trigger any operational consequence for a driver.
9. **Resolve the non-EU hosting issue** — either migrate to EU-based infrastructure or establish appropriate Standard Contractual Clauses with AutoSafe Technologies.
10. **Investigate and control shadow AI usage** — identify which tools company data is being entered into and establish an AI acceptable use policy.

---

*This document was generated from the AI Governance Full Assessment questionnaire (Discovery API dummy data — Autonomous Driver Monitoring System profile). It should be reviewed by the Data Protection Officer (DPO), Legal Counsel, Works Council (if applicable), and the AI system owner.*
