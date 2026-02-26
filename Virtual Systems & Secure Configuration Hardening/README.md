# 🔐 Virtual Systems & Secure Configuration Hardening
## 📌 Project Overview

In this project, I deployed and configured a virtualized Windows-based lab environment to simulate enterprise network infrastructure. The lab included domain systems, kiosk workstations, administrative systems, and a domain server.

The primary objective was to harden system configurations using Group Policy, local security policies, firewall profiles, and audit settings to meet defined security requirements while maintaining operational usability.

## 🛡️ Security Design Principles

This project focused on:

* Principle of Least Privilege (PoLP)
* Defense in Depth
* System Hardening
* Auditability & Accountability
* Secure Baseline Configuration

> Rather than relying on perimeter defenses alone, I implemented host-level security controls to reduce attack surface and enforce standardized protections across systems.

## 🔧 Key Technical Deliverables
## 🔐 User Account Control (UAC) Hardening

* Increased UAC enforcement to prevent silent privilege escalation.
* Reduced risk of malware executing with elevated privileges.

## 🔑 Local Password Policy Enforcement

* Strengthened password complexity requirements.
* Configured minimum length and password history.
* Reduced susceptibility to brute-force and credential stuffing attacks.

## 🖥️ Desktop Background Restrictions

* Restricted non-admin users from modifying system configurations.
* Prevented users from altering enforced visual security policies.

## 📜 Local Audit Policy Configuration
![Desc](https://github.com/DanielSantiago10/Networking-Security-Series-Projects/blob/main/Virtual%20Systems%20%26%20Secure%20Configuration%20Hardening/Audit%20Policy.png)
* Enabled auditing of:
  * Logon events
  * Account management changes
  * Policy modifications
* Improved visibility into suspicious behavior and insider threats.

## ⚠️ Logon Banner Configuration

* Implemented legal logon warning requiring acknowledgment.
* Strengthened legal defensibility and deterrence.

## 🔥 Windows Firewall Profile Configuration

* Modified default firewall profiles.
* Ensured secure baseline traffic filtering.

## 🧠 Conceptual Deep Dive: Virtualization & Sandboxing

A major component of this project was understanding virtualization as a security control, not just an infrastructure tool.

**Benefits of Virtualization in Cybersecurity**
* Safe malware analysis in isolated virtual machines.
* Controlled testing of updates and configurations.
* Reduced hardware costs and increased scalability.
* Rapid rollback capability via snapshots.

**Limitations & Risks**

* Advanced malware can detect hypervisors.
* Virtual sandbox evasion techniques reduce effectiveness.
* Reduced stealth in certain sandbox implementations.

## 💡 How This Relates to Cybersecurity

This project reflects real-world security baseline implementation tasks performed by:

* Security Analysts
* Systems Administrators
* Blue Team Engineers

Specifically, it demonstrates:

* How misconfigured endpoints become lateral movement paths.
* Why auditing is critical for incident response.
* How host-based firewalls act as internal segmentation controls.

The importance of secure configuration management (aligned with CIS Benchmarks & NIST guidance).

Hardening endpoints is often the difference between:

> A contained compromise
> 
> vs.
> 
> A domain-wide breach

**📈 Lessons Learned**

**1️⃣ Security is Stronger at the Endpoint**

Even in segmented networks, weak host configurations can undermine everything.

**2️⃣ Default Settings Are Rarely Secure**

Operating systems are designed for usability first. Hardening requires intentional configuration.

**3️⃣ Audit Logs Are Gold During Incidents**

Without auditing enabled, forensic investigations become guesswork.

**4️⃣ Virtualization Is Both a Tool and a Target**

While virtualization improves security testing, attackers are adapting to detect and bypass sandbox environments.
