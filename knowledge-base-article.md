# Knowledge Base Article

## Title

How to Respond to Suspected Microsoft 365 Phishing and Mailbox Compromise

> **Project Note:** This is a simulated knowledge base article created for cybersecurity portfolio development. It does not contain real customer data, real incident logs, credentials, or private information.

## Purpose

This article provides a repeatable response process for suspected Microsoft 365 account compromise involving phishing, unusual sign-ins, suspicious mailbox rules, or unauthorized forwarding.

The goal is to help support teams, SOC analysts, and partners quickly understand what to review, what containment steps to take, and when escalation may be required.

## Common Signs of Microsoft 365 Account Compromise

A Microsoft 365 account may be compromised if any of the following are observed:

- User interacted with a phishing email
- Unusual sign-in activity appears in the account
- Sign-ins occur from unfamiliar locations or IP addresses
- Suspicious mailbox rules are created
- Emails are missing, moved, deleted, or hidden
- External forwarding is enabled without authorization
- User reports sent emails they did not send
- Multiple users report receiving phishing emails from the account
- MFA prompts occur unexpectedly
- Security alerts or password reset emails are moved out of the inbox

## Why Mailbox Rules Matter

Attackers may create mailbox rules after gaining access to an account.

These rules can be used to:

- Hide security alerts
- Move password reset emails
- Delete warning messages
- Forward emails externally
- Monitor sensitive conversations
- Maintain visibility into mailbox activity

Because of this, mailbox rule review is an important step in suspected Microsoft 365 compromise investigations.

## Response Checklist

- [ ] Confirm the affected user account
- [ ] Confirm whether the user interacted with a phishing email
- [ ] Review recent sign-in activity
- [ ] Identify unfamiliar IP addresses, devices, or locations
- [ ] Reset the affected user's password
- [ ] Revoke active sessions
- [ ] Review and remove suspicious mailbox rules
- [ ] Disable unauthorized external forwarding
- [ ] Confirm MFA is enabled and enforced
- [ ] Search for similar phishing emails across the environment
- [ ] Review whether other users show similar suspicious activity
- [ ] Monitor the affected account after containment
- [ ] Document all actions taken

## Recommended Containment Steps

### 1. Reset the User Password

Resetting the password helps prevent continued access using exposed credentials.

### 2. Revoke Active Sessions

Revoking sessions is important because an attacker may still have an active session even after the password is changed.

### 3. Review Mailbox Rules

Look for rules that:

- Move emails to hidden folders
- Delete messages automatically
- Forward emails externally
- Target security-related words
- Hide password reset or MFA notifications

### 4. Disable Unauthorized Forwarding

Unauthorized forwarding may allow an attacker to continue receiving messages even after initial access is removed.

### 5. Confirm MFA Enforcement

Confirm that MFA is enabled and properly enforced for the affected user.

### 6. Review Sign-In Activity

Review recent sign-ins for:

- Unfamiliar locations
- Unknown devices
- Suspicious IP addresses
- Unusual login times
- Repeated failed attempts
- Successful logins from unexpected regions

### 7. Search for Similar Activity

Check whether other users received the same phishing email or show similar mailbox behavior.

## When to Escalate

Escalate the incident if:

- Multiple users are affected
- Suspicious sign-ins continue after password reset
- Suspicious mailbox rules reappear
- External forwarding continues after containment
- The affected account sent phishing emails
- The account has privileged access
- Sensitive data exposure is suspected
- The partner reports business impact

## Partner-Friendly Explanation

A suspected Microsoft 365 account compromise should be treated seriously because an attacker may have accessed the mailbox using stolen credentials.

The most important steps are to reset the password, revoke active sessions, review mailbox rules, disable unauthorized forwarding, and confirm MFA is enabled. These actions help remove unauthorized access and reduce the chance of continued mailbox misuse.

## Example Support Response

Hello,

We reviewed the reported Microsoft 365 mailbox activity and identified behavior that may be consistent with account compromise.

Recommended next steps are to reset the affected user's password, revoke active sessions, review and remove suspicious mailbox rules, disable unauthorized forwarding, and confirm MFA enforcement.

We also recommend reviewing whether other users received the same phishing message and continuing to monitor the account for additional suspicious sign-in or mailbox activity.

Thank you.

## Documentation Best Practices

When documenting this type of incident, include:

- Affected user
- Date and time of report
- Summary of suspicious behavior
- Evidence reviewed
- Sign-in activity notes
- Mailbox rule findings
- Forwarding findings
- Recommended containment steps
- Partner communication notes
- Escalation decision
- Closure criteria

## Closure Criteria

This case can be closed when:

- [ ] Password reset is completed
- [ ] Active sessions are revoked
- [ ] Suspicious mailbox rules are removed
- [ ] Unauthorized forwarding is disabled
- [ ] MFA status is confirmed
- [ ] No additional suspicious sign-ins are observed
- [ ] No additional affected users are identified
- [ ] Partner confirms recommended actions were completed
- [ ] Final incident notes are documented

## Key Takeaways

- Phishing can lead to credential theft and mailbox compromise.
- Password reset alone may not be enough if active sessions remain valid.
- Mailbox rules and forwarding should always be reviewed.
- Clear partner communication is critical during security incidents.
- Repeatable documentation helps improve consistency and response quality.
