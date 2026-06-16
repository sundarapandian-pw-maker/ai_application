# 🚚 SYSTEM_INFO — Predictive Vehicle Maintenance Platform



## 1. System Identity & Ownership

The system under evaluation is formally named the **Predictive Vehicle Maintenance Platform**. It has been deployed within the company's **Operations** department to manage fleet efficiency. The system is managed and owned by the fleet operations team, with the primary contact point designated as **fleet.ops@company.com**.

This platform is a **Third-Party** software solution developed and supported by the vendor **FleetPredict AI**. The current active deployment in our live environment is version **2.4**, which is fully in the **Production** lifecycle stage. All system logs, user interfaces, configuration consoles, and model outputs are set to the **English** language.

---

## 2. AI Capabilities & Functionality

Technically, the system is classified under the **Predictive ML** AI type. It incorporates advanced **Machine Learning** and **Predictive Analytics** capabilities to monitor vehicle states in real time. 

The primary purpose of the system is to predict vehicle component failures and optimize maintenance scheduling to reduce downtime and operational costs. To achieve this, the system processes continuous telematics streams and outputs structured **Risk Scores** and maintenance **Recommendations** directly to the logistics dispatch database.

---

## 3. Human Interaction & Decision-Making

The platform actively **interacts with people**, specifically the drivers operating company vehicles and the dispatch team. The system operates under a **Fully Automated** decision mode. 

There is **None** (no human oversight) integrated into the core decision loop. The AI engine automatically generates alerts, rates driver risk profiles, and adjusts maintenance schedules. If a vehicle or driver receives a high-risk score, the system automatically schedules maintenance or logs warnings without requiring any human operator review or manual override.

---

## 4. High-Risk Classification (EU AI Act)

Under the European Union AI Act, this deployment qualifies as a High-Risk AI System. It is deployed across two Annex III high-risk domains:
1. **Critical Infrastructure**: As it controls and schedules the maintenance of logistics transport networks.
2. **Employee Monitoring**: As it continuously tracks, profiles, and evaluates driver performance.

Because the system **profiles individuals** (employees/drivers) and **infers emotions** (using biometric sensors to determine driver fatigue, stress, and behavioral states), it directly **impacts fundamental rights**. Given the automated routing and scheduling of heavy vehicles, the official impact type is designated as a **Safety impact**.

---

## 5. Personal Data & GDPR Compliance

The system processes personal data at various levels of sensitivity. The standard personal data categories collected are the driver's **Name**, **Employee ID**, and real-time **Location** coordinates.

Additionally, the system processes special category data under GDPR Article 9, specifically **Biometric** and **Health** data derived from cabin cameras and wearability sensors that detect driver alertness. It also processes Article 10 criminal data, specifically the driver's **Criminal Record** history, to evaluate insurance risk and safety clearance.

The data subjects involved in this processing are solely company **Employees**. The data sources feeding the system include **Internal Systems** (HR databases) and a **Third-party API** (telematics and fleet sensors). The collected telemetry is processed in its **Raw** state. The primary processing actions performed on this data are to **Analyse**, **Profile**, and **Score** driver profiles. All operations take place in the **EU** region, and there is no **cross-border transfer** of personal data (it remains within the region). However, the collected operational data is **used for training** purposes by the model, and all records are subject to a **3 Years** retention period.

---

## 6. Technical Controls & Infrastructure

The infrastructure hosting this system is located in a **Vendor Cloud non-EU** environment, meaning data is stored outside the European Economic Area. 

From a technical governance perspective, the model is **No** (not documented), meaning there is no official model card or conformity documentation. The system's explainability posture is rated **No**, as it operates as a black box with no explanation provided for its risk scores. Furthermore, system logging is **No** (disabled), and there is no **version tracking** active for the models deployed in the production environment.

---

## 7. Governance Controls & Risk Exposure

The system has not been subject to standard compliance checks. Legal review has **No** (not been completed), and a Data Protection Impact Assessment (DPIA) is **No** (not completed), despite being legally mandatory for this data profile. 

No **bias testing** has been performed on the predictive algorithms to check for discrimination. Additionally, there is **No** (no active incident response plan) for AI-specific failures, and the company has **No** (not signed a Vendor DPA) under Article 28 GDPR with FleetPredict AI.

There are **None** (no shadow AI tools in use) by the team for this platform. However, company data has been entered into the vendor's public tools, so **company data entered** is true. 

The system's business criticality is rated as **Mission Critical**, and its business impact is classified as a **Safety impact** due to the potential consequences of a fleet navigation or component warning failure.

---

