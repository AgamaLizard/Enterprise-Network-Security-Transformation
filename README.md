# Enterprise-Network-Security-Transformation
A comprehensive security architecture and implementation plan for a multi-site network merger, focusing on Zero-Trust and Cloud-Hybrid integration.

# Enterprise Network Security Transformation & Merger

## Project Overview
[cite_start]This project outlines a strategic security overhaul for a merger between a financial services firm and a medical software provider. [cite_start]The design unifies disparate infrastructures into a hardened **Hybrid-Cloud environment** while adhering to a strict **$50,000 first-year budgetary cap**.

![Network Topology](Proposed-Merged-Network-Topology.png)

### **Cost-Benefit Analysis & Financial Strategy**
| Category | Strategy | Rationale & Budgetary Impact |
| :--- | :--- | :--- |
| **Infrastructure** | **Transition to OpEx** | [cite_start]Shifted to a subscription-based model to avoid high upfront hardware costs. |
| **Perimeter** | **Cloud-Based NGFW** | [cite_start]Scalable perimeter security that reduces initial capital expenditure. |
| **Internal Defense**| **Hardware Repurposing** | [cite_start]Repurposed existing firewalls for internal segmentation to save significant costs. |
| **Identity** | **Cloud IAM with MFA** | [cite_start]Enforced mandatory MFA while leveraging existing licenses to minimize spending. |

---

## Technical Architecture & Security Model
[cite_start]The merged network adopts a **Zero-Trust** security model integrating on-premises infrastructure with cloud-based services.

### **Vulnerability Remediation**
Prior to integration, the following critical risks were identified and mitigated:
* [cite_start]**Remote Code Execution (RCE):** Mitigated critical flaws including dRuby (CVE-2021-29425), Java RMI (CVE-2017-3241), and Ghostcat (CVE-2020-1938).
* [cite_start]**Legacy Systems:** Decommissioned end-of-life Windows 7 and Server 2012 systems to close unpatched security gaps.
* [cite_start]**Perimeter Hardening:** Closed high-risk open ports, specifically RDP (3389), to prevent unauthorized remote access.

### **Regulatory Compliance**
* [cite_start]**PCI DSS:** Isolated the Cardholder Data Environment (CDE) on dedicated VLANs with strict firewall rules.
* [cite_start]**HIPAA:** Secured ePHI via dedicated segmentation and robust IAM audit trails.

---

## Technical Specifications (OSI/TCP-IP Mapping)
| Component Type | OSI Layer | TCP/IP Layer |
| :--- | :--- | :--- |
| **Cloud-Based NGFW** | Layers 3 – 7 | Layers 3 – 4 |
| **VLAN Segmentation** | Layer 2 | Layer 2 |
| **Centralized IAM / MFA**| Layer 7 | Layer 4 |
| **Endpoint Detection (EDR)**| Layers 3 – 7 | Layers 3 – 4 |
