\# Ticket INC0012847 - Remote User Unable to Access Marketing Shared Drive



\## Ticket Information



| Field | Value |

|--------|-------|

| Ticket ID | INC0012870 |

| Priority | High |

| Category | Network Drive / File Share |

| Status | Resolved |

| Assigned To | Kenyotta Eave |



\---



\# Executive Summary



A remote employee reported being unable to access the Marketing Department shared drive. The mapped network drive appeared disconnected and generated a "Network path not found" error. After verifying VPN connectivity, file server availability, account permissions, and group memberships, the issue was traced to a stale network drive mapping. Recreating the mapped drive using the correct UNC path restored access.



\---



\# User Information



\*\*Name:\*\* Sarah Mitchell



\*\*Department:\*\* Marketing



\*\*Issue Reported:\*\*



> Unable to access the Marketing shared drive while working remotely. The mapped drive appears disconnected and displays "Network path not found."



\---



\# Environment



\- Windows Workstation

\- Remote User

\- VPN Connection

\- FILESERV01 File Server

\- Marketing Department Network Share



\---



\# Investigation Timeline



\## Step 1 – Gather Initial Information



Confirmed with the user:



\- Internet connectivity available

\- Email functioning normally

\- Unable to access Marketing shared drive

\- Error displayed:

&#x20; - \*\*Network path not found\*\*



\---



\## Step 2 – Verify VPN Connectivity



Verified:



\- VPN connected successfully



\### Result



✅ VPN functioning correctly.



\---



\## Step 3 – Verify File Server



Checked infrastructure.



Verified:



\- File Server Online



\### Result



✅ File server operational.



\---



\## Step 4 – Verify User Account



Checked Active Directory.



Verified:



\- Account Active

\- Marketing Group Membership

\- Domain Users

\- Printer-Users



\### Result



✅ Permissions appeared correct.



\---



\## Step 5 – Inspect Network Drive



Observed:



\- Marketing Department Drive displayed as disconnected.

\- Drive could not be opened.



\### Action Taken



Removed the stale network drive mapping.



\---



\## Step 6 – Obtain Correct Network Path



Asked the user for the location of the Marketing shared drive.



User provided:



```text

\\\\FILESERV01\\departments\\Marketing

```



\---



\## Step 7 – Recreate Network Drive



Mapped the drive using:



| Setting | Value |

|----------|-------|

| Drive Letter | D: |

| Folder | `\\\\FILESERV01\\departments\\Marketing` |



Successfully reconnected the shared drive.



\---



\# Root Cause



The workstation contained a stale/disconnected mapped network drive.



Although the VPN, file server, and user permissions were functioning correctly, the local drive mapping no longer pointed to an active connection. Recreating the mapping restored access.



\---



\# Resolution



\- Verified VPN connectivity

\- Verified file server status

\- Verified Active Directory account

\- Verified group memberships

\- Removed disconnected drive mapping

\- Mapped the drive using the correct UNC path

\- Confirmed access restored



\---



\# Customer Communication



\*\*Opening\*\*



> Thank you for contacting the IT Service Desk. I'll investigate the issue with your Marketing shared drive and work to restore your access.



\*\*Closing\*\*



> I've recreated your connection to the Marketing shared drive and confirmed that it's working again. Please let us know if you experience any additional issues.



\---



\# Lessons Learned



\- Always verify VPN connectivity before investigating file share issues.

\- Verify server availability before modifying client settings.

\- Confirm Active Directory permissions before assuming an access issue.

\- Remove stale drive mappings before recreating them.

\- Ask the user for additional information if documentation is unavailable.

\- Avoid guessing network paths; verify the correct UNC path whenever possible.



\---



\# Troubleshooting Process



```text

User reports disconnected drive

&#x20;       │

&#x20;       ▼

Verify Internet

&#x20;       │

&#x20;       ▼

Verify VPN

&#x20;       │

&#x20;       ▼

Verify File Server

&#x20;       │

&#x20;       ▼

Verify AD Account

&#x20;       │

&#x20;       ▼

Verify Group Membership

&#x20;       │

&#x20;       ▼

Inspect Mapped Drive

&#x20;       │

&#x20;       ▼

Remove Stale Mapping

&#x20;       │

&#x20;       ▼

Obtain Correct UNC Path

&#x20;       │

&#x20;       ▼

Map Network Drive

&#x20;       │

&#x20;       ▼

Verify Access

&#x20;       │

&#x20;       ▼

Resolve Ticket

```



\---



\# Skills Demonstrated



\- Active Directory Verification

\- VPN Troubleshooting

\- SMB File Share Troubleshooting

\- Network Drive Mapping

\- Windows File Explorer

\- Customer Communication

\- Root Cause Analysis

\- Incident Documentation

\- Tier 1 Help Desk Investigation



\---



\# Screenshots



\- Ticket Details

\- Remote Desktop Session

\- VPN Connected

\- File Server Status

\- User Account Verification

\- Group Membership Verification

\- Disconnected Network Drive

\- Remove Network Drive

\- Map Network Drive Window

\- UNC Path Configuration

\- Successful Drive Mapping

\- Ticket Resolved



\---



\# Final Status



\*\*Resolved\*\*



The Marketing Department network drive was successfully restored by recreating the mapped drive using the correct UNC path.



\*\*Final UNC Path\*\*



```text

\\\\FILESERV01\\departments\\Marketing

```

