\# INC0012865 - Incorrect System Time and Time Zone Affecting Meetings



\## Learning Objective



Learn how to troubleshoot Windows date, time, and time synchronization issues that impact business applications, meeting scheduling, and file timestamps.



\---



\# Ticket Information



| Field | Value |

|-------|-------|

| Ticket ID | INC0012865 |

| Priority | High |

| Category | Windows Configuration |

| User | Kevin Park |

| Department | Sales |

| Location | Floor 2 |



\---



\# Incident Summary



Kevin Park reported that his workstation displayed the incorrect time and time zone. The computer was configured for Eastern Time even though he worked in the Central Time Zone. The incorrect system clock caused Team Chat meetings to appear at the wrong times, resulting in a missed meeting and incorrect file timestamps.



\---



\# Business Impact



\- Missed scheduled meeting

\- Three additional meetings scheduled later that day

\- Incorrect meeting times displayed

\- Incorrect file timestamps

\- Reduced productivity



\---



\# Initial Assessment



Based on the user's description, the initial hypotheses included:



\- Incorrect Windows time zone configuration

\- Windows Time synchronization issue

\- Time server synchronization failure

\- Domain time synchronization issue



\---



\# Customer Information



The user reported:



\- Computer configured for Eastern Time

\- Located in Central Time

\- Minutes appeared inaccurate

\- Restarting the computer did not resolve the issue



\---



\# Investigation



\## Remote Desktop Session



Established a remote session to verify the system's date, time, time zone, and synchronization settings.



\### Observations



Verified:



\- Current time displayed: 11:32 PM

\- Time Zone: Eastern Time

\- Set Time Automatically: Enabled

\- Sync Now option available



The investigation confirmed the workstation was configured with the incorrect time zone.



\---



\# Root Cause



The workstation was configured with the incorrect Windows time zone.



Although automatic time synchronization was enabled, Windows synchronized using the incorrect time zone configuration, causing calendar appointments and timestamps to display incorrectly.



\---



\# Resolution



Performed the following actions:



\- Changed Windows Time Zone from Eastern Time to Central Time

\- Initiated manual time synchronization using \*\*Sync Now\*\*

\- Verified the system clock updated correctly

\- Confirmed the ticket issue was resolved



\---



\# Verification



Confirmed:



\- Correct Central Time selected

\- Successful time synchronization

\- Correct system time displayed

\- Meeting times restored

\- Ticket resolved successfully



\---



\# Troubleshooting Timeline



1\. Reviewed incident details

2\. Connected via Remote Desktop

3\. Verified current system time

4\. Verified Windows time zone

5\. Confirmed automatic time synchronization enabled

6\. Changed time zone to Central Time

7\. Performed manual synchronization

8\. Verified correct system time

9\. Closed ticket



\---



\# Lessons Learned



\- Verify user-reported symptoms before making changes.

\- Time synchronization alone does not correct an incorrect time zone.

\- Incorrect system time can impact calendars, authentication, timestamps, and business productivity.

\- Always verify both the time zone and synchronization settings.

\- Validate the fix before closing the ticket.



\---



\# Skills Demonstrated



\- Windows Administration

\- Windows Time Service

\- Time Zone Configuration

\- Remote Desktop Support

\- Windows Settings

\- Root Cause Analysis

\- User Support

\- Ticket Documentation

\- Incident Resolution

\- Verification and Validation



\---



\# Interview Talking Point



This ticket demonstrated the importance of distinguishing between system time and time zone configuration. During the investigation, I verified the workstation settings rather than assuming the user's description was entirely accurate. I confirmed the computer was configured for the wrong time zone while automatic synchronization remained enabled. After correcting the time zone and forcing a manual synchronization, I verified the system clock and meeting times were accurate before resolving the incident.

