\# INC583175 - User Reports Slow Computer / Outlook Not Connecting



\## Learning Objective



Develop a structured troubleshooting methodology for performance complaints by distinguishing between perceived slowness and underlying network or application connectivity issues. Practice evidence-based troubleshooting, customer communication, and proper escalation procedures.



\---



\# Ticket Information



| Field | Value |

|-------|-------|

| Ticket ID | INC0012872 |

| Priority | Medium |

| Category | Performance / Network Connectivity |

| User | Mike Johnson |

| Department | Operations |

| Device | SD1076 |



\---



\# Incident Summary



Mike Johnson reported that his computer had become increasingly slow over the last several days. He explained that opening applications and documents took much longer than normal, Outlook frequently became unresponsive, and the entire workstation occasionally appeared to freeze.



\---



\# Business Impact



\- Reduced employee productivity

\- Unable to access Outlook

\- Unable to access company resources

\- Delays completing daily work



\---



\# Initial Assessment



Initial hypotheses included:



\- High CPU, memory, or disk utilization

\- Failing storage device

\- Windows update issues

\- Malware infection

\- Network connectivity problems

\- VPN connectivity issue



\---



\# Customer Interview



Information gathered from the user:



\- Computer has been slow for several days.

\- Performance issues affect nearly all applications.

\- Outlook and Microsoft Office applications are affected the most.

\- No new software has been installed.

\- Multiple restarts did not resolve the issue.

\- User was unaware of any company-wide outage.



\---



\# Investigation



\## Remote Desktop Session



Connected to the workstation to determine whether the issue affected the operating system globally or only specific applications.



\### Observations



\- Desktop responsive

\- Mouse responsive

\- File Explorer opened normally

\- Settings opened normally

\- Local documents opened normally

\- No obvious system lag observed



This indicated the workstation itself was functioning normally.



\---



\## Windows Inspection



Performed the following:



\- Installed pending Windows Updates

\- Ran Disk Cleanup

\- Performed Windows Security Full Scan

\- Removed detected items (if applicable)



Issue remained after maintenance.



\---



\## Network Investigation



Verified IP configuration.



\### ipconfig Results



IPv4 Address:

10.0.1.98



Default Gateway:

10.0.1.1



Configuration appeared valid.



\---



\## Connectivity Testing



Verified:



\- Gateway reachable

\- Internet connectivity

\- DNS resolution



Commands executed:



\- ping 10.0.1.1

\- ping 8.8.8.8

\- ping google.com



All tests completed successfully.



\---



\## Outlook Testing



Observed:



\- Outlook remained in "Trying to connect"

\- Internal company resources inaccessible

\- Browser continually loaded without displaying content



\---



\## VPN Investigation



Consulted internal VPN SOP.



Discovered:



User was \*\*not connected\*\* to the corporate VPN.



Connected VPN successfully.



VPN assigned address:



10.8.0.98



Verified tunnel status:



Active



Retested Outlook and internal resources.



Issue persisted.



\---



\## Asset Verification



Confirmed:



\- Device status: Active

\- Asset assignment correct



\---



\# Troubleshooting Timeline



1\. Interviewed user

2\. Established Remote Desktop session

3\. Verified workstation responsiveness

4\. Installed Windows Updates

5\. Performed Disk Cleanup

6\. Ran malware scan

7\. Verified IP configuration

8\. Tested gateway connectivity

9\. Tested internet connectivity

10\. Verified DNS resolution

11\. Reviewed VPN documentation

12\. Connected VPN

13\. Retested Outlook

14\. Retested company resources

15\. Verified asset status

16\. Escalated ticket



\---



\# Root Cause



Unable to determine during Tier 1 investigation.



Evidence indicated:



\- Workstation functioning normally

\- Internet connectivity operational

\- DNS operational

\- VPN connected successfully



Despite successful remediation attempts, Outlook and internal resources remained inaccessible.



Issue required additional investigation by higher-level support.



\---



\# Resolution



Performed all approved Tier 1 troubleshooting steps including:



\- Operating system maintenance

\- Malware scan

\- Windows updates

\- Network diagnostics

\- VPN verification

\- Asset verification



Escalated ticket with complete documentation after exhausting Tier 1 troubleshooting procedures.



\---



\# Escalation Notes



Escalated to higher-level support after confirming:



\- Local workstation healthy

\- Network connectivity operational

\- VPN active

\- Outlook still unable to connect

\- Internal resources still inaccessible



Provided complete troubleshooting history to prevent duplicate work.



\---



\# Lessons Learned



\- User-reported symptoms may not accurately identify the underlying problem.

\- Performance complaints should be validated through observation rather than assumption.

\- Always follow internal SOPs before escalating.

\- Verify VPN connectivity whenever internal resources are unavailable.

\- Evidence-based troubleshooting is more valuable than trying random fixes.

\- Knowing when to escalate is an important Tier 1 skill.



\---



\# Skills Demonstrated



\- Customer interviewing

\- Active listening

\- Root cause analysis

\- Windows troubleshooting

\- Network diagnostics

\- VPN troubleshooting

\- Malware remediation

\- Windows maintenance

\- Documentation

\- Professional escalation

\- Evidence-based troubleshooting



\---



\# Interview Talking Point



One of the most valuable lessons from this ticket was learning that customer-reported symptoms don't always identify the actual problem. The user believed the computer itself was slow, but through a structured investigation I verified the workstation was healthy, tested network connectivity, reviewed VPN configuration, performed system maintenance, and documented every troubleshooting step. When the issue remained unresolved after exhausting Tier 1 procedures, I escalated it with detailed findings, allowing the next support team to continue the investigation without repeating work.

