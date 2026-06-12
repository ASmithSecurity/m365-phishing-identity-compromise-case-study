# SOC Investigation Template

> **Purpose:** This template provides a repeatable structure for documenting security alerts, suspected compromises, phishing reports, suspicious logins, endpoint alerts, and other SOC-style investigations.

## Alert Summary

| Field | Details |
|---|---|
| Alert Name |  |
| Date / Time |  |
| Severity | Low / Medium / High / Critical |
| Status | Open / Investigating / Escalated / Contained / Closed |
| Affected User |  |
| Affected Host |  |
| Source IP |  |
| Destination IP / Domain |  |
| Related Indicators |  |

## Initial Triage Questions

- What triggered the alert or report?
- Who or what asset is affected?
- Is this activity expected or unusual?
- Is there evidence of unauthorized access?
- Is there evidence of phishing, malware, or suspicious account behavior?
- Are other users, endpoints, or systems affected?
- Does the issue require escalation?

## What Happened?

Briefly explain the alert in plain language.

Example:

A suspicious login was observed for a user account from an unfamiliar location. The activity may indicate credential compromise and requires additional validation.

## Evidence Reviewed

- 
- 
- 

## Indicators of Compromise

| Indicator | Notes |
|---|---|
| Suspicious IP Address |  |
| Unusual Login Location |  |
| Suspicious Mailbox Rule |  |
| External Forwarding |  |
| Malicious URL |  |
| File Hash |  |
| Suspicious Process |  |
| Affected User / Host |  |

## Analysis

Explain why the activity appears benign, suspicious, or malicious.

Consider:

- Was the activity expected for this user?
- Was the login location unusual?
- Was the device known or unknown?
- Were mailbox rules or forwarding changes observed?
- Was there evidence of phishing interaction?
- Were multiple users or systems affected?
- Did the activity continue after containment?

## Potential Impact

Describe what systems, users, or data may be affected.

Examples:

- Unauthorized mailbox access
- Credential theft
- Suspicious forwarding behavior
- Hidden security notifications
- Exposure of sensitive email content
- Malware execution
- Lateral movement risk
- Additional user compromise

## Recommended Actions

- [ ] Validate whether the activity was expected
- [ ] Contact the affected user or partner for confirmation
- [ ] Reset password if compromise is suspected
- [ ] Revoke active sessions
- [ ] Review MFA status
- [ ] Review mailbox rules and forwarding
- [ ] Search for similar activity across the environment
- [ ] Block malicious indicators if confirmed
- [ ] Escalate to SOC / security team if needed
- [ ] Document all actions taken

## Escalation Decision

**Escalate:** Yes / No

**Reason:**

Explain why the issue should or should not be escalated.

## Severity Reasoning

| Severity | Criteria |
|---|---|
| Low | Suspicious but low-confidence activity with limited impact |
| Medium | Suspicious activity affecting one user or asset with possible security impact |
| High | Likely compromise, successful suspicious login, malware execution, or active incident |
| Critical | Widespread compromise, ransomware, major outage, or confirmed business impact |

## Customer / Partner-Friendly Summary

Write a short explanation that a non-technical customer could understand.

Example:

The account showed activity that may indicate unauthorized access. Recommended next steps are to reset the password, revoke active sessions, review mailbox rules, and confirm MFA is enabled.

## Closure Criteria

This investigation can be closed when:

- [ ] The alert has been reviewed
- [ ] Evidence has been documented
- [ ] Severity has been assigned
- [ ] Recommended actions have been provided
- [ ] Escalation decision has been documented
- [ ] Partner or internal stakeholder has been updated
- [ ] No additional suspicious activity is observed

## Lessons Learned

Document what this alert reinforced or taught.

Examples:

- Importance of reviewing mailbox rules after suspected phishing
- Importance of revoking sessions after password reset
- Importance of clear partner communication during incidents
- Importance of documenting timelines and containment actions
