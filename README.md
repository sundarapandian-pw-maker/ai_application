# 🚚 Predictive Vehicle Maintenance Platform — AI Governance Profile

> **Repository**: AI Governance Demo Data  
> **System**: Predictive Vehicle Maintenance Platform  
> **Framework**: EU AI Act (High Risk Annex III) & GDPR compliance profile  
> **Version**: 2.4 | **Lifecycle Stage**: Production | **Primary Language**: English

---

## ⚠️ System Identity, Context & Ownership

The system described in this repository is named the **Predictive Vehicle Maintenance Platform**. It operates within the organization's **Operations** department and is managed under the direct supervision of the fleet operations unit, with **fleet.ops@company.com** serving as the primary owner and contact address. 

The software itself is a **Third-Party** system sourced from the external vendor **FleetPredict AI**. It is currently deployed as version **2.4** and runs actively in our live **Production** environment. All documentation, system UI elements, and configuration outputs are prepared in the **English** language.

---

## ⚙️ AI Capabilities & Output Profile

This platform is classified under the **Predictive ML** AI type, employing advanced **Machine Learning** and **Predictive Analytics** to evaluate vehicles and operator habits. 

The primary purpose of the system is to predict vehicle component failures and optimize maintenance scheduling to reduce downtime and operational costs. The model processes telemetry, vibration, and operator performance data to output structured **Risk Scores** (related to vehicle wear and driver habits) and actionable maintenance **Recommendations** for dispatchers.

---

## 👥 Human Interaction & Automated Decisions

The platform **interacts with people** by tracking driver telematics and presenting recommendations to fleet dispatchers. 

The system operates in a **Fully Automated** decision mode with **None** (no human oversight) integrated into the core alert-routing loop. Risk levels and component warning scores automatically trigger vehicle bookings, operational restrictions, and safety alerts without requiring any manual review or secondary approval by a fleet manager.

---

## ⚖️ High-Risk Triggers & Rights Impact (EU AI Act)

Under the EU AI Act framework, this system qualifies as a High-Risk AI System. It is actively deployed in two Annex III high-risk domains:
1. **Critical Infrastructure**: Since it controls scheduling and maintenance for transport infrastructure.
2. **Employee Monitoring**: Since it tracks and profiles employees (drivers).

Because the system **profiles individuals** (drivers) to determine risk and **infers emotions** (detecting behavioral states like stress and fatigue from telemetry/video patterns), it directly **impacts fundamental rights**. Due to the real-world navigation and scheduling risks, the official impact type is designated as a **Safety impact**.

---

## 🔒 GDPR Data Protection Profile

From a data protection perspective, the platform processes multiple categories of personal data. The standard personal data collected consists of the driver's **Name**, **Employee ID**, and real-time GPS **Location**. 

Under GDPR Article 9, it also processes sensitive category data, specifically **Biometric** and **Health** indicators collected via cabin telematics to evaluate alertness. Under Article 10, the platform processes **Criminal Record** information to verify driver clearances.

The data subjects involved in this system are solely company **Employees**. The data sources feeding the platform are **Internal Systems** and a **Third-party API**. All data is collected in its **Raw** state and subjected to three main processing actions: **Analyse**, **Profile**, and **Score**. All operations occur within the **EU** region, and there is no **cross-border transfer** of personal data (cross_border_transfer is false). The processed data is **used for training** the models, and all logs and personal records are subject to a **3 Years** retention period.

---

## 🛠️ Technical Controls & Infrastructure

The platform is hosted on a **Vendor Cloud non-EU** infrastructure, indicating that telemetry and profile database hosting occurs outside the EEA. 

Regarding technical controls, the model is **No** (not documented), meaning no model card or conformity file is available. The system's explainability score is **No**, operating as a black box. System logging is **No** (logging_enabled is false/No), and there is no **version tracking** active in the production pipeline.

---

## 📋 Compliance Status & Governance Exposure

An audit of the system reveals significant governance gaps. Legal review is **No** (not completed), and a Data Protection Impact Assessment (DPIA) is **No** (not completed). 

The predictive models are **No** (not tested for bias), and there is **No** (no incident response plan) for AI failures. The company has **No** (not signed a Vendor DPA) under Article 28 GDPR with the vendor.

There are **None** (no shadow AI tools in use) by the operations team for this platform. However, company data has been entered into the vendor's public tools, so **company data entered** is true (Yes). 

The system's business criticality is rated as **Mission Critical**, and its business impact is classified as a **Safety impact** due to the potential consequences of fleet or component warning failures.

---
