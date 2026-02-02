# Enterprise-Network-Security-Transformation
A comprehensive security architecture and implementation plan for a multi-site network merger, focusing on Zero-Trust and Cloud-Hybrid integration.

# Enterprise Network Security Transformation & Merger

## Project Overview
[cite_start]This project outlines a strategic security overhaul for a merger between a financial services firm and a medical software provider[cite: 291, 328, 477]. [cite_start]The design unifies disparate infrastructures into a hardened **Hybrid-Cloud environment** while adhering to a **$50,000 first-year budget**[cite: 388, 574].

![Network Topology](Proposed-Merged-Network-Topology.pdf)

### **Cost-Benefit Analysis & Financial Strategy**
| Category | Strategy | Rationale & Budgetary Impact |
| :--- | :--- | :--- |
| **Infrastructure** | **Transition to OpEx** | [cite_start]Shifted to a subscription-based model to avoid high upfront hardware costs[cite: 421, 555, 559]. |
| **Perimeter** | **Cloud-Based NGFW** | [cite_start]Scalable perimeter security that reduces initial capital expenditure[cite: 393, 419, 421]. |
| **Internal Defense**| **Hardware Repurposing** | [cite_start]Repurposed firewalls for internal segmentation to save significant costs[cite: 394, 422, 424]. |
| **Identity** | **Cloud IAM with MFA** | [cite_start]Enforced mandatory MFA while leveraging existing licenses to minimize spending[cite: 332, 399, 427]. |

## Technical Architecture
[cite_start]The merged network adopts a **Zero-Trust** security model integrating on-premises infrastructure with cloud services[cite: 388, 389].

### **Vulnerability Remediation**
Prior to integration, the following critical risks were mitigated:
* [cite_start]**Remote Code Execution (RCE):** Mitigated flaws in dRuby, Java RMI, and Ghostcat[cite: 326, 374, 572].
* [cite_start]**Legacy Systems:** Decommissioned end-of-life Windows 7 and Server 2012 systems to close security gaps[cite: 309, 342, 405].
* [cite_start]**Perimeter Hardening:** Closed high-risk open ports, specifically RDP (3389), to prevent unauthorized access[cite: 295, 356, 365].

### **Regulatory Compliance**
* [cite_start]**PCI DSS:** Isolated the Cardholder Data Environment (CDE) on dedicated VLANs[cite: 477, 480].
* [cite_start]**HIPAA:** Secured ePHI via dedicated segmentation and robust IAM audit trails[cite: 488, 491, 494].
