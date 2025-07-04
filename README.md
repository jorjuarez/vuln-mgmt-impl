# Vulnerability Management Program Implementation

In this project, we simulate the implementation of a comprehensive vulnerability management program, from inception to completion.

_**Inception State:**_ the organization has no existing policy or vulnerability management practices in place.

_**Completion State:**_ a formal policy is enacted, stakeholder buy-in is secured, and a full cycle of organization-wide vulnerability remediation is successfully completed.

---

### Project Highlights

This project documents the end-to-end implementation of a vulnerability management program.

* **Challenge:** Establish a formal security process in an organization with no existing vulnerability management.
* **Action:** Developed policy, secured stakeholder buy-in, performed scans, and executed a full remediation cycle.
* **Result:** Achieved an **80% reduction** in total vulnerabilities, including a **100% resolution** of all critical risks.

<img width="1000" alt="image" src="https://github.com/user-attachments/assets/cfc5dbcf-3fcb-4a71-9c13-2a49f8bab3e6">

# Skills & Technologies Showcased

- **Vulnerability Management:** Tenable.io, Nessus, Scan Analysis, Remediation Prioritization
- **Cloud & OS:** Azure Virtual Machines, Windows Server Administration
- **Automation & Scripting:** PowerShell, BASH
- **IT Governance:** Policy Creation, Change Management (CAB), Stakeholder Negotiation

---


# Table of Contents

- [Technology Utilized](#technology-utilized)
- [Step 1: Vulnerability Management Policy Draft Creation](#step-1-vulnerability-management-policy-draft-creation)
- [Step 2: Case Study - Securing Stakeholder Buy-In for a New Security Policy](#step-2-case-study---securing-stakeholder-buy-in-for-a-new-security-policy)
- [Step 3: Policy Finalization and Senior Leadership Sign-Off](#step-3-policy-finalization-and-senior-leadership-sign-off)
- [Step 4: Case Study - Implementing a Secure Credentialed Scanning Program](#step-4-case-study---implementing-a-secure-credentialed-scanning-program)
- [Step 5: Initial Scan of Server Team Assets](#step-5-initial-scan-of-server-team-assets)
- [Step 6: Vulnerability Assessment and Prioritization](#step-6-vulnerability-assessment-and-prioritization)
- [Step 7: Distributing Remediations to Remediation Teams](#step-7-distributing-remediations-to-remediation-teams)
- [Step 8: Case Study - Collaborative Review and Triage of Vulnerability Scan Results](#step-8-case-study---collaborative-review-and-triage-of-vulnerability-scan-results)
- [Step 9: Case Study - Presenting a Security Change to the Change Advisory Board (CAB)](#step-9-case-study---presenting-a-security-change-to-the-change-advisory-board-cab)
- [Step 10 - Remediation Effort](#step-10---remediation-effort)
  - [Remediation Round 1: Outdated Wireshark Removal](#remediation-round-1-outdated-wireshark-removal)
  - [Remediation Round 2: Insecure Protocols & Ciphers](#remediation-round-2-insecure-protocols--ciphers)
  - [Remediation Round 3: Guest Account Group Membership](#remediation-round-3-guest-account-group-membership)
  - [Remediation Round 4: Windows OS Updates](#remediation-round-4-windows-os-updates)
- [First Cycle Remediation Effort Summary](#first-cycle-remediation-effort-summary)
- [On-going Vulnerability Management (Maintenance Mode)](#on-going-vulnerability-management-maintenance-mode)

---

### Step 1: Vulnerability Management Policy Draft Creation

This phase focuses on drafting a Vulnerability Management Policy as a starting point for stakeholder engagement. The initial draft outlines scope, responsibilities, and remediation timelines, and may be adjusted based on feedback from relevant departments to ensure practical implementation before final approval by upper management.  
[Draft Policy](https://docs.google.com/document/d/1N7DBV2VxZWyqdRabs9VhIQoNhNQTFX0jYSr47uoWPgg/edit?usp=sharing)

---

### Step 2: Case Study - Securing Stakeholder Buy-In for a New Security Policy

### Objective
As a Cyber VM Analyst, the objective was to implement a more aggressive vulnerability remediation policy. To ensure the policy was both effective for security and operationally feasible, a proactive partnership with the IT server team was crucial for developing a balanced and realistic solution.

---

### Challenge & Approach
The organization needed to reduce its risk exposure by accelerating vulnerability remediation timelines. An initial draft policy proposed a 48-hour deadline for all critical vulnerabilities. While secure, this timeline was unfeasible for the server team given their operational workload, creating a potential conflict between security goals and IT capacity.

Instead of dictating terms, a collaborative process was initiated with the Server Team Manager to build consensus and find a practical path forward. The approach centered on three key compromises:

* **Tiered Timelines:** A more manageable 7-day remediation window was established for most critical vulnerabilities.
* **Urgent Threat Exception:** The aggressive 48-hour deadline was reserved for true zero-day exploits and other imminent threats, allowing for a rapid response when it mattered most.
* **Smooth Transition:** A six-month grace period was secured post-launch to allow teams to adapt to the new process without immediate pressure.

---

### Outcome & Impact
This collaborative negotiation transformed the server team from potential blockers into key partners. The resulting policy was not only formally adopted but had strong buy-in from all stakeholders.

Ultimately, a stronger security policy was successfully implemented that balanced aggressive goals with operational reality. This project strengthened the relationship between the Cybersecurity and IT Operations teams and created a more robust and sustainable vulnerability management program.

---

### Skills Demonstrated
* Stakeholder Management & Negotiation
* Cybersecurity Policy Development
* Proactive & Empathetic Communication
* Vulnerability Management Lifecycle
* Collaborative Problem-Solving
* Risk Management & Assessment

---

### Step 3: Policy Finalization and Senior Leadership Sign-Off

After gathering feedback from the server team, the policy is revised, addressing aggressive remediation timelines. With final approval from upper management, the policy now guides the program, ensuring compliance and reference for pushback resolution.  
[Finalized Policy](https://docs.google.com/document/d/1N7DBV2VxZWyqdRabs9VhIQoNhNQTFX0jYSr47uoWPgg/edit?usp=sharing)

![image](https://github.com/user-attachments/assets/b3461993-53c6-4d27-add4-a85232eb093d)

---

### Step 4: Case Study - Implementing a Secure Credentialed Scanning Program

### Objective
To operationalize a new vulnerability management policy by establishing a regular, credentialed scanning schedule for the server environment. The goal was to gain deep, authenticated visibility into system vulnerabilities while addressing the server team's concerns regarding security and operational stability.

---

### Challenge & Approach
The initial proposal for a 4-6 hour weekly scan across 200 servers was met with resistance. The Server Team Manager raised two critical objections, which were addressed with targeted solutions to build trust and find a practical path forward:

**Challenge (Operational Risk):** The potential for high resource utilization during the scan could impact server performance.
**Solution (Phased Pilot):** To demonstrate minimal performance impact, a pilot scan was first conducted on a single, non-critical server to closely monitor resource use before any full-scale deployment.

**Challenge (Security Risk):** Providing a single, persistent administrative account for all 200 machines created an unacceptable security risk.
**Solution (JIT Credentials):** To mitigate this risk, a Just-in-Time (JIT) access model was implemented. A dedicated service account remained disabled by default, was enabled only for the scan's duration, and was immediately disabled upon completion, adhering to the principle of least privilege.

---

### Outcome & Impact
The server team agreed to the revised approach. The manager demonstrated full buy-in by immediately tasking a team member with automating the JIT account provisioning process.

By proactively addressing legitimate concerns, this approach overcame initial resistance and established a secure, operationally sound process for credentialed scanning. This built a foundation of trust for the ongoing vulnerability management program, ensuring security objectives could be met without compromising operational integrity.

---

### Skills Demonstrated
* Technical Problem-Solving
* Risk Mitigation & Management
* Technical Negotiation
* Principle of Least Privilege
* Stakeholder Collaboration
* Vulnerability Scanning & Management  



---

### Step 5: Initial Scan of Server Team Assets

In this phase, an insecure Windows Server is provisioned to simulate the server team's environment. After creating vulnerabilities, an authenticated scan is performed, and the results are exported for future remediation steps.  

![image](https://github.com/user-attachments/assets/c1382b4f-ff00-48c3-83bc-5474c33cf279)

[Scan 1 - Initial Scan](https://drive.google.com/file/d/1QuwXnY6RIhrgr3tE7P_xs6Onnm_02CHO/view?usp=sharing)




---

### Step 6: Vulnerability Assessment and Prioritization

We assessed vulnerabilities and established a remediation prioritization strategy based on ease of remediation and impact. The following priorities were set:

1. Third Party Software Removal (Wireshark)
2. Windows OS Secure Configuration (Protocols & Ciphers)
3. Windows OS Secure Configuration (Guest Account Group Membership)
4. Windows OS Updates

---

### Step 7: Distributing Remediations to Remediation Teams

The server team received remediation scripts and scan reports to address key vulnerabilities. This streamlined their efforts and prepared them for a follow-up review.  

<img width="635" alt="image" src="https://github.com/user-attachments/assets/bbf9478f-e1d1-4898-846e-b510ec8c6f72">

[Key Vulnerabilities Remediation Email](https://github.com/jorjuarez/Cybersecurity-Portfolio-Public/blob/main/misc/remediation-email.md)

---

### Step 8: Case Study - Collaborative Review and Triage of Vulnerability Scan Results

### Objective
To analyze the results of the first credentialed vulnerability scan and translate the raw data into a prioritized, actionable remediation plan in collaboration with the server team.

---

### Challenge & Approach
The primary challenge was to analyze and contextualize the raw scan data, separating critical vulnerabilities from low-priority noise to create an achievable remediation plan.

A collaborative review session was initiated with the server team to systematically triage the findings. The process began by confirming that the pilot scan caused no performance issues, building confidence for future scans. From there, the vulnerabilities were grouped into logical categories:

* **High-Priority (Manual Remediation):** This category included outdated software (Wireshark), a critical misconfiguration (Guest account in the local Administrators group), and deprecated protocols/ciphers (TLS 1.0/1.1).
* **Automated Remediation:** Vulnerabilities related to out-of-date Microsoft products (e.g., Edge) were identified as likely to be resolved by the existing patch management solution.
* **Informational / Low-Risk:** Findings like self-signed SSL certificates were identified as low-risk and deprioritized to focus efforts on more critical items.

To ensure feasibility, the analyst proactively confirmed with the Server Team Manager that the high-priority items were low-risk to remediate and would be approved through the Change Control Board. This led to a clear action plan where the analyst took responsibility for packaging remediation solutions, while the server team managed automated patching.

---

### Outcome & Impact
The collaborative review successfully transformed a long list of vulnerabilities into a short, prioritized list of actionable tasks. The server team understood exactly what needed to be done and why, and they agreed to the remediation plan.

By proactively filtering noise and collaborating with asset owners, an efficient triage process was established. This built a strong partnership and ensured that remediation efforts were focused on the most significant risks, with a clear plan ready to present at the next Change Control Board.

---

### Skills Demonstrated
* Vulnerability Analysis & Triage
* Technical Communication
* Collaborative Problem-Solving
* Risk Prioritization
* Remediation Planning
* IT Process Integration (Patching, Change Control)

---

### Step 9: Case Study - Presenting a Security Change to the Change Advisory Board (CAB)

### Objective
To present a planned security remediation to the Change Advisory Board (CAB) and gain official approval by clearly articulating the technical change, its associated risks, and a robust mitigation and rollback strategy.

---

### Challenge & Approach
The change involved disabling deprecated TLS protocols and weak cipher suites across the server environment. While technically a simple registry modification deployed via PowerShell, any change to cryptographic standards carries the inherent risk of disrupting critical application connectivity. The challenge was to assure the CAB that all potential risks had been considered and that a comprehensive safety net was in place.

The presentation to the CAB was structured around two pillars to proactively address their primary concerns:

1.  **Clear Communication:** The change was explained in simple terms: a PowerShell script would modify the Windows registry to disable outdated protocols (TLS 1.0, 1.1) and ciphers. Describing it as a common and well-understood procedure demystified the change for non-specialist stakeholders.
2.  **Proactive Risk Mitigation:** To proactively address concerns about negative impacts, a multi-layered safety plan was detailed:
    * **Tiered Deployment:** The change would follow a phased rollout (Pilot -> Pre-Production -> Production), allowing for issues to be caught in a small, controlled group before impacting the entire environment.
    * **Automated Rollback Script:** A fully tested, automated PowerShell script was created to instantly revert the registry changes to their original state, ensuring a near-zero Recovery Time Objective (RTO) if unforeseen issues arose.

---

### Outcome & Impact
The CAB approved the change. By anticipating questions and presenting a comprehensive, multi-layered safety plan, this approach demonstrated thoroughness and due diligence.

This not only secured the necessary approval but also built the board's confidence in the security team's ability to manage operational risk. The remediation was subsequently deployed without issue, successfully hardening the security posture of the server fleet.

---

### Skills Demonstrated
* Change Management (CAB Process)
* Risk Assessment & Mitigation
* Technical Communication
* Remediation Scripting (PowerShell)
* Deployment Planning (Phased Rollout)
* IT Governance & Compliance

---
### Step 10 - Remediation Effort

#### Remediation Round 1: Outdated Wireshark Removal

The server team used a PowerShell script to remove outdated Wireshark. A follow-up scan confirmed successful remediation.  
[Wireshark Removal Script](https://github.com/jorjuarez/Cybersecurity-Portfolio-Public/blob/main/automation/remediation-wireshark-uninstall.ps1) - *A PowerShell script to silently uninstall specific versions of Wireshark from Windows systems.* 

![image](https://github.com/user-attachments/assets/58da86b6-9d02-4150-aef5-22459e84fca1)


[Scan 2 - Third Party Software Removal](https://drive.google.com/file/d/1-IxeP9eZLepWvczgAc3uH-avaGp_SMjP/view?usp=drive_link)


#### Remediation Round 2: Insecure Protocols & Ciphers

The server team used PowerShell scripts to remediate insecure protocols and cipher suites. A follow-up scan verified successful remediation, and the results were saved for reference.  
[PowerShell: Insecure Protocols Remediation](https://github.com/jorjuarez/Cybersecurity-Portfolio-Public/blob/main/automation/toggle-protocols.ps1)
[PowerShell: Insecure Ciphers Remediation](https://github.com/jorjuarez/Cybersecurity-Portfolio-Public/blob/main/automation/toggle-cipher-suites.ps1)

![image](https://github.com/user-attachments/assets/a59819fb-da29-4d9f-93d5-edf35c147268)


[Scan 3 - Ciphersuites and Protocols](https://drive.google.com/file/d/1tza2bBV5xJ8OTBRromuWwNv6mRbj2rXg/view?usp=sharing)


#### Remediation Round 3: Guest Account Group Membership

The server team removed the guest account from the administrator group. A new scan confirmed remediation, and the results were exported for comparison.  
[PowerShell: Guest Account Group Membership Remediation](https://github.com/jorjuarez/Cybersecurity-Portfolio-Public/blob/main/automation/toggle-guest-local-administrators.ps1)  

![image](https://github.com/user-attachments/assets/1eec9c35-ff8b-4f21-953e-62c66280b5b2)


[Scan 4 - Guest Account Group Removal](https://drive.google.com/file/d/1KBVnQ7fzZmQ0SlsvKJRb5IWmG8DRq8mJ/view?usp=sharing)


#### Remediation Round 4: Windows OS Updates

Windows updates were re-enabled and applied until the system was fully up to date. A final scan verified the changes  

![image](https://github.com/user-attachments/assets/9ce498b9-c78a-412a-8f2b-d78149c0d355)


[Scan 5 - Post Windows Updates](https://drive.google.com/file/d/1nSl8vtLY1IIqD4ponfLcGkID_2wD9ODy/view?usp=sharing)

---

### First Cycle Remediation Effort Summary

The remediation process reduced total vulnerabilities by 80%, from 30 to 6. Critical vulnerabilities were resolved by the second scan (100%), and high vulnerabilities dropped by 90%. Mediums were reduced by 76%. In an actual production environment, asset criticality would further guide future remediation efforts.  

![image](https://github.com/user-attachments/assets/f44a9acf-45f9-4507-bf32-7d238db1d4ea)


[Remediation Data](https://docs.google.com/spreadsheets/d/1pXadJqQ1Fi75gYpYLEWCIPbsSlADI1CJZaO4iAHSD7g/edit?usp=sharing)

---

### On-going Vulnerability Management (Maintenance Mode)

After completing the initial remediation cycle, the vulnerability management program transitions into **Maintenance Mode**. This phase ensures that vulnerabilities continue to be managed proactively, keeping systems secure over time. Regular scans, continuous monitoring, and timely remediation are crucial components of this phase. (See [Finalized Policy](https://docs.google.com/document/d/1N7DBV2VxZWyqdRabs9VhIQoNhNQTFX0jYSr47uoWPgg/edit?usp=sharing) for scanning and remediation cadence requirements.)

Key activities in Maintenance Mode include:
- **Scheduled Vulnerability Scans**: Perform regular scans (e.g., weekly or monthly) to detect new vulnerabilities as systems evolve.
- **Patch Management**: Continuously apply security patches and updates, ensuring no critical vulnerabilities remain unpatched.
- **Remediation Follow-ups**: Address newly identified vulnerabilities promptly, prioritizing based on risk and impact.
- **Policy Review and Updates**: Periodically review the Vulnerability Management Policy to ensure it aligns with the latest security best practices and organizational needs.
- **Audit and Compliance**: Conduct internal audits to ensure compliance with the vulnerability management policy and external regulations.
- **Ongoing Communication with Stakeholders**: Maintain open communication with teams responsible for remediation, ensuring efficient coordination.

By maintaining an active vulnerability management process, organizations can stay ahead of emerging threats and ensure long-term security resilience.
