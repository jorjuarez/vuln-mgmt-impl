# Official [Cyber Range](http://joshmadakor.tech/cyber-range) Project

# Vulnerability Management Program Implementation

In this project, we simulate the implementation of a comprehensive vulnerability management program, from inception to completion.

_**Inception State:**_ the organization has no existing policy or vulnerability management practices in place.

_**Completion State:**_ a formal policy is enacted, stakeholder buy-in is secured, and a full cycle of organization-wide vulnerability remediation is successfully completed.

---

<img width="1000" alt="image" src="https://github.com/user-attachments/assets/cfc5dbcf-3fcb-4a71-9c13-2a49f8bab3e6">

# Technology Utilized
- Tenable (enterprise vulnerability management platform)
- Azure Virtual Machines (Nessus scan engine + scan targets)
- PowerShell & BASH (remediation scripts)

---


# Table of Contents

- [Vulnerability Management Policy Draft Creation](#vulnerability-management-policy-draft-creation)
- [Case Study 1: Securing Stakeholder Buy-In](#case-study-securing-stakeholder-buy-in-for-a-new-security-policy)
- [Policy Finalization and Senior Leadership Sign-Off](#policy-finalization-and-senior-leadership-sign-off)
- [Case Study 2: Implementing Secure Scanning](#case-study-implementing-a-secure-credentialed-scanning-program)
- [Initial Scan of Server Team Assets](#step-5-initial-scan-of-server-team-assets)
- [Vulnerability Assessment and Prioritization](#step-6-vulnerability-assessment-and-prioritization)
- [Distributing Remediations to Remediation Teams](#step-7-distributing-remediations-to-remediation-teams)
- [Mock Meeting: Post-Initial Discovery Scan (Server Team)](#step-8-mock-meeting-post-initial-discovery-scan-server-team)
- [Mock CAB Meeting: Implementing Remediations](#step-9-mock-cab-meeting-implementing-remediations)
- [Remediation Round 1: Outdated Wireshark Removal](#remediation-round-1-outdated-wireshark-removal)
- [Remediation Round 2: Insecure Protocols & Ciphers](#remediation-round-2-insecure-protocols--ciphers)
- [Remediation Round 3: Guest Account Group Membership](#remediation-round-3-guest-account-group-membership)
- [Remediation Round 4: Windows OS Updates](#remediation-round-4-windows-os-updates)
- [First Cycle Remediation Effort Summary](#first-cycle-remediation-effort-summary)

---

### Vulnerability Management Policy Draft Creation

This phase focuses on drafting a Vulnerability Management Policy as a starting point for stakeholder engagement. The initial draft outlines scope, responsibilities, and remediation timelines, and may be adjusted based on feedback from relevant departments to ensure practical implementation before final approval by upper management.  
[Draft Policy](https://docs.google.com/document/d/1N7DBV2VxZWyqdRabs9VhIQoNhNQTFX0jYSr47uoWPgg/edit?usp=sharing)

---

### Case Study: Securing Stakeholder Buy-In for a New Security Policy

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

### Policy Finalization and Senior Leadership Sign-Off

After gathering feedback from the server team, the policy is revised, addressing aggressive remediation timelines. With final approval from upper management, the policy now guides the program, ensuring compliance and reference for pushback resolution.  
[Finalized Policy](https://docs.google.com/document/d/1rvueLX_71pOR8ldN9zVW9r_zLzDQxVsnSUtNar8ftdg/edit?usp=drive_link)

![image](https://github.com/user-attachments/assets/b3461993-53c6-4d27-add4-a85232eb093d)

---

### Case Study: Implementing a Secure Credentialed Scanning Program

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

### Step 5) Initial Scan of Server Team Assets

In this phase, an insecure Windows Server is provisioned to simulate the server team's environment. After creating vulnerabilities, an authenticated scan is performed, and the results are exported for future remediation steps.  

<img width="635" alt="image" src="https://github.com/user-attachments/assets/937cccbd-36bb-4445-97b9-e915085cda81" style="border: 2px solid black;">

[Scan 1 - Initial Scan](https://drive.google.com/file/d/1RBPVj_azKJMwmRZ8QILlb4hxIjQU3wQ7/view?usp=drive_link)




---

### Step 6) Vulnerability Assessment and Prioritization

We assessed vulnerabilities and established a remediation prioritization strategy based on ease of remediation and impact. The following priorities were set:

1. Third Party Software Removal (Wireshark)
2. Windows OS Secure Configuration (Protocols & Ciphers)
3. Windows OS Secure Configuration (Guest Account Group Membership)
4. Windows OS Updates

---

### Step 7) Distributing Remediations to Remediation Teams

The server team received remediation scripts and scan reports to address key vulnerabilities. This streamlined their efforts and prepared them for a follow-up review.  

<img width="635" alt="image" src="https://github.com/user-attachments/assets/bbf9478f-e1d1-4898-846e-b510ec8c6f72">

[Remediation Email](https://github.com/joshmadakor1/lognpacific-public/blob/main/misc/remediation-email.md)

---

### Step 8) Mock Meeting: Post-Initial Discovery Scan (Server Team)

The server team reviewed vulnerability scan results, identifying outdated software, insecure accounts, and deprecated protocols. The remediation packages were prepared for submission to the Change Control Board (CAB). 

<a href="https://youtu.be/0tjjFewxSNw" target="_"><img width="600" src="https://github.com/user-attachments/assets/03027c66-5f7c-42d0-b6dd-09d053c040b1"/></a>

[Meeting Video](https://youtu.be/0tjjFewxSNw)

---

### Step 9) Mock CAB Meeting: Implementing Remediations

The Change Control Board (CAB) reviewed and approved the plan to remove insecure protocols and cipher suites. The plan included a rollback script and a tiered deployment approach.  

<a href="https://youtu.be/zOFPkTa9kY8" target="_"><img width="600" src="https://github.com/user-attachments/assets/07164e63-fbce-471a-b469-29a6d41b7bb8"/></a>

[Meeting Video](https://youtu.be/zOFPkTa9kY8)

---
### Step 10 ) Remediation Effort

#### Remediation Round 1: Outdated Wireshark Removal

The server team used a PowerShell script to remove outdated Wireshark. A follow-up scan confirmed successful remediation.  
[Wireshark Removal Script](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/remediation-wireshark-uninstall.ps1)  

<img width="634" alt="image" src="https://github.com/user-attachments/assets/7b4f9ab2-d230-4458-ac0f-c0ff070ae79a">

[Scan 2 - Third Party Software Removal](https://drive.google.com/file/d/1UiwPPTtuSZKk02hiMyXf31pXUIeC5EWt/view?usp=drive_link)


#### Remediation Round 2: Insecure Protocols & Ciphers

The server team used PowerShell scripts to remediate insecure protocols and cipher suites. A follow-up scan verified successful remediation, and the results were saved for reference.  
[PowerShell: Insecure Protocols Remediation](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/toggle-protocols.ps1)
[PowerShell: Insecure Ciphers Remediation](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/toggle-cipher-suites.ps1)

<img width="630" alt="image" src="https://github.com/user-attachments/assets/0e96120d-8ec9-4f76-8e42-79c752200010">

[Scan 3 - Ciphersuites and Protocols](https://drive.google.com/file/d/1Qc6-ezQvwReCGUZNtnva0kCZo_-zW-Sm/view?usp=drive_link)


#### Remediation Round 3: Guest Account Group Membership

The server team removed the guest account from the administrator group. A new scan confirmed remediation, and the results were exported for comparison.  
[PowerShell: Guest Account Group Membership Remediation](https://github.com/joshmadakor1/lognpacific-public/blob/main/automation/toggle-guest-local-administrators.ps1)  

<img width="627" alt="image" src="https://github.com/user-attachments/assets/870a3eac-3398-44fe-91c0-96f3c2578df4">

[Scan 4 - Guest Account Group Removal](https://drive.google.com/file/d/1jVgikjfrV1YjOcL3QRT_oUB0Y82w22V7/view?usp=drive_link)


#### Remediation Round 4: Windows OS Updates

Windows updates were re-enabled and applied until the system was fully up to date. A final scan verified the changes  

<img width="627" alt="image" src="https://github.com/user-attachments/assets/870a3eac-3398-44fe-91c0-96f3c2578df4">

[Scan 5 - Post Windows Updates](https://drive.google.com/file/d/1tmDjeHl5uiGitRwWy8kFRi33q-nGi1Zt/view?usp=drive_link)

---

### First Cycle Remediation Effort Summary

The remediation process reduced total vulnerabilities by 80%, from 30 to 6. Critical vulnerabilities were resolved by the second scan (100%), and high vulnerabilities dropped by 90%. Mediums were reduced by 76%. In an actual production environment, asset criticality would further guide future remediation efforts.  

<img width="1920" alt="image" src="https://github.com/user-attachments/assets/51f0aae8-7f36-4d90-b29f-5257e57155f9">

[Remediation Data](https://docs.google.com/spreadsheets/d/1FTtFfZYmFsNLU6pm8nTzsKyKE-d2ftXzX_DPwcnFNfA/edit?gid=0#gid=0)

---

### On-going Vulnerability Management (Maintenance Mode)

After completing the initial remediation cycle, the vulnerability management program transitions into **Maintenance Mode**. This phase ensures that vulnerabilities continue to be managed proactively, keeping systems secure over time. Regular scans, continuous monitoring, and timely remediation are crucial components of this phase. (See [Finalized Policy](https://docs.google.com/document/d/1rvueLX_71pOR8ldN9zVW9r_zLzDQxVsnSUtNar8ftdg/edit?usp=drive_link) for scanning and remediation cadence requirements.)

Key activities in Maintenance Mode include:
- **Scheduled Vulnerability Scans**: Perform regular scans (e.g., weekly or monthly) to detect new vulnerabilities as systems evolve.
- **Patch Management**: Continuously apply security patches and updates, ensuring no critical vulnerabilities remain unpatched.
- **Remediation Follow-ups**: Address newly identified vulnerabilities promptly, prioritizing based on risk and impact.
- **Policy Review and Updates**: Periodically review the Vulnerability Management Policy to ensure it aligns with the latest security best practices and organizational needs.
- **Audit and Compliance**: Conduct internal audits to ensure compliance with the vulnerability management policy and external regulations.
- **Ongoing Communication with Stakeholders**: Maintain open communication with teams responsible for remediation, ensuring efficient coordination.

By maintaining an active vulnerability management process, organizations can stay ahead of emerging threats and ensure long-term security resilience.
