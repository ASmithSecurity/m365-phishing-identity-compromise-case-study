# Incident Flow Diagram

> **Project Note:** This diagram represents a simulated Microsoft 365 phishing and identity compromise investigation workflow. It does not contain real customer data, logs, credentials, or private information.

## Investigation Flow

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
```

## Workflow Explanation

This workflow shows the basic path of a suspected Microsoft 365 phishing and identity compromise incident.

The incident begins with a user receiving and interacting with a phishing email. After the user enters credentials, suspicious Microsoft 365 activity may appear, such as unusual sign-ins, inbox rule abuse, or unauthorized forwarding behavior.

A partner or customer then reports the suspicious activity. The SOC or support team reviews the reported behavior, documents findings, recommends containment steps, and provides a final partner-facing summary.

## Key Response Points

- Confirm the affected user account
- Review unusual sign-in activity
- Check for suspicious mailbox rules
- Check for unauthorized forwarding
- Reset the affected user's password
- Revoke active sessions
- Confirm MFA is enabled and enforced
- Document the incident timeline
- Provide clear partner-facing guidance
- Monitor for continued suspicious activity

## Containment Flow

| Step | Action | Purpose |
|---|---|---|
| 1 | Reset password | Prevent continued use of exposed credentials |
| 2 | Revoke sessions | Remove active attacker sessions |
| 3 | Review mailbox rules | Identify persistence or hiding behavior |
| 4 | Disable forwarding | Prevent continued data exposure |
| 5 | Confirm MFA | Strengthen account protection |
| 6 | Monitor activity | Confirm suspicious behavior does not continue |

## Lessons Demonstrated

This diagram demonstrates the importance of structured incident response, clear escalation, partner communication, and repeatable containment steps during suspected identity compromise events.
