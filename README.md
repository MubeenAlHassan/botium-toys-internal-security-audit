# Botium Toys — Internal IT Security Audit & Compliance Assessment 🛡️

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Audit-blue)
![Compliance](https://img.shields.io/badge/Compliance-Assessment-brightgreen)
![NIST CSF](https://img.shields.io/badge/Framework-NIST%20CSF-orange)
![PCI-DSS](https://img.shields.io/badge/Standard-PCI--DSS-yellow)
![GDPR](https://img.shields.io/badge/Regulation-GDPR-blueviolet)

## 📋 Executive Summary
Botium Toys is a growing U.S.-based toy retailer expanding its operations from a single physical storefront into the international e-commerce market. This rapid growth has placed significant pressure on the IT infrastructure, exposing the business to potential compliance violations and security vulnerabilities. This project involves a comprehensive internal IT security audit designed to evaluate the current security posture, ensure business continuity, and align operations with critical regulatory requirements (PCI DSS, GDPR) and industry best practices (NIST CSF).

## 🎯 Audit Scope & Objectives
The scope of this audit encompasses the IT infrastructure supporting Botium Toys' online and physical operations.
- **Target Systems:** E-commerce platform, internal network, point-of-sale (POS) systems, and inventory management servers.
- **Data Assets:** Customer Personally Identifiable Information (PII), payment card data, employee records, and proprietary business data.
- **Objectives:** 
  - Identify existing vulnerabilities and gaps in security controls.
  - Assess compliance with PCI DSS for payment processing and GDPR for E.U. customer data privacy.
  - Develop a prioritized remediation roadmap to mitigate identified risks and ensure business continuity.

## 📊 Security Frameworks & Compliance Checklist
The following table summarizes the assessment of current security controls mapped against relevant frameworks and regulations.

| Control / Practice | Framework / Standard | Status | Description |
| :--- | :--- | :---: | :--- |
| **Principle of Least Privilege** | NIST CSF (PR.AC) | ❌ Missing | Access controls are not strictly enforced based on roles. |
| **Firewall** | NIST CSF / PCI DSS | ✅ Present | Network perimeter is protected by an active firewall. |
| **Intrusion Detection System (IDS)** | NIST CSF (DE.AE) | ❌ Missing | No system in place to detect unauthorized network access. |
| **Data Encryption (At Rest/In Transit)** | PCI DSS / GDPR | ❌ Missing | Sensitive customer and payment data lacks adequate encryption. |
| **Separation of Duties** | SOC 1/2 | ❌ Missing | Critical IT functions are concentrated, increasing insider risk. |
| **Disaster Recovery / Backups** | NIST CSF (RC.RP) | ❌ Missing | No formalized plan or regular backups to ensure business continuity. |
| **Breach Notification Policy** | GDPR | ❌ Missing | Lack of procedures for timely notification of data breaches. |
| **Data Classification** | GDPR / NIST CSF | ❌ Missing | Data is not categorized by sensitivity level. |

## ⚠️ Risk Assessment & Vulnerability Analysis
The audit identified five critical risk areas that require immediate attention to prevent operational disruption and regulatory penalties:

1. **Unencrypted Sensitive Data:** The absence of encryption for data at rest and in transit severely compromises payment card information and customer PII, leading to direct PCI DSS and GDPR violations.
2. **Lack of Intrusion Detection System (IDS):** Without an IDS, the network is highly vulnerable to undetected malicious activity and prolonged unauthorized access.
3. **Absent Disaster Recovery Plan:** The lack of a formal disaster recovery strategy and regular backups puts the organization at high risk of prolonged downtime and data loss in the event of a cyberattack or system failure.
4. **GDPR Non-Compliance:** The absence of data classification, breach notification procedures, and strict access controls exposes the company to significant fines as it expands into the European market.
5. **Lack of Separation of Duties:** Concentrated IT privileges increase the risk of insider threats and accidental misconfigurations without adequate oversight.

## 🚀 Prioritized Remediation Roadmap
To address the identified vulnerabilities and align with compliance standards, the following phased remediation plan is recommended:

### Phase 1: Immediate Priority (0-30 Days)
- **Implement Data Encryption:** Deploy strong encryption protocols for all payment processing and sensitive customer data both in transit (TLS) and at rest.
- **Establish Access Controls:** Enforce the Principle of Least Privilege and implement Separation of Duties across all IT systems and databases.

### Phase 2: High Priority (30-90 Days)
- **Deploy an IDS/IPS:** Install and configure an Intrusion Detection/Prevention System to monitor network traffic for malicious activity.
- **Develop Disaster Recovery Plan:** Create a comprehensive Disaster Recovery and Business Continuity Plan, including automated, off-site backups.

### Phase 3: Medium-Term (90-180 Days)
- **Establish Compliance Policies:** Draft and implement formal GDPR-compliant policies, including Data Classification and Breach Notification procedures.
- **Security Awareness Training:** Roll out mandatory security training for all employees focusing on phishing, data handling, and compliance.

## 📁 Deliverables
- 📄 **[Full Executive Audit Report (PDF)](./botium_toys_audit_report.pdf)** - A detailed 3-page summary of the audit findings, compliance status, and executive recommendations.

## 🎓 Author & Program Attribution
This internal security audit was completed as a Capstone/Portfolio Activity for the **Google Cybersecurity Professional Certificate** program. It demonstrates practical skills in risk assessment, compliance auditing, and security control evaluation.
