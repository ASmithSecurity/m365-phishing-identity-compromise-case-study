# Project Overview & Takeaways

> **Purpose:** This file summarizes what this project is designed to demonstrate to employers, recruiters, and hiring managers reviewing my cybersecurity portfolio.

## Project Goal

The goal of this project is to demonstrate practical SOC support and incident response documentation skills using a simulated Microsoft 365 phishing and identity compromise scenario.

This project is designed to show that I can:

- Review suspicious activity in a structured way
- Identify common phishing and identity compromise indicators
- Document evidence clearly
- Explain security findings to non-technical partners
- Recommend containment steps
- Identify when escalation is needed
- Create repeatable documentation for future incidents
- Communicate calmly during a suspected security event

## Key Findings

| Finding | Why It Matters |
|---|---|
| Unusual sign-in activity | May indicate unauthorized access from an unfamiliar location, device, or IP address |
| Suspicious mailbox rules | Attackers may create rules to hide alerts, move messages, or maintain visibility |
| Possible external forwarding | May indicate data exposure or attacker persistence |
| User-reported phishing interaction | Possible initial access vector through credential theft |
| MFA status requires review | MFA enforcement can reduce account compromise risk |
| Active sessions require review | Existing sessions may remain valid unless revoked |

## Recommended Containment Actions

- [ ] Reset the affected user's password
- [ ] Revoke active user sessions
- [ ] Review and remove suspicious mailbox rules
- [ ] Disable unauthorized external forwarding
- [ ] Confirm MFA is enabled and enforced
- [ ] Review recent sign-in activity
- [ ] Search for similar phishing emails across the environment
- [ ] Check whether other users have similar mailbox rules
- [ ] Monitor the affected account for continued suspicious activity
- [ ] Document all actions taken

## MITRE ATT&CK Mapping

| Technique | Description |
|---|---|
| Phishing | User may have entered credentials into a fake login page |
| Valid Accounts | Attacker may have used stolen credentials to access the mailbox |
| Email Collection | Mailbox access may allow review of sensitive messages |
| Email Forwarding Rule | Attacker may create rules to forward, hide, or redirect messages |
| Account Discovery | Attacker may review account details after login |

## What This Project Shows Employers

This project demonstrates practical ability in:

### SOC Support

- Reviewing suspicious activity
- Organizing investigation notes
- Identifying possible compromise indicators
- Escalating when activity suggests higher risk

### Incident Communication

- Explaining security findings clearly
- Writing partner-facing summaries
- Translating technical details into plain language
- Providing calm, actionable next steps

### Documentation

- Creating internal SOC notes
- Building an investigation template
- Writing a knowledge base article
- Creating repeatable incident response documentation

### Microsoft 365 Security Concepts

- Reviewing suspicious sign-in behavior
- Understanding mailbox rule abuse
- Recognizing external forwarding risk
- Identifying phishing-related account compromise patterns
- Understanding the importance of MFA and session revocation

## Lessons Learned

This project reinforced that SOC support is not only about identifying suspicious activity. It is also about communicating clearly, documenting decisions, explaining risk, and helping partners understand what actions matter most.

A single unusual sign-in may not always confirm compromise. However, when unusual sign-in activity is combined with phishing interaction, suspicious mailbox rules, and possible forwarding behavior, the incident should be treated as high priority.

Clear documentation helps SOC teams, support teams, and partners stay aligned during active security incidents.

## Employer-Facing Summary

This project shows my ability to think through a realistic security support scenario from start to finish.

It includes:

- A simulated phishing and identity compromise scenario
- Key findings and risk explanation
- Recommended containment actions
- Internal SOC escalation notes
- Partner-facing communication
- A reusable investigation template
- A knowledge base article
- MITRE ATT&CK mapping
- Lessons learned from the investigation

The project is intended to demonstrate readiness for entry-level SOC support, cybersecurity support, IT security support, and incident response support roles.
