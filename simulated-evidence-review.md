# Simulated Evidence Review

> **Project Note:** This file contains simulated evidence for a Microsoft 365 phishing and identity compromise case study. No real logs, customer data, credentials, or private information are included.

## Evidence Review Overview

This document demonstrates how a SOC analyst or SOC support specialist might review and document simulated evidence during a suspected Microsoft 365 phishing and identity compromise investigation.

The simulated case involves a user who interacted with a phishing email, followed by suspicious sign-in behavior, mailbox rule activity, and possible external forwarding.

## Investigation Goals

- Review suspicious sign-in activity
- Identify possible unauthorized mailbox access
- Review mailbox rules for suspicious behavior
- Check for possible external forwarding
- Document indicators of compromise
- Recommend containment actions
- Provide clear partner-facing next steps

## Simulated Sign-In Activity Review

| Time | User | Source IP | Location | Result | Notes |
|---|---|---|---|---|---|
| 08:58 | user@example.com | 203.0.113.25 | Seattle, WA | Success | Expected user location |
| 09:04 | user@example.com | 198.51.100.44 | Unknown Region | Success | Unusual location; requires review |
| 09:06 | user@example.com | 198.51.100.44 | Unknown Region | Success | Same suspicious source observed again |
| 09:13 | user@example.com | 198.51.100.44 | Unknown Region | Success | Continued activity from suspicious source |
| 09:45 | user@example.com | 203.0.113.25 | Seattle, WA | Success | User returns from normal location |

## Sign-In Activity Assessment

The successful sign-ins from `198.51.100.44` are suspicious because they originate from an unfamiliar location and occur shortly after the user reportedly interacted with a phishing email.

This pattern may indicate that credentials were exposed and used by an unauthorized actor.

## Simulated Mailbox Rule Review

| Rule Name | Action | Suspicious? | Notes |
|---|---|---|---|
| Move Security Alerts | Move messages to Archive | Yes | Security-related emails moved out of inbox |
| Forward Invoice Messages | Forward externally | Yes | Possible data exposure or attacker monitoring |
| Newsletter Cleanup | Move newsletters to folder | No | Expected user behavior |
| Password Reset Filter | Move messages to RSS Subscriptions | Yes | May hide password reset or security notifications |

## Mailbox Rule Assessment

Several mailbox rules appear suspicious because they target security-related messages, password reset messages, or possible business-sensitive email content.

Attackers commonly use mailbox rules to hide security warnings, maintain visibility into conversations, or redirect messages after gaining unauthorized access.

## Simulated Forwarding Review

| Forwarding Type | Destination | Authorized? | Notes |
|---|---|---|---|
| External forwarding | external-mailbox@example.net | No | Suspicious forwarding destination |
| Internal forwarding | None observed | N/A | No approved internal forwarding identified |

## Forwarding Assessment

Unauthorized external forwarding may allow an attacker to continue receiving copies of email messages even after initial access is removed.

This should be disabled immediately if confirmed unauthorized.

## Indicators of Compromise

| Indicator | Status | Risk |
|---|---|---|
| User interacted with phishing email | Observed | Credential theft risk |
| Successful login from unfamiliar IP | Observed | Possible unauthorized access |
| Suspicious mailbox rule | Observed | Persistence / hiding activity |
| External forwarding | Observed | Possible data exposure |
| MFA status requires review | Unknown | Account protection gap |
| Active sessions require review | Unknown | Continued access risk |

## Analyst Notes

The simulated evidence suggests possible unauthorized mailbox access following a phishing interaction.

The strongest indicators are:

- Successful sign-ins from an unfamiliar location
- Suspicious mailbox rules targeting security-related messages
- Possible external forwarding behavior
- Timeline alignment between phishing interaction and unusual account activity

## Recommended Containment Actions

- [ ] Reset the affected user's password
- [ ] Revoke active sessions
- [ ] Remove suspicious mailbox rules
- [ ] Disable unauthorized external forwarding
- [ ] Confirm MFA is enabled and enforced
- [ ] Review recent sign-in activity
- [ ] Search for similar phishing messages across the environment
- [ ] Check whether other users have similar mailbox rules
- [ ] Monitor the affected account for continued suspicious activity

## Severity Assessment

| Category | Assessment |
|---|---|
| Severity | High |
| Confidence | Medium to High |
| Scope | Single user in this simulated case |
| Business Impact | Possible mailbox exposure |
| Escalation Needed | Yes |

## Escalation Reasoning

This case should be escalated because there are multiple indicators consistent with identity compromise, including successful suspicious sign-ins, mailbox rule abuse, and possible forwarding behavior.

Escalation is especially important if additional users are affected, if the suspicious activity continues after containment, or if sensitive data exposure is suspected.

## Partner-Facing Summary

The account showed activity that may indicate unauthorized access after a phishing interaction. Suspicious behavior included unusual sign-ins, mailbox rule changes, and possible forwarding behavior.

Recommended next steps are to reset the affected user's password, revoke active sessions, review and remove suspicious mailbox rules, disable unauthorized forwarding, confirm MFA enforcement, and monitor for additional suspicious activity.

## Lessons Learned

This simulated evidence review demonstrates the importance of connecting multiple weak signals into a stronger investigation narrative.

A single unusual login may not always confirm compromise, but unusual sign-ins combined with phishing interaction, suspicious mailbox rules, and forwarding behavior should be treated as a high-priority incident.

Clear documentation helps SOC teams explain what happened, why it matters, and what steps should be taken next.
