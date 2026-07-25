\# Ticket INC441437 - Unable to Connect to Network



\## Ticket Information



| Field | Value |

|--------|-------|

| Ticket ID | INC441437 |

| Priority | Medium |

| Category | Network Connectivity |

| Status | Resolved |

| Assigned To | Kenyotta Eave |



\---



\# Executive Summary



A Facilities employee reported being unable to access the internet while other employees remained connected. Initial investigation determined the issue was isolated to the user's workstation. The workstation displayed a "Cannot connect to this network" error. The wireless network profile was removed and recreated by forgetting the network, reconnecting, and re-entering the wireless password. Network connectivity was restored successfully.



\---



\# User Information



\*\*Name:\*\* Eugene Williams



\*\*Department:\*\* Facilities



\*\*Extension:\*\* 1089



\---



\# Reported Issue



The user reported:



\- Unable to access the internet.

\- Websites would not load.

\- Other employees were not experiencing the issue.

\- User had already disconnected and reconnected the network cable without success.



Business impact:



\- Unable to complete work requiring internet connectivity.

\- Quarterly inspection report due by Friday.



\---



\# Environment



\- Windows Workstation

\- Corporate Wireless Network

\- VPN Client



\---



\# Investigation Timeline



\## Step 1 – Review Ticket



Reviewed the reported symptoms.



Key observations:



\- Only one user affected.

\- Other employees had normal internet access.

\- Issue isolated to a single workstation.



\---



\## Step 2 – Develop Initial Hypotheses



Possible causes considered:



\- Network adapter issue

\- Wireless network profile issue

\- DHCP/IP configuration issue

\- VPN connectivity issue



Because the issue affected only one workstation, company-wide infrastructure problems were considered unlikely.



\---



\## Step 3 – Remote Investigation



Connected to the user's workstation.



Observed:



\- Windows displayed:



> Cannot connect to this network.



\- VPN client was disconnected.



Determined the VPN disconnection was a symptom of the workstation lacking network connectivity rather than the root cause.



\---



\## Step 4 – Corrective Action



Removed the saved wireless network profile by selecting:



\*\*Forget Network\*\*



Reconnected to the corporate wireless network.



Entered the wireless network password.



Successfully re-established the connection.



\---



\## Step 5 – Verify Resolution



Confirmed:



\- Workstation successfully connected to the wireless network.

\- Internet connectivity restored.

\- User verified normal functionality.



Ticket resolved.



\---



\# Root Cause



The workstation contained an invalid or corrupted saved wireless network profile, preventing successful authentication to the corporate wireless network.



Removing and recreating the wireless connection restored connectivity.



\---



\# Resolution



\- Reviewed reported symptoms.

\- Confirmed issue was isolated to one workstation.

\- Connected remotely.

\- Verified Windows network error.

\- Removed saved wireless network profile.

\- Reconnected to the wireless network.

\- Entered network credentials.

\- Verified internet connectivity restored.



\---







\# Lessons Learned



\- Determine whether a connectivity issue is isolated or organization-wide before troubleshooting.

\- A disconnected VPN is often a symptom rather than the root cause of a network connectivity issue.

\- Forgetting and reconnecting to a wireless network can resolve corrupted or outdated Wi-Fi profiles.

\- Verify connectivity after reconnecting before closing the incident.



\---



\# Troubleshooting Process



```text

Receive Ticket

&#x20;     │

&#x20;     ▼

Determine Scope

&#x20;     │

&#x20;     ▼

Single Workstation Affected

&#x20;     │

&#x20;     ▼

Remote Into Workstation

&#x20;     │

&#x20;     ▼

Observe "Cannot connect to this network"

&#x20;     │

&#x20;     ▼

Identify VPN Disconnection as Symptom

&#x20;     │

&#x20;     ▼

Forget Wireless Network

&#x20;     │

&#x20;     ▼

Reconnect to Wi-Fi

&#x20;     │

&#x20;     ▼

Enter Network Password

&#x20;     │

&#x20;     ▼

Verify Internet Connectivity

&#x20;     │

&#x20;     ▼

Resolve Ticket

```



\---



\# Skills Demonstrated



\- Windows Network Troubleshooting

\- Wireless Network Configuration

\- VPN Troubleshooting

\- Root Cause Analysis

\- Remote Desktop Support

\- Incident Documentation

\- Customer Communication

\- Tier 1 Help Desk Support



\---



\# Recommended Screenshots



\- Ticket Details

\- Remote Desktop Session

\- "Cannot connect to this network" Error

\- Wireless Network Settings

\- Forget Network Option

\- Successful Reconnection

\- Ticket Resolved



\---



\# Final Status



\*\*Resolved\*\*



The workstation was unable to connect because of an invalid or corrupted wireless network profile. Removing the saved profile and reconnecting to the corporate Wi-Fi restored internet connectivity.

