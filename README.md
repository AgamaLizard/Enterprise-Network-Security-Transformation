# Enterprise-Network-Security-Transformation
A comprehensive security architecture and implementation plan for a multi-site network merger, focusing on Zero-Trust and Cloud-Hybrid integration.

# Enterprise Network Security Transformation & Merger

## Project Overview
This project outlines a strategic security overhaul for a merger between a financial services firm and a medical software provider. The design unifies disparate infrastructures into a hardened **Hybrid-Cloud environment** while adhering to a **$50,000 first-year budget**.

![Network Topology](Proposed-Merged-Network-Topology.png.)

### **Cost-Benefit Analysis & Financial Strategy**
| Category | Strategy | Rationale & Budgetary Impact |
| :--- | :--- | :--- |
| **Infrastructure** | **Transition to OpEx** | Shifted to a subscription-based model to avoid high upfront hardware costs. |
| **Perimeter** | **Cloud-Based NGFW** | Scalable perimeter security that reduces initial capital expenditure. |
| **Internal Defense**| **Hardware Repurposing** | Repurposed firewalls for internal segmentation to save significant costs. |
| **Identity** | **Cloud IAM with MFA** | Enforced mandatory MFA while leveraging existing licenses to minimize spending. |

## Technical Architecture
The merged network adopts a **Zero-Trust** security model integrating on-premises infrastructure with cloud services.

### **Vulnerability Remediation**
Prior to integration, the following critical risks were mitigated:
* **Remote Code Execution (RCE):** Mitigated flaws in dRuby, Java RMI, and Ghostcat.
* **Legacy Systems:** Decommissioned end-of-life Windows 7 and Server 2012 systems to close security gaps.
* **Perimeter Hardening:** Closed high-risk open ports, specifically RDP (3389), to prevent unauthorized access.

### **Regulatory Compliance**
* **PCI DSS:** Isolated the Cardholder Data Environment (CDE) on dedicated VLANs.
* **HIPAA:** Secured ePHI via dedicated segmentation and robust IAM audit trails.
