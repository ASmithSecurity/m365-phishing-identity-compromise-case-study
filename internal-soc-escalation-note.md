
# Internal SOC Notes

> **Project Note:** This is a simulated SOC documentation file created for cybersecurity portfolio development. It does not contain real customer data, real incident logs, credentials, or private information.

## Case Overview

This document contains internal SOC-style notes for a simulated Microsoft 365 phishing and identity compromise investigation.

The purpose of this file is to demonstrate how an analyst or SOC support specialist may document investigation details, evidence reviewed, potential impact, escalation reasoning, and recommended response actions.

## Alert Summary

| Field | Details |
|---|---|
| Alert Name | Suspected Microsoft 365 Account Compromise |
| Alert Type | Phishing / Identity Compromise |
| Severity | High |
| Status | Escalated for Containment Review |
| Affected Asset | User Mailbox / Microsoft 365 Account |
| Reported By | Partner / Customer |
| Primary Concern | Possible Credential Theft and Unauthorized Mailbox Access |

## Initial Report

A partner reported suspicious mailbox behavior after a user interacted with a suspected phishing email.

Reported activity included:

- Unusual sign-in behavior
- Suspicious mailbox activity
- Possible inbox rule abuse
- Possible external forwarding behavior
- User concern about missing or moved email messages

## Internal Analyst Summary

A suspected Microsoft 365 identity compromise was reviewed after a user reportedly interacted with a phishing email. The activity may indicate that the user's credentials were exposed and used to access the mailbox.

The reviewed behavior is consistent with common phishing-based compromise patterns, including suspicious sign-ins, mailbox rule changes, and possible forwarding activity.

Containment actions are recommended to prevent continued unauthorized access and reduce the risk of additional compromise.

## Evidence Reviewed

| Evidence | Analyst Notes |
|---|---|
| User-reported phishing interaction | User reportedly interacted with suspicious email content |
| Unusual sign-in behavior | Sign-in activity appeared inconsistent with expected user behavior |
| Suspicious mailbox activity | Mailbox behavior suggested possible unauthorized changes |
| Possible inbox rule abuse | Rule behavior may have been used to hide, move, delete, or redirect messages |
| Possible forwarding behavior | External forwarding may indicate data exposure or attacker persistence |
| MFA status | Requires validation to confirm whether stronger authentication was enabled and enforced |
| Active sessions | Should be revoked to remove potentially compromised sessions |

## Indicators of Compromise

Potential indicators reviewed in this simulated case:

- Successful sign-in from unfamiliar location
- Sign-in activity outside normal user behavior
- Suspicious mailbox rule creation
- Possible external forwarding configuration
- User interaction with suspected phishing link
- Unexpected mailbox changes
- Missing or moved messages
- Need for MFA and session review

## Potential Impact

The suspected activity could result in:

- Unauthorized mailbox access
- Credential theft
- Exposure of sensitive email content
- Hidden or redirected security alerts
- Unauthorized email forwarding
- Phishing emails sent from a trusted account
- Continued access through active sessions
- Possible compromise of additional users

## Initial Assessment

| Category | Assessment |
|---|---|
| Confidence | Medium to High |
| Urgency | High |
| Business Impact | Possible mailbox exposure and continued account misuse |
| Confirmed Scope | Single user in this simulated case |
| Escalation Needed | Yes |
| Recommended Status | Escalated for containment and partner follow-up |

## Recommended Containment Actions

- [ ] Reset the affected user's password
- [ ] Revoke active user sessions
- [ ] Review and remove suspicious inbox rules
- [ ] Disable unauthorized external forwarding
- [ ] Confirm MFA is enabled and enforced
- [ ] Review recent sign-in activity
- [ ] Search for similar phishing emails across the environment
- [ ] Review whether other users show similar mailbox rule changes
- [ ] Monitor the affected account after containment

## Escalation Criteria

Escalate further if any of the following are observed:

- Additional affected users are identified
- Suspicious sign-ins continue after password reset
- Suspicious mailbox rules reappear after removal
- External forwarding continues after containment
- Evidence suggests broader tenant compromise
- The affected account sent phishing emails to internal or external users
- The partner reports business impact or sensitive data exposure
- The affected account has privileged access

## Incident Timeline

| Time | Event |
|---|---|
| 08:15 | User receives suspicious email |
| 08:21 | User reportedly interacts with phishing link |
| 09:04 | Unusual sign-in activity observed |
| 09:10 | Suspicious mailbox rule behavior identified |
| 09:18 | Possible forwarding behavior observed |
| 09:35 | Partner reports suspicious mailbox activity |
| 09:45 | Investigation begins |
| 10:05 | Containment recommendations prepared |
| 10:30 | Partner begins password reset and MFA review |
| 11:00 | Incident summary and follow-up recommendations delivered |

## Suggested Internal Note

Suspected Microsoft 365 account compromise following reported phishing interaction. Activity reviewed includes unusual sign-in behavior, suspicious mailbox changes, possible inbox rule abuse, and potential forwarding behavior.

Recommended actions include password reset, session revocation, mailbox rule review, forwarding review, MFA validation, and continued monitoring.

Escalation is recommended if additional users are identified, suspicious activity continues after containment, or evidence suggests broader tenant compromise.

## MITRE ATT&CK Mapping

| Technique | Description |
|---|---|
| Phishing | User may have entered credentials into a fake login page |
| Valid Accounts | Attacker may have used stolen credentials to access the mailbox |
| Email Collection | Mailbox access may allow review of sensitive messages |
| Email Forwarding Rule | Attacker may create rules to forward, hide, or redirect messages |
| Account Discovery | Attacker may review account details after login |

## Analyst Notes

The highest priority is to confirm whether the suspicious access was authorized. If unauthorized, containment should focus on resetting credentials, revoking sessions, removing persistence mechanisms such as mailbox rules or forwarding, and validating MFA enforcement.

The partner-facing explanation should avoid unnecessary technical depth and focus on:

- What happened
- Why it matters
- What actions should be taken now
- What follow-up monitoring is recommended
- When escalation may be needed

## Closure Criteria

This incident can be considered contained when:

- [ ] Password reset is completed
- [ ] Active sessions are revoked
- [ ] Suspicious mailbox rules are removed
- [ ] Unauthorized forwarding is disabled
- [ ] MFA status is confirmed
- [ ] No additional suspicious sign-ins are observed
- [ ] No additional affected users are identified
- [ ] Partner confirms recommended actions were completed

## Lessons Learned

This simulated case reinforced the importance of structured documentation during suspected identity compromise incidents.

Strong SOC documentation should clearly capture:

- The reported issue
- Evidence reviewed
- Potential impact
- Recommended containment actions
- Escalation criteria
- Timeline of events
- Partner-facing next steps

Clear internal notes help SOC teams, support teams, and partners stay aligned during active security incidents.
```
