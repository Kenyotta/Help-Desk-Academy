\# Ticket INC417718 - Company-Wide Email Outage



\## Ticket Information



| Field | Value |

|--------|-------|

| Ticket ID | INC417718 |

| Priority | High |

| Category | Email Infrastructure |

| Status | Resolved |

| Assigned To | Kenyotta Eave |



\---



\# Executive Summary



A company-wide email outage prevented all employees from sending and receiving email. Outlook displayed a "Disconnected" status for all users, and webmail was also unavailable. Investigation determined the Mail Server was operating in a degraded state. Rebooting the Mail Server restored email services across the organization.



\---



\# User Information



\*\*Reported By:\*\* Fiona Blake



\*\*Department:\*\* Legal



\*\*Location:\*\* Floor 2



\*\*Extension:\*\* x4550



\---



\# Reported Issue



The reporting user stated:



\- Nobody in the company could send or receive email.

\- Outlook displayed \*\*Disconnected\*\* for every employee.

\- Webmail failed to load.

\- Clients continued sending emails, but employees could not access them.



Business impact:



\- Company-wide communication outage.

\- Client communications halted.

\- Multiple departments affected.



\---



\# Environment



\- Corporate Email Infrastructure

\- Mail Server

\- Outlook Client

\- Webmail



\---



\# Investigation Timeline



\## Step 1 – Review Ticket



Analyzed the reported symptoms.



Key observations:



\- Entire organization affected.

\- Outlook disconnected.

\- Webmail unavailable.

\- Multiple users impacted.



This indicated an infrastructure issue rather than an individual workstation problem.



\---



\## Step 2 – Develop Initial Hypotheses



Possible causes considered:



\- Mail Server outage

\- Mail Server degraded state

\- Exchange or mail services failure

\- Network connectivity issue

\- DNS issue

\- Firewall or gateway issue



Client-side issues were considered unlikely because the entire organization was affected.



\---



\## Step 3 – Investigate Infrastructure



Accessed the Server Room.



Reviewed server status.



Observed:



\*\*Mail Server\*\*



Status:



> Degraded



No other infrastructure components were identified as unhealthy.



\---



\## Step 4 – Recovery



The simulator provided two recovery options:



\- Reboot

\- Shutdown



Shutdown would unnecessarily extend the outage.



Selected:



\*\*Reboot Mail Server\*\*



\---



\## Step 5 – Verify Resolution



Following the reboot:



\- Mail Server returned to a healthy operational state.

\- Outlook reconnected.

\- Webmail became accessible.

\- Company email services restored.



Ticket resolved.



\---



\# Root Cause



The Mail Server entered a degraded operational state, preventing both Outlook clients and webmail from communicating with the email service.



Rebooting the server restored normal mail services.



\---



\# Resolution



\- Reviewed business impact.

\- Confirmed issue affected the entire organization.

\- Investigated shared infrastructure.

\- Identified Mail Server degradation.

\- Rebooted Mail Server.

\- Verified restoration of email services.

\- Closed incident.



\---



\# Customer Communication



\## Opening



> Thank you for contacting the IT Service Desk. We are investigating a company-wide email issue affecting multiple users and will work to restore service as quickly as possible.



\## Closing



> Email services have been restored successfully. Outlook and webmail are functioning normally again. Please let us know if you experience any additional issues.



\---



\# Lessons Learned



\- Determine the scope of an issue before troubleshooting.

\- Company-wide outages usually indicate shared infrastructure problems.

\- Both Outlook and webmail failing points toward the email server rather than an individual workstation.

\- Investigate server health before making recovery decisions.

\- Choose the least disruptive recovery option available.

\- Always verify service restoration after infrastructure recovery.



\---



\# Troubleshooting Process



```text

Receive Incident

&#x20;       │

&#x20;       ▼

Determine Scope

&#x20;       │

&#x20;       ▼

Entire Company Affected

&#x20;       │

&#x20;       ▼

Investigate Shared Infrastructure

&#x20;       │

&#x20;       ▼

Mail Server Status

&#x20;       │

&#x20;       ▼

Server Degraded

&#x20;       │

&#x20;       ▼

Reboot Mail Server

&#x20;       │

&#x20;       ▼

Verify Email Services Restored

&#x20;       │

&#x20;       ▼

Close Incident

```



\---



\# Skills Demonstrated



\- Major Incident Identification

\- Infrastructure Troubleshooting

\- Server Health Assessment

\- Root Cause Analysis

\- Business Impact Evaluation

\- Incident Prioritization

\- Customer Communication

\- Service Restoration

\- Tier 1 Help Desk Operations



\---



\# Recommended Screenshots



\- Ticket Details

\- Server Room

\- Mail Server Status (Degraded)

\- Mail Server Reboot

\- Mail Server Healthy

\- Ticket Resolved



\---



\# Final Status



\*\*Resolved\*\*



A degraded Mail Server caused a company-wide email outage. Rebooting the server restored Outlook connectivity and webmail functionality, returning email services to normal operation.

