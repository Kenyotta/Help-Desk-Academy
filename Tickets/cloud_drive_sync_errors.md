\# Ticket INC500770 - Cloud Drive Sync Errors and Duplicate Files



\## Ticket Information



| Field | Value |

|--------|-------|

| Ticket ID | INC500770 |

| Priority | Medium |

| Category | Cloud Storage / Synchronization |

| Status | Resolved |

| Assigned To | Kenyotta Eave |



\---



\# Executive Summary



A user reported repeated cloud drive synchronization errors and duplicate file prompts after installing a screen saver from an online source. Investigation determined the cloud drive had not synchronized for some time. A manual synchronization successfully completed, restoring normal cloud drive operation and eliminating the reported issue.



\---



\# User Information



\*\*Name:\*\* Derek Chang



\*\*Employee ID:\*\* EMP-4105



\*\*Extension:\*\* x4305



\*\*Computer:\*\* SD1073



\---



\# Reported Issue



The user reported:



\- Cloud Drive Sync Error

\- Duplicate versions of files being detected

\- Prompt asking whether to \*\*Keep Both\*\* or \*\*Overwrite\*\*

\- Issue began Monday

\- Recently installed a screen saver downloaded from an online website



\---



\# Environment



\- Windows Workstation

\- Cloud Storage Service

\- Corporate Network



\---



\# Investigation Timeline



\## Step 1 – Review Ticket



Reviewed the reported symptoms.



Initial observations:



\- Duplicate file conflicts

\- Synchronization errors

\- Recent software installation



\---



\## Step 2 – Develop Initial Hypotheses



Possible causes considered:



\- Cloud sync client issue

\- Corrupted synchronization cache

\- Multiple folders syncing the same content

\- Recently installed third-party software

\- Malware or unwanted software



No assumptions were made before gathering evidence.



\---



\## Step 3 – Remote Investigation



Connected to the user's workstation.



Opened File Explorer.



Navigated to:



Cloud Drive



Observed message:



> Last synced a while ago – some files may be missing.



A \*\*SYNC\*\* option was available.



\---



\## Step 4 – Perform Manual Synchronization



Selected \*\*SYNC\*\*.



Result:



> All files synced successfully.



\---



\## Step 5 – Verify Resolution



Confirmed synchronization completed successfully.



User verified:



\- Sync errors no longer appearing.

\- Cloud drive functioning normally.



\---



\# Root Cause



The cloud storage client had fallen behind on synchronization.



Because synchronization had not completed recently, the cloud service generated duplicate file conflict prompts.



Performing a manual synchronization restored the cloud drive to a healthy state.



\---



\# Resolution



\- Reviewed reported symptoms.

\- Connected to the workstation.

\- Inspected Cloud Drive status.

\- Identified outdated synchronization.

\- Initiated manual synchronization.

\- Confirmed successful sync.

\- Verified issue resolved with the user.



\---



\# Customer Communication



\## Opening



> Thank you for contacting the IT Service Desk. I'll investigate the cloud drive synchronization issue and determine why duplicate file prompts are occurring.



\## Closing



> Your cloud drive has successfully synchronized and appears to be functioning normally again. Please let us know if the issue returns or if you continue receiving duplicate file notifications.



\---



\# Lessons Learned



\- Always investigate the application's current status before assuming corruption or malware.

\- Follow the evidence rather than the most concerning possibility.

\- Manual synchronization can resolve stale cloud synchronization states.

\- Verify functionality with the user before closing the incident.

\- Recently installed software should be documented and investigated if symptoms persist, even when it is not the immediate cause.



\---



\# Troubleshooting Process



```text

Review Ticket

&#x20;     │

&#x20;     ▼

Develop Initial Hypotheses

&#x20;     │

&#x20;     ▼

Remote Into Workstation

&#x20;     │

&#x20;     ▼

Inspect Cloud Drive Status

&#x20;     │

&#x20;     ▼

Identify Outdated Synchronization

&#x20;     │

&#x20;     ▼

Run Manual Sync

&#x20;     │

&#x20;     ▼

Verify Synchronization Success

&#x20;     │

&#x20;     ▼

Confirm User Issue Resolved

&#x20;     │

&#x20;     ▼

Close Ticket

```



\---



\# Skills Demonstrated



\- Tier 1 Help Desk Troubleshooting

\- Root Cause Analysis

\- Cloud Storage Support

\- Remote User Assistance

\- Customer Communication

\- Incident Documentation

\- Evidence-Based Troubleshooting



\---



\# Recommended Screenshots



\- Ticket Details

\- Remote Desktop Session

\- Cloud Drive Status ("Last synced a while ago")

\- Manual Sync Button

\- Successful Synchronization

\- Ticket Resolved



\---



\# Final Status



\*\*Resolved\*\*



Manual synchronization restored the cloud drive to a healthy state, eliminating the synchronization errors and duplicate file prompts.

