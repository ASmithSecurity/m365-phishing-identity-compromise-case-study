# Microsoft 365 Phishing & Identity Compromise Incident Case Study

> **Project Note:** This is a simulated cybersecurity portfolio project created for educational and professional development purposes. It does not contain real customer data, real incident data, private logs, credentials, or confidential information.

## Project Overview

This project is a simulated incident response case study focused on a suspected Microsoft 365 phishing and identity compromise scenario.

The purpose of this project is to demonstrate SOC support skills including incident communication, investigation documentation, partner-facing summaries, escalation notes, containment planning, and knowledge base writing.

This project is aligned with entry-level SOC Support Specialist, Cybersecurity Support Analyst, and IT Security Support roles.

## Scenario

A partner reports that an employee received a phishing email and later noticed suspicious Microsoft 365 mailbox behavior.

Reported activity includes:

- Unusual sign-in behavior
- Suspicious mailbox rules
- Possible external forwarding
- Missing or moved messages
- Potential credential exposure
- Partner request for containment guidance

The goal of the investigation is to determine whether the behavior is consistent with identity compromise and provide clear next steps to contain the issue.

## Skills Demonstrated

- SOC alert triage concepts
- Phishing investigation fundamentals
- Microsoft 365 identity compromise analysis
- Mailbox rule abuse review
- Partner-facing incident communication
- Internal SOC documentation
- Escalation reasoning
- Containment and remediation planning
- Knowledge base article writing
- Incident timeline documentation
- Technical findings translated into plain language

## Tools & Concepts Used

- Microsoft 365 security concepts
- Entra ID / Azure AD sign-in behavior concepts
- Mailbox rule abuse indicators
- Multi-factor authentication review
- Session revocation
- Password reset procedures
- SIEM and log analysis concepts
- MITRE ATT&CK mapping
- Incident response lifecycle
- SOC documentation practices

## Repository Contents

| File | Purpose |
|---|---|
| [`partner-facing-summary.md`](partner-facing-summary.md) | Customer/partner-friendly explanation of the suspected incident and recommended actions |
| [`internal-soc-escalation-note.md`](internal-soc-escalation-note.md) | Internal SOC-style escalation note with evidence, impact, and escalation criteria |
| [`investigation-template.md`](investigation-template.md) | Reusable SOC investigation template for documenting future alerts |
| [`knowledge-base-article.md`](knowledge-base-article.md) | Mock knowledge base article for responding to Microsoft 365 phishing and mailbox compromise |
| [`incident-flow-diagram.md`](incident-flow-diagram.md) | Text-based incident workflow diagram showing investigation and containment flow |
| [`simulated-evidence-review.md`](simulated-evidence-review.md) | Simulated sign-in, mailbox rule, forwarding, and indicator review |
| [`screenshots/`](screenshots/) | Folder for project screenshots and documentation previews |
| [`notes/`](notes/) | Folder for additional investigation notes |
| [`resources/`](resources/) | Folder for supporting resources and references |

## Simulated Alert Summary

| Field | Details |
|---|---|
| Alert Type | Suspected Microsoft 365 account compromise |
| Severity | High |
| Affected Asset | User mailbox / Microsoft 365 account |
| Reported By | Partner / Customer |
| Primary Concern | Possible credential theft and unauthorized mailbox access |

## Reported Symptoms

- User received and interacted with a suspicious email
- Unusual sign-in activity was observed
- Unexpected mailbox forwarding behavior was identified
- Suspicious inbox rules were discovered
- User reported missing or moved messages
- Partner requested guidance on containment and next steps

## Investigation Workflow

1. Confirm the affected user account.
2. Review the phishing report and user interaction timeline.
3. Review sign-in activity for unfamiliar IP addresses, devices, or locations.
4. Check mailbox rules for suspicious movement, deletion, forwarding, or hiding behavior.
5. Identify whether external forwarding is enabled.
6. Confirm whether MFA is enabled and enforced.
7. Determine whether active sessions should be revoked.
8. Document findings in an internal SOC note.
9. Provide partner-facing containment recommendations.
10. Create a knowledge base article for repeatable response handling.

## Incident Flow

```text
User receives phishing email
        |
        v
User clicks link and enters credentials
        |
        v
Unusual Microsoft 365 sign-in detected
        |
        v
Suspicious mailbox rule or forwarding behavior observed
        |
        v
Partner reports suspicious mailbox activity
        |
        v
SOC reviews indicators and documents findings
        |
        v
Containment recommendations provided
        |
        v
Password reset, session revocation, mailbox rule cleanup, MFA review
        |
        v
Partner receives final summary and follow-up recommendations
