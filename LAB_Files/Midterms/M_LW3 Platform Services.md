![image](https://github.com/user-attachments/assets/ea5698bf-76b6-4475-aa1f-984127b56437)

# **SYSADM1 – Platform Services**
# **Requirement:** 
- A virtual machine running Windows Server

**Objective/s:**

To analyze IIS logs in the Event Viewer to identify critical web service metrics, understand common error codes, and learn how to monitor the health of web applications.

**Instructions**

**Part 1: Opening Event Viewer and Loading Logs**

1. Access the event viewer in the server.  
1. From the event viewer, explore the windows log and list down its major categories 

![image](https://github.com/user-attachments/assets/0f10839a-59fb-45c4-8ad6-0fede8f8a592)

- **There are five major categories under the Windows Logs: They are the Application, Security, Setup, System and Forwarded Events.**

**Part 2: Filtering and Analyzing IIS Events**

1. Apply filter to the windows log categories to display errors for the past 12 hours.

![image](https://github.com/user-attachments/assets/f2998f5b-38f4-41a2-afec-3747eceb8b54)

- **There are 8 Error Events, 4 from the source of ‘Security-SPP’, 2 from ‘Service Control Manager’ and 1 each from ‘Perflib’ and ‘Time-Service’.** 


1. **Identify Critical Events** or recurring events. 

![image](https://github.com/user-attachments/assets/14159196-2801-4e73-93ef-0e390fb42701)

- **Total number of Event are 24, having 16 Warnings and 8 Erros**

1. **Analyze the Events**:
   1. For each critical or recurring event, **record the following details**:
      1. **Event ID**
      1. **Source**
      1. **Timestamp**
      1. **Description**

![image](https://github.com/user-attachments/assets/1671baaf-f429-48fb-a1b8-94ba003af7d0)

-----
**Part 3: Troubleshooting and Solution Development**

1. Review the logs and check for recurring errors. 
- **The logs revealed several recurring errors over a 12-hour period, including issues from the Security-SPP, Service Control Manager, Perflib, and Time-Service sources.** 

1. Is there a specific time or pattern to these errors?
- **Upon analyzing the timestamps, I observed that these errors tend to occur around the same timeframe. Most of the critical events, such as the** NETLOGON **and** Perflib **errors.**

1. Draft a Troubleshooting Report:
   1. Based on the events found, create a short report with the following sections:
-----
**Report Structure**

**1.** Overview

- **The logs revealed multiple error events occurring within a 12-hour timeframe, indicating issues that need troubleshooting to ensure web services' health. Errors include application and service-related issues, impacting system functionality.**

**2.** Key Findings

- List the critical events you found. Example:
  - **Event ID 503**: Application pool stopped at 10:05 AM.
  - **Event ID 404**: Page not found error at 11:15 AM.

- **Event ID 6006 (Winlogon):** Indicates the system shutdown at 9:28:08 AM.
- **Event ID 1014 (Security-SPP):** Related to activation or licensing issues at 9:19:56 AM.
- **Event ID 5781 (NETLOGON):** Suggests potential DNS configuration problems at 9:30:29 AM
- **Event ID 7030 (Service Control Manager):** Highlights a failed service start at 9:21:40 AM
- **Event ID 1008 (Perflib):** Performance library errors indicate registry misconfigurations at 9:26:24 AM.

**3.** Root Causes and Solutions

- Describe the likely cause of each error and how you would fix it. 

![image](https://github.com/user-attachments/assets/0ee27349-8eff-4461-b88e-090e6fb35ddf)

-----
**Part 4: Reflection Questions**

1. What are the most common causes of a **503 Service Unavailable** error?

1. How would you **monitor login attempts** to detect potential security threats?

1. Why is **monitoring logs** in Event Viewer important for administrators?
- During the Lab Activity I noticed and realized that monitoring logs in Event Viewer is crucial for administrators because it provides insights into the health and performance of the system. Logs capture important events, such as hardware failures, application errors, and security incidents. By analyzing these logs, administrators can proactively address issues, improve troubleshooting processes, and ensure compliance with security policies. It also aids in forensic analysis when investigating incidents, making it an essential practice for maintaining system integrity and reliability.

Grading Rubric

|**Criteria**|**Excellent**|**Good**|**Needs Improvement**|**Poor**|**Points**|||
| :- | :- | :- | :- | :- | :- | :- | :- |
|**Log Analysis**|Identifies all key events (503, 404, 500, etc.) with accurate event details.|Identifies most key events with minor errors in details.|Identifies some events, but with incomplete or incorrect details.|Fails to identify key events or provides incorrect details.|/10|||
|**Troubleshooting Solutions**|Proposes logical, effective solutions to all identified issues.|Solutions are mostly correct but miss some key points.|Solutions are somewhat vague or incomplete.|Solutions are unclear or incorrect.|/10|||
|**Report Structure & Clarity**|Well-organized report with all sections clearly completed.|Report is mostly organized with minor formatting issues.|Report is disorganized or missing sections.|Report is unclear or incomplete.|/10|||
|**Recommendations for Monitoring**|Provides thoughtful, proactive recommendations to prevent future issues.|Recommendations are relevant but lack depth.|Recommendations are vague or incomplete.|Fails to provide relevant recommendations.|/10|||
|**Participation & Effort**|Actively engaged in the activity, followed instructions thoroughly.|Participated but required some guidance.|Minimal participation, needed significant help.|Did not participate meaningfully.|/10|||
|**Score**|**/50**|||||||

`	`Page 7** of 7**	
