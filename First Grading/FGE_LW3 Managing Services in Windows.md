**﻿![image](https://github.com/user-attachments/assets/a565b8f4-5029-46c8-b07a-4aa246ebe232)**

# SYSADM1 – Managing Services in Windows
# Requirement: 
- A virtual machine running Linux and Windows OS

**Services** are background processes that run independently of user interactions in Windows. They provide essential system functions, such as network connectivity, printing, and time synchronization. This lab will guide you through the process of managing services using the Services app.
# Instructions: 
1. Open the Start menu and search for "Services"

  ![image](https://github.com/user-attachments/assets/73d950a4-e3f6-41bb-b4b0-914bf274fbaf)


1. Familiarize yourself with the columns, including Service Name, Display Name, Status, and Startup type.

   ![image](https://github.com/user-attachments/assets/94f71147-bd47-49f1-8764-1d95b321f993)


1. Right-click on a service and select "Start", "Stop", or "Restart". Fill out the table below

![image](https://github.com/user-attachments/assets/85eeb435-9a79-4f40-8684-1a4b073c8102)

   1. Select five network services, right-click to view its properties. Modify the startup setting to Manual.

   ![image](https://github.com/user-attachments/assets/0f676ad1-4016-4410-92a3-41f2cc2f3d86)

   **SS**:

1. Explore the "General", "Recovery", and "Log On" tabs to understand additional service settings.

1. Create a batch file that will be added as a new service later on. Refer to the batch file code below.

  ![image](https://github.com/user-attachments/assets/5eecdc62-3e69-4875-b30c-f755ba8b5236)

1. Save the batch file in Z:\lastname\_timer.bat

   ![image](https://github.com/user-attachments/assets/ae8c6f66-8a08-4a32-b8d3-bf3499b3b4d0)


1. Use the sc command to add timer.bat service in the command line interface.

   *sc create BatchTimerService binPath= "path\_to\_your\_batch\_file.bat" start= auto*

   *net start BatchTimerService*

   **Replace path\_to\_your\_batch\_file.bat with the actual path to your batch file.**

   ![image](https://github.com/user-attachments/assets/27c74371-3722-4d66-b6fa-2ad597d6d3ca)


1. Verify that BatchTimerService has been added to the services.

   **SS:** 

   ![image](https://github.com/user-attachments/assets/2733b4dd-c0dd-4e2f-961a-f516198abcd6)


1. **Testing the Service:** Now, if you open a new command prompt, you should see the timer countdown without requiring your interaction. Once the timer finishes, you'll see the "Timer finished!" message.

   **SS:**

   ![image](https://github.com/user-attachments/assets/bd05ad46-0c38-4220-94ad-ef7e7ac68719)



**Rubric**

|**Criteria**|**Excellent (10)**|**Good (7)**|**Needs Improvement (3)**|**Unsatisfactory (1)**|
| :-: | :-: | :-: | :-: | :-: |
|Understanding of Services|Demonstrates a deep understanding of the concept of services, their roles, and their importance in Windows.|Shows a solid understanding of services, but may lack some depth in specific areas.|Has a basic understanding of services, but may struggle with specific concepts.|Shows little or no understanding of services.|
|Service Management Skills|Successfully starts, stops, restarts, and configures services using the Services app.|Demonstrates proficiency in managing services, but may encounter minor difficulties.|Can perform basic service management tasks, but may need assistance or guidance.|Struggles to perform even basic service management tasks.|
|Custom Service Creation|Successfully creates and manages a custom service using the appropriate tools and techniques.|Can create a custom service, but may encounter minor difficulties or require assistance.|Has limited experience with creating custom services.|Cannot create a custom service.|
|Problem-Solving|Demonstrates strong problem-solving skills when encountering challenges or errors.|Can effectively troubleshoot and resolve most issues related to service management.|May require assistance to troubleshoot some issues.|Struggles to troubleshoot and resolve issues.|
|Documentation and Reporting|Provides clear and concise documentation of the lab activities, including relevant screenshots and observations.|Documents the lab activities adequately, but may lack some detail or clarity.|Provides basic documentation, but may be disorganized or incomplete.|Does not provide any documentation or reporting.|
|**Score:**|`     `**/50**||||


`	`Page 6** of 6**	
