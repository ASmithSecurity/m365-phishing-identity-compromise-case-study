# Partner-Facing Incident Summary

> **Project Note:** This is a simulated cybersecurity portfolio document created for training and professional development. No real customer data, logs, credentials, or private information are included.

## Incident Summary

A suspected Microsoft 365 account compromise was reviewed after a user reportedly interacted with a phishing email and later experienced suspicious mailbox behavior.

The activity reviewed in this simulated case included:

- Unusual sign-in behavior
- Suspicious mailbox rules
- Possible email forwarding behavior
- User-reported phishing interaction
- Potential credential exposure

These findings are commonly associated with phishing-based identity compromise. In this type of incident, an attacker may use stolen credentials to access a mailbox, create rules to hide activity, forward messages externally, or attempt additional compromise from a trusted user account.

## Key Findings

| Finding | Why It Matters |
|---|---|
| Unusual sign-in activity | May indicate that the account was accessed from an unfamiliar location, device, or IP address |
| Suspicious mailbox rules | Attackers often create rules to hide alerts, move messages, or prevent users from seeing security warnings |
| Possible forwarding behavior | Email forwarding may expose sensitive messages or allow continued visibility into mailbox activity |
| User-reported phishing interaction | The user may have entered credentials into a fake login page |
| MFA status requires review | MFA can reduce the risk of unauthorized account access, but only if properly enabled and enforced |

## Recommended Immediate Actions

- [ ] Reset the affected user's password
- [ ] Revoke active user sessions
- [ ] Review and remove suspicious mailbox rules
- [ ] Disable unauthorized external forwarding
- [ ] Confirm multi-factor authentication is enabled and enforced
- [ ] Review recent sign-in activity for unfamiliar IP addresses, devices, or locations
- [ ] Search for similar phishing emails sent to other users
- [ ] Monitor the affected account for continued suspicious activity

## Plain-Language Explanation

The affected mailbox showed activity that may indicate unauthorized access.

The safest next step is to treat the account as potentially compromised, reset access, remove suspicious mailbox changes, and confirm stronger authentication controls are in place.

## Why This Matters

If an attacker gains access to a mailbox, they may be able to:

- Read sensitive messages
- Create forwarding rules
- Hide security alerts
- Send phishing emails to other users
- Attempt additional account compromise
- Maintain access through active sessions if they are not revoked

## Suggested Partner Response

The activity reviewed suggests the account may have been exposed through phishing. We recommend resetting the affected user's password, revoking active sessions, reviewing mailbox rules, disabling unauthorized forwarding, and confirming MFA enforcement.

Continued monitoring is recommended to confirm that suspicious activity does not continue after containment.

## Follow-Up Recommendations

After the immediate containment steps are completed, the partner should also:

1. Confirm whether other users received the same phishing email.
2. Review organization-wide forwarding rules.
3. Confirm MFA coverage across all users.
4. Educate the affected user on phishing indicators.
5. Monitor for additional suspicious sign-ins.
6. Document all actions taken during containment.
7. Review whether similar mailbox rules exist on other accounts.

## Example Customer Update

Hello,

We reviewed the reported Microsoft 365 mailbox activity and identified behavior commonly associated with possible account compromise, including unusual sign-in activity and suspicious mailbox changes.

At this time, we recommend resetting the affected user's password, revoking active sessions, reviewing mailbox rules, disabling unauthorized forwarding, and confirming MFA is enabled. These steps help reduce the risk of continued unauthorized access.

We also recommend reviewing whether other users received the same phishing email and continuing to monitor the account for additional suspicious activity.

Thank you.
