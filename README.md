# Enterprise-Network-Security-Transformation
A comprehensive security architecture and implementation plan for a multi-site network merger, focusing on Zero-Trust and Cloud-Hybrid integration.

# Enterprise Network Security Transformation & Merger

## Project Overview
This project outlines a strategic security overhaul for a merger between a financial services firm and a medical software provider. The design unifies disparate infrastructures into a hardened **Hybrid-Cloud environment** while adhering to a strict **$50,000 first-year budgetary cap**.

![Network Topology](Proposed-Merged-Network-Topology.png)

### **Cost-Benefit Analysis & Financial Strategy**
| Category | Strategy | Rationale & Budgetary Impact |
| :--- | :--- | :--- |
| **Infrastructure** | **Transition to OpEx** | Shifted to a subscription-based model to avoid high upfront hardware costs. |
| **Perimeter** | **Cloud-Based NGFW** | Scalable perimeter security that reduces initial capital expenditure. |
| **Internal Defense**| **Hardware Repurposing** | Repurposed existing firewalls for internal segmentation to save significant costs. |
| **Identity** | **Cloud IAM with MFA** | Enforced mandatory MFA while leveraging existing licenses to minimize spending. |

---

## Technical Architecture & Security Model
The merged network adopts a **Zero-Trust** security model integrating on-premises infrastructure with cloud-based services.

### **Vulnerability Remediation**
Prior to integration, the following critical risks were identified and mitigated:
* **Remote Code Execution (RCE):** Mitigated critical flaws including dRuby (CVE-2021-29425), Java RMI (CVE-2017-3241), and Ghostcat (CVE-2020-1938).
* **Legacy Systems:** Decommissioned end-of-life Windows 7 and Server 2012 systems to close unpatched security gaps.
* **Perimeter Hardening:** Closed high-risk open ports, specifically RDP (3389), to prevent unauthorized remote access.

### **Regulatory Compliance**
* **PCI DSS:** Isolated the Cardholder Data Environment (CDE) on dedicated VLANs with strict firewall rules.
* **HIPAA:** Secured ePHI via dedicated segmentation and robust IAM audit trails.

---

## Technical Specifications: OSI & TCP/IP Layer Mapping

To ensure the security architecture is technically sound, each infrastructure component has been mapped to its respective layer in the OSI and TCP/IP models.

| Component Type | OSI Layer(s) | TCP/IP Layer(s) |
| :--- | :--- | :--- |
| **Cloud-Based Next-Generation Firewall (NGFW)** | Layers 3 (Network) - 7 (Application) | Layers 3 (Internet) - 4 (Application) |
| **On-Premises Firewalls (Repurposed)** | Layers 3 (Network) - 7 (Application) | Layers 3 (Internet) - 4 (Application) |
| **VLANs (Logical Segmentation)** | Layer 2 (Data Link) | Layer 2 (Link) |
| **Micro-segmentation (Cloud NSGs/Security Groups)** | Layers 3 (Network) - 4 (Transport) | Layers 3 (Internet) - 4 (Transport) |
| **Centralized IAM System** | Layer 7 (Application) | Layer 4 (Application) |
| **Endpoint Detection and Response (EDR)** | Layers 3 (Network) - 7 (Application) | Layers 3 (Internet) - 4 (Application) |
| **Mobile Device Management (MDM)** | Layer 7 (Application) | Layer 4 (Application) |
| **Cloud-Based SIEM / Analytics Tools** | Layer 7 (Application) | Layer 4 (Application) |
| **Core Switching (Cisco/HPE/Aruba)** | Layer 2 (Data Link) | Layer 2 (Link) |
| **Wireless Access Points (Meraki/Aruba)** | Layers 1 (Physical) - 3 (Network) | Layers 1 (Link) - 3 (Internet) |
| **Servers** | Layers 1 (Physical) - 7 (Application) | Layers 1 (Link) - 4 (Application) |
| **Internet Connection (Physical Media)** | Layer 1 (Physical) | Layer 1 (Link) |



---

## Project Strategy & Compliance
* **Budgetary Constraint:** Successfully integrated all components within a **$50,000 first-year budget**.
* **Remediation:** Addressed critical RCE vulnerabilities (dRuby, Java RMI, Ghostcat) identified in pre-merger audits.
* **Compliance Frameworks:** Aligned architecture with **PCI DSS** (Cardholder Data) and **HIPAA** (ePHI) requirements via strict segmentation.
