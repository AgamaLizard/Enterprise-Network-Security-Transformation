# Enterprise Network Security Transformation & Merger

## Project Overview
This project represents a comprehensive security architecture designed for the merger of a financial services firm and a medical software provider. The solution establishes a hardened **Hybrid-Cloud environment** while strictly adhering to a **$50,000 first-year budgetary cap**.

![Network Topology](Proposed-Merged-Network-Topology.png)

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
| **Core Switching (Cisco/HPE/Aruba)** | Layer 2 (Data Link) | Layer 2 (Link) |
| **Wireless Access Points (Meraki/Aruba)** | Layers 1 (Physical) - 3 (Network) | Layers 1 (Link) - 3 (Internet) |
| **Servers** | Layers 1 (Physical) - 7 (Application) | Layers 1 (Link) - 4 (Application) |



---

## Security Strategy & Risk Mitigation
The architecture adopts a **Zero-Trust** security model and successfully remediated critical pre-merger vulnerabilities:

* **Remote Code Execution (RCE):** Mitigated critical flaws including dRuby (CVE-2021-29425), Java RMI (CVE-2017-3241), and Ghostcat (CVE-2020-1938).
* **Legacy Systems:** Decommissioned end-of-life Windows 7 and Server 2012 systems to close unpatched security gaps.
* **Perimeter Hardening:** Closed high-risk open ports (FTP/RDP) and enforced mandatory MFA via Duo.
* **Compliance Frameworks:** Aligned controls with **PCI DSS** (Cardholder Data) and **HIPAA** (ePHI) requirements via strict VLAN isolation and encryption.

---

## Financial Strategy: $50,000 Budget Cap
A key requirement was managing integration within a strict financial limit. The strategy included:

| Category | Strategy | Rationale & Budgetary Impact |
| :--- | :--- | :--- |
| **Infrastructure** | **Transition to OpEx** | Shifted to cloud subscriptions to avoid high upfront hardware capital costs. |
| **Internal Defense**| **Hardware Repurposing** | Reused existing Fortinet/Sophos hardware for internal zones to save costs. |
| **Endpoint Protection** | **License Expansion** | Expanded existing Sophos Intercept X deployments to reduce new procurement needs. |

---

## Technical Competencies
`Hybrid Cloud Architecture` `Zero-Trust Security` `Network Segmentation` `Vulnerability Management` `PCI DSS & HIPAA Compliance` `EDR/SIEM Implementation`
