\# Ticket INC453563 - Cafeteria Printer Not Responding



\## Ticket Information



| Field | Value |

|--------|-------|

| Ticket ID | INC453563 |

| Priority | Medium |

| Category | Printer / Network Printing |

| Status | Resolved |

| Assigned To | Kenyotta Eave |



\---



\# Executive Summary



A Sales employee reported that the cafeteria printer appeared offline despite being powered on and stocked with paper. Investigation revealed the workstation was attempting to communicate with the printer using an outdated IP address. The stale printer was removed and re-added using the current TCP/IP address from the knowledge base. Printing functionality was successfully restored.



\---



\# User Information



\*\*Name:\*\* Rachel Green



\*\*Department:\*\* Sales



\*\*Extension:\*\* x5585



\*\*Printer:\*\* Cafeteria-Printer-E



\---



\# Reported Issue



The user reported:



\- Printer appeared offline.

\- Printer was powered on.

\- Printer had paper loaded.

\- Unable to print cafeteria menus.

\- Printer had been functioning normally several weeks earlier.



Business Impact:



\- Daily cafeteria menus could not be printed.

\- Event materials could not be produced.

\- Staff resorted to handwritten signage.



\---



\# Environment



\- Windows Workstation

\- Network Printer

\- TCP/IP Printer Connection



Printer IP Address:



10.0.2.54



\---



\# Investigation Timeline



\## Step 1 – Review Ticket



Reviewed the incident details.



Observed:



\- Printer reported as offline.

\- Hardware appeared operational.

\- Issue isolated to one workstation.



\---



\## Step 2 – Remote Support



Connected remotely to the user's workstation using the Remote Support tool.



Opened:



Settings → Devices



\---



\## Step 3 – Remove Stale Printer



Located the offline printer.



Removed the existing printer configuration.



\---



\## Step 4 – Re-add Printer



Selected:



Add Printer



↓



Add printer using TCP/IP address or hostname



Entered:



10.0.2.54



Windows successfully detected and installed the printer.



\---



\## Step 5 – Verification



Printed a Windows Test Page.



Confirmed with the user that:



\- Printer was online.

\- Test page printed successfully.

\- Normal printing resumed.



Ticket resolved.



\---



\# Root Cause



The workstation contained an outdated printer configuration that referenced the printer's previous IP address.



Because the printer's network IP had changed, Windows could no longer communicate with the device.



Removing the stale printer configuration and adding the printer using the current TCP/IP address restored communication.



\---



\# Resolution



\- Connected remotely.

\- Opened printer settings.

\- Removed offline printer.

\- Added printer using current TCP/IP address.

\- Verified successful installation.

\- Printed test page.

\- Confirmed functionality with the user.



\---





\---



\# Lessons Learned



\- Network printers often rely on static TCP/IP addresses.

\- An outdated printer IP can cause Windows to report the printer as offline even when the device is powered on.

\- Re-adding a printer using its current TCP/IP address restores communication when printer IP changes occur.

\- Always verify functionality with a test page before closing the incident.



\---



\# Troubleshooting Process



Receive Ticket

&#x20;       │

&#x20;       ▼

Determine Scope

&#x20;       │

&#x20;       ▼

Remote Into User Workstation

&#x20;       │

&#x20;       ▼

Locate Offline Printer

&#x20;       │

&#x20;       ▼

Remove Stale Printer Configuration

&#x20;       │

&#x20;       ▼

Add Printer Using TCP/IP Address

&#x20;       │

&#x20;       ▼

Enter Current Printer IP (10.0.2.54)

&#x20;       │

&#x20;       ▼

Print Test Page

&#x20;       │

&#x20;       ▼

Confirm With User

&#x20;       │

&#x20;       ▼

Resolve Ticket



\---



\# Skills Demonstrated



\- Windows Printer Administration

\- TCP/IP Printer Configuration

\- Remote Desktop Support

\- Printer Troubleshooting

\- Network Device Configuration

\- Incident Documentation

\- Customer Communication

\- Tier 1 Help Desk Support



\---



\# Recommended Screenshots



\- Original Ticket

\- Remote Support Session

\- Printer Settings

\- Remove Printer

\- Add Printer Wizard

\- TCP/IP Address Entry

\- Successful Test Page

\- Ticket Resolved



\---



\# Final Status



\*\*Resolved\*\*



The workstation was configured with an outdated printer connection after the cafeteria printer's IP address changed. Recreating the printer using the current TCP/IP address restored normal printing.

