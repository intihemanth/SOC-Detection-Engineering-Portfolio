
# 🧬 Multi-Vector Incident Response & Recovery

**A NIST SP 800-61 Aligned Methodology**

![NIST 800-61](https://img.shields.io/badge/Framework-NIST%20SP%20800--61-blue?style=flat-square)
![T1542.001](https://img.shields.io/badge/MITRE-T1542.001-critical?style=flat-square)
![T1547.001](https://img.shields.io/badge/MITRE-T1547.001-critical?style=flat-square)


---

## 📖 Overview

This document outlines a defensible incident response and recovery methodology for multi-stage malware incidents, aligned to **NIST SP 800-61**. It was written as a practitioner reference to address a gap I've seen repeatedly discussed in IR: the risk of **premature re-imaging** before root cause and persistence mechanisms are fully understood.

The goal isn't just "how to contain an incident" — it's *why* skipping steps in that process (specifically, re-imaging too early) leads to silent re-infection, failed audits, and destroyed forensic evidence.

> **Note:** This is a general methodology writeup based on industry frameworks and public best practices, not a record of any specific client incident or proprietary employer detection logic.

---

## 🧩 What's Covered

| Section | Description |
|---|---|
| **NIST Life Cycle Alignment** | Containment, Eradication, and Recovery phases mapped to concrete actions |
| **Risks of Premature Re-imaging** | Three real-world failure patterns: firmware persistence, identity/cloud persistence, and user-driven backup reinfection |
| **Compliance Impact** | Why skipping forensic imaging violates chain-of-custody requirements under PCI DSS, HIPAA, and GDPR |
| **Recommended Workflow** | A 5-step, order-of-operations remediation process |

## 🎯 Key Techniques Referenced (MITRE ATT&CK)

| Technique ID | Name | Relevance |
|---|---|---|
| `T1542.001` | Pre-OS Boot: System Firmware | UEFI/BIOS persistence surviving a standard re-image |
| `T1547.001` | Boot or Logon Autostart Execution: Registry Run Keys | Persistence via Run keys, including reinfection through user backups |

## 💡 Why This Matters

Most IR writeups stop at "contain, eradicate, recover." This one focuses on the **failure modes inside that process** — specifically three ways a "successful" re-image still leaves an environment compromised:

1. **Firmware-level persistence** surviving OS replacement entirely
2. **Identity-layer persistence** (OAuth tokens, IAM roles, SSH keys) that a clean OS image can't touch
3. **The "Boomerang" effect** — malware reintroduced via a user's own pre-incident data backup

## 📄 Read the Full Report

[Multi-Vector Incident Response & Recovery Report](./Methodology/Multi-Vector Incident Response & Recovery/report.md)

---

Part of my [SOC & Detection Engineering Portfolio](../../) · **📫 [Connect on LinkedIn](https://linkedin.com/in/inti-hemanth/)**
