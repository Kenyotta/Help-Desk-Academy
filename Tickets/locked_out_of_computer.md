\# Ticket INC976636 - Expired Password and Account Unlock



\## Ticket Information



| Field | Value |

|--------|-------|

| Ticket ID | INC976636 |

| Priority | Critical |

| Category | Account Access |

| Status | Resolved |

| Assigned To | Kenyotta Eave |



\---



\# Executive Summary



A Finance employee reported being unable to sign into their workstation on the day SEC quarterly reports were due. Investigation in Active Directory revealed the user's password had expired. The account was unlocked, the password was reset, and a temporary password was issued, restoring access.



\---



\# User Information



\*\*Name:\*\* Derek Chambers



\*\*Employee ID:\*\* EMP-0445



\*\*Department:\*\* Finance



\*\*Extension:\*\* 4010



\---



\# Reported Issue



The user reported being locked out of their workstation and stated that SEC quarterly reports were due that day. The user expressed urgency due to the business impact.



\---



\# Environment



\- Windows Domain Environment

\- Active Directory

\- Corporate Workstation



\---



\# Investigation Timeline



\## Step 1 – Review Ticket



Reviewed the voicemail and identified:



\- User unable to access workstation

\- Critical business deadline

\- Finance department

\- High business impact



\---



\## Step 2 – Develop Initial Hypotheses



Possible causes considered:



\- Account lockout

\- Forgotten password

\- Password expired

\- MFA issue



\---



\## Step 3 – Investigate Active Directory



Located Derek Chambers' account.



Observed:



\- Password expired



Further review confirmed the account also required unlocking.



\---



\## Step 4 – Restore Account Access



Performed the following actions:



\- Unlocked Active Directory account

\- Reset password

\- Generated temporary password

\- Communicated temporary credentials to the user



\---



\## Step 5 – Verify Resolution



Confirmed the user successfully regained access to the workstation using the temporary password.



Ticket resolved.



\---



\# Root Cause



The user's Active Directory password had expired, preventing successful authentication. The account also required unlocking before access could be restored.



\---



\# Resolution



\- Investigated Active Directory account status

\- Confirmed password expiration

\- Unlocked account

\- Reset password

\- Issued temporary password

\- Verified successful login



\---



\# Customer Communication



\## Opening



> Thank you for contacting the IT Service Desk. I'll review your account and determine why you're unable to sign in.



\## Closing



> Your account has been unlocked and your password has been reset. I've provided a temporary password so you can sign in immediately. You'll be prompted to create a new password after logging in.



\---



\# Lessons Learned



\- Never assume "locked out" automatically means a forgotten password.

\- Verify account status in Active Directory before making changes.

\- Password expiration and account lockout can occur simultaneously.

\- Prioritize high business impact incidents appropriately.

\- Verify access has been restored before closing the incident.



\---



\# Troubleshooting Process



```text

Receive Ticket

&#x20;     │

&#x20;     ▼

Review Business Impact

&#x20;     │

&#x20;     ▼

Investigate Active Directory

&#x20;     │

&#x20;     ▼

Password Expired

&#x20;     │

&#x20;     ▼

Unlock Account

&#x20;     │

&#x20;     ▼

Reset Password

&#x20;     │

&#x20;     ▼

Provide Temporary Password

&#x20;     │

&#x20;     ▼

Verify User Login

&#x20;     │

&#x20;     ▼

Resolve Ticket

```



\---



\# Skills Demonstrated



\- Active Directory User Management

\- Password Reset

\- Account Unlock

\- Authentication Troubleshooting

\- Incident Prioritization

\- Customer Communication

\- Root Cause Analysis

\- Tier 1 Help Desk Support



\---



\# Recommended Screenshots



\- Ticket Details

\- Active Directory User Account

\- Password Expired Status

\- Unlock Account

\- Password Reset

\- Temporary Password Issued

\- Ticket Resolved



\---



\# Final Status



\*\*Resolved\*\*



The user's password had expired and the account required unlocking. After unlocking the account, resetting the password, and issuing temporary credentials, the user successfully regained access to the workstation.

