# Cyber-HandsOnLab

# 16-Module Job-Ready Cybersecurity Training Path (Hands-On)

This repository now contains a complete, practical, job-ready cybersecurity roadmap with hands-on labs, detailed activities, and measurable outcomes.

## Program Snapshot
- **Target audience:** Beginners to IT professionals transitioning to cybersecurity
- **Duration:** 24-32 weeks (part-time) or 12-16 weeks (full-time)
- **Format:** Learn -> Practice -> Validate -> Report
- **Outcome:** SOC-ready, analyst-ready, and junior defensive security roles

## Learning Method (Applied in Every Module)
1. **Concept Briefing** (core theory + attack/defense context)
2. **Tooling Walkthrough** (how tools work and when to use them)
3. **Hands-On Lab** (step-by-step execution in lab environment)
4. **Evidence Collection** (screenshots, logs, IoCs, artifacts)
5. **Reporting** (technical + executive summary)
6. **Assessment** (quiz, practical check, and interview-style questions)

---

## Module 1 - Introduction to Cybersecurity & Reconnaissance
**Goal:** Understand cybersecurity domains, attacker lifecycle, legal boundaries, and reconnaissance fundamentals.

### Topics
- CIA triad, risk, threat, vulnerability, exploit, impact
- Blue Team vs Red Team vs Purple Team
- Passive/active recon and OSINT scope
- Rules of engagement and ethical testing

### Hands-On Lab (Recon Starter)
1. Build a target profile using passive OSINT (domain, DNS, metadata).
2. Perform safe active recon on approved lab targets.
3. Document findings: exposed services, technologies, and attack surface.

### Deliverables
- Recon report with scope, tools used, findings, and risk rating.

---

## Module 2 - Linux Fundamentals & Security Lab Environment Setup
**Goal:** Build a secure lab and gain Linux command-line confidence.

### Topics
- Linux filesystem, users/groups, permissions, process management
- Bash basics, package management, logs, SSH hygiene
- Virtualization/networking basics for labs

### Hands-On Lab (Lab Buildout)
1. Install virtualization platform and create attacker + defender VMs.
2. Configure isolated virtual network and snapshots.
3. Harden Linux baseline (firewall, least privilege, updates).
4. Validate connectivity and logging between systems.

### Deliverables
- Lab topology diagram + hardened Linux checklist.

---

## Module 3 - Network Scanning & Vulnerability Detection
**Goal:** Discover assets and identify vulnerabilities responsibly.

### Topics
- TCP/IP, common ports/services, scan types and detection footprints
- Vulnerability scanning lifecycle and false positives
- Prioritization by exploitability and business impact

### Hands-On Lab (Scan & Validate)
1. Perform host discovery and port scanning.
2. Enumerate service versions and operating systems.
3. Run vulnerability scanner and export findings.
4. Validate high-risk findings manually to reduce false positives.

### Deliverables
- Validated vulnerability list with remediation priorities.

---

## Module 4 - Network Traffic Analysis & Protection
**Goal:** Analyze packet and flow data to detect suspicious activity.

### Topics
- Packet structure, protocols, baseline vs anomaly
- Traffic capture and filtering strategies
- Detection of beaconing, lateral movement, and exfil patterns

### Hands-On Lab (PCAP Investigation)
1. Capture traffic from a controlled scenario.
2. Filter by protocol, host, and suspicious behavior.
3. Reconstruct attack timeline from packet evidence.
4. Propose network controls to prevent recurrence.

### Deliverables
- Traffic analysis worksheet + incident timeline.

---

## Module 5 - Active Directory Security & Enumeration
**Goal:** Understand AD architecture, common misconfigurations, and defense.

### Topics
- AD objects, Kerberos/NTLM, trusts, Group Policy basics
- Privilege paths, weak ACLs, stale accounts, and delegation risks
- Defensive hardening and monitoring priorities

### Hands-On Lab (AD Enumeration)
1. Enumerate users, groups, shares, and privilege relationships.
2. Identify risky accounts and policy gaps.
3. Harden key settings (password, lockout, admin tiering concepts).
4. Re-test to verify risk reduction.

### Deliverables
- AD findings matrix + hardening action plan.

---

## Module 6 - Email Security & Phishing Analysis
**Goal:** Detect, analyze, and respond to phishing and email-borne threats.

### Topics
- Email headers, SPF/DKIM/DMARC fundamentals
- Social engineering indicators and payload delivery methods
- Safe triage and user-reporting workflows

### Hands-On Lab (Phishing Triage)
1. Parse suspicious email headers and authentication results.
2. Analyze URLs, attachments, and sender reputation safely.
3. Classify as malicious/suspicious/benign with evidence.
4. Draft user advisory and SOC escalation note.

### Deliverables
- Phishing analysis report + awareness bulletin.

---

## Module 7 - SOC Operations & Security Monitoring
**Goal:** Operate core SOC workflows and triage alerts effectively.

### Topics
- SIEM fundamentals, event normalization, detection rules
- Alert triage workflow and prioritization
- Incident ticketing and evidence handling

### Hands-On Lab (SOC Triage)
1. Ingest log sources (endpoint, auth, network).
2. Build basic detection queries and alert rules.
3. Triage alerts using severity/confidence framework.
4. Escalate one incident with full analyst notes.

### Deliverables
- Alert triage runbook + sample ticket pack.

---

## Module 8 - Firewalls, IDS/IPS & Network Defense
**Goal:** Design layered network defenses and tune detection.

### Topics
- Firewall policy design and segmentation principles
- IDS/IPS signatures vs behavior detections
- Rule tuning and false positive management

### Hands-On Lab (Defensive Control Tuning)
1. Create baseline firewall rules for segmented zones.
2. Deploy IDS/IPS detection set in monitor mode.
3. Simulate known benign and malicious traffic.
4. Tune rules and document before/after performance.

### Deliverables
- Network defense policy set + tuning log.

---

## Module 9 - Web Server Security, Hardening & Web Application Security
**Goal:** Secure web infrastructure and understand common web attacks.

### Topics
- Server hardening, TLS basics, secure headers
- OWASP Top 10 attack patterns and mitigations
- Logging and secure deployment checks

### Hands-On Lab (Web Hardening)
1. Baseline scan of web server and app exposure.
2. Apply hardening controls (patching, config, headers, TLS).
3. Re-scan and test against common attack vectors.
4. Document residual risks and compensating controls.

### Deliverables
- Hardened web checklist + verification report.

---

## Module 10 - EDR/XDR & Endpoint Protection
**Goal:** Detect and contain endpoint threats with modern telemetry.

### Topics
- Endpoint telemetry, behavioral detection, ATT&CK mapping
- Investigation pivots: process tree, parent-child anomalies, hashes
- Isolation/containment and response workflows

### Hands-On Lab (Endpoint Incident)
1. Review endpoint alerts and process execution chain.
2. Hunt for related indicators across endpoints.
3. Isolate compromised endpoint and collect artifacts.
4. Create containment and recovery steps.

### Deliverables
- Endpoint IR case file + containment checklist.

---

## Module 11 - Cloud IAM Security & Monitoring
**Goal:** Secure identities and monitor cloud activity.

### Topics
- IAM users, roles, policies, trust boundaries, least privilege
- Cloud logging/monitoring and anomaly detection
- Misconfiguration patterns (public access, over-permissive roles)

### Hands-On Lab (Cloud IAM Hardening)
1. Audit IAM identities and policy permissions.
2. Detect privilege escalation and persistence risks.
3. Implement least-privilege policy corrections.
4. Configure logging alerts for sensitive actions.

### Deliverables
- IAM risk register + corrected policy set.

---

## Module 12 - Vulnerability Assessment & Reporting
**Goal:** Produce professional vulnerability assessments and actionable reports.

### Topics
- Assessment scoping, asset criticality, and methodology
- CVSS/contextual risk scoring
- Remediation tracking and validation testing

### Hands-On Lab (End-to-End VA)
1. Define scope and critical assets.
2. Scan, validate, and prioritize vulnerabilities.
3. Build technical findings with proof and remediation steps.
4. Prepare executive summary with risk themes.

### Deliverables
- Full VA report (technical + executive sections).

---

## Module 13 - ASD Essential Eight & Compliance Frameworks
**Goal:** Map controls to compliance requirements and implementation maturity.

### Topics
- ASD Essential Eight strategies and maturity levels
- Mapping to broader governance frameworks
- Gap assessment and remediation roadmaps

### Hands-On Lab (Compliance Gap Review)
1. Assess current-state controls against Essential Eight.
2. Score maturity and identify control gaps.
3. Build phased remediation roadmap with owners/timelines.
4. Define evidence requirements for audit readiness.

### Deliverables
- Compliance gap assessment + maturity roadmap.

---

## Module 14 - Threat Intelligence & Security Reporting
**Goal:** Convert threat data into defensive action and leadership reporting.

### Topics
- Tactical/operational/strategic threat intelligence
- IOC vs TTP analysis and ATT&CK alignment
- Executive communication and decision-focused reporting

### Hands-On Lab (Intel-to-Detection)
1. Ingest threat report and extract relevant IOCs/TTPs.
2. Convert intel into SIEM/EDR detections.
3. Validate detections with controlled test data.
4. Publish stakeholder-ready threat brief.

### Deliverables
- Threat brief + detection update changelog.

---

## Module 15 - Capstone: Enterprise Incident Response Simulation
**Goal:** Execute a complete incident response lifecycle in a realistic scenario.

### Simulation Stages
1. **Preparation:** scope, comms plan, and IR roles.
2. **Detection & Analysis:** correlate multi-source alerts.
3. **Containment:** short-term and long-term containment decisions.
4. **Eradication & Recovery:** root cause removal and service restoration.
5. **Lessons Learned:** post-incident review and control improvements.

### Hands-On Lab (Team Exercise)
1. Receive simulated incident injects.
2. Investigate artifacts across endpoint, network, and identity logs.
3. Produce decisions under time pressure.
4. Deliver technical incident report + executive debrief.

### Deliverables
- Full IR report, timeline, and corrective action register.

---

## Module 16 - Career Readiness, Certification Prep & Job Placement
**Goal:** Convert technical capability into interview and job performance.

### Topics
- Resume and portfolio building from lab artifacts
- Analyst interview question banks and mock interviews
- Certification alignment (entry to intermediate)
- Professional communication and stakeholder updates

### Hands-On Lab (Job-Ready Portfolio)
1. Build portfolio with 5+ completed lab reports.
2. Record a mock incident briefing presentation.
3. Complete mock technical interview panel.
4. Create 90-day onboarding plan for first cybersecurity role.

### Deliverables
- Job-ready portfolio, resume, and interview readiness scorecard.

---

## Assessment & Completion Criteria
- Module quizzes and practical checkpoints
- Minimum **70%** on theory assessments
- Successful completion of all mandatory labs
- Capstone incident response pass evaluation
- Submission of professional reporting portfolio

## Suggested Weekly Schedule
- **Weekdays:** 60-90 minutes study + lab prep
- **Weekend:** 3-5 hour deep lab execution + reporting
- **Mentor review:** Weekly feedback on findings and communication

## Final Outcome
By completing this path, learners demonstrate practical competency in:
- Security operations and incident response
- Network, endpoint, AD, cloud, and web defense
- Vulnerability management and compliance mapping
- Threat intelligence consumption and security reporting

This program is designed to bridge learning directly into cybersecurity job responsibilities.
