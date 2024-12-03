![image](https://github.com/user-attachments/assets/4b417f1b-1b4c-4825-8724-a4e9b92bde27)


# SYSADM1 -- Monitoring Print Services in Windows Server 2019 {#sysadm1-monitoring-print-services-in-windows-server-2019}

# Requirement:  {#requirement}

- A virtual machine running Linux and Windows OS

Part 1: Setting Up Print Services

1.  Install and configure **print.srv** domain

![image](https://github.com/user-attachments/assets/9ce69055-d325-4b78-bd7b-61ca5260767f)


2.  Connect one client to the recently created domain

![image](https://github.com/user-attachments/assets/205ad594-e99e-446a-b3ef-78067638ada3)

3.  Install Print Services Role:

![image](https://github.com/user-attachments/assets/46f2fe6a-447e-4114-bd13-ef78e20247d8)


4.  Search the internet for any printer installer and convert it to iso

![image](https://github.com/user-attachments/assets/1d3e1a43-fde2-405a-acf7-d84917bd17ed)


5.  Install and deploy it as network printer

S![image](https://github.com/user-attachments/assets/27241980-744f-4d3c-b8cd-f28f1cf3e8aa)


Part 2: Monitoring Print Services

Objective: Familiarize yourself with monitoring tools available in
Windows Server 2019.

1.  Event Viewer:

    - Open Event Viewer (run eventvwr.msc).

**SS:**

![image](https://github.com/user-attachments/assets/891c2d02-7654-4eef-84ca-37622fd368bb)


- Navigate to Applications and Services Logs \> Microsoft \> Windows \>
  PrintService.

**SS:**

![image](https://github.com/user-attachments/assets/efd8716c-6f6e-4d27-8814-2c89105e705c)


- Review logs for print jobs, errors, and warnings.

**SS:**

![image](https://github.com/user-attachments/assets/d3a625f2-2be2-4a9a-bc02-bc64056f8b81)


2.  Performance Monitor:

    - Open Performance Monitor (run perfmon).

**SS:**

![image](https://github.com/user-attachments/assets/57ed8883-f483-48da-b403-890823cbfad1)


- In the left pane, expand Data Collector Sets \> System.

**SS:**

![image](https://github.com/user-attachments/assets/9e304b1e-c4c3-45bf-9f9e-13c1abc75ed4)


- Right-click System Performance and select Start.

**SS:**

![image](https://github.com/user-attachments/assets/8b168a60-6a6a-48b3-80cf-6824f96ca67a)


- Monitor performance metrics related to print services.

**SS:**

![image](https://github.com/user-attachments/assets/cdcf7529-15bf-4533-8bd3-3c861c7b5093)


3.  Using Print Management Console:

    - Open Print Management from Server Manager.

**SS:**

![image](https://github.com/user-attachments/assets/c9951b8b-c997-477d-9785-ff925e61a112)


- View active print jobs and their status

- Use the Printers node to check the status of all printers.

![image](https://github.com/user-attachments/assets/5d31436f-3be2-4eaa-acc5-25472714a2a3)

![image](https://github.com/user-attachments/assets/17cc9377-26c1-4bdb-9e6b-d0716d0fcbcb)


Part 3: Exploring Third-Party Monitoring Tools

1.  Research at least two third-party print monitoring tools

    - Consider factors such as features, pricing, and compatibility with
      Windows Server 2019.
      
![image](https://github.com/user-attachments/assets/c877a462-9f0d-48b9-a7ff-4d7298327dba)


2.  Install and Configure:

    - Choose one of the tools to install in your environment.

**SS:**

![image](https://github.com/user-attachments/assets/044d3314-be94-44a2-b847-aa54ee51f802)


- Follow the installation instructions provided by the tool\'s
  documentation.

- Configure it to monitor your print services.

3.  Test and Report Findings:

    - Generate a report or dashboard from the tool.

    - Analyze the collected data (e.g., print volume, errors, user
      activity).

![image](https://github.com/user-attachments/assets/0b2f20b8-1f45-4d09-aff7-77eac7a784e8)
![image](https://github.com/user-attachments/assets/eb9313ed-bd4e-41eb-bebf-72a52e3371d2)
![image](https://github.com/user-attachments/assets/e205524b-45b6-40b4-a9db-641e79fe7a42)



Rubric

| **Criteria** | **1 (Unsatisfactory)** | **2 (Needs Improvement)** | **3 (Satisfactory)** | **4 (Good)** | **5 (Excellent)** | **Score** |
|--------------|------------------------|---------------------------|----------------------|--------------|-------------------|-----------|

| **Part 1: Setting Up Print Services** |     |     |     |     |     |     |
|---------------------------------------|-----|-----|-----|-----|-----|-----|

| **Domain Installation** | No domain created | Domain created with errors | Domain created correctly | Domain configured well | Domain configured and documented thoroughly |     |
|-------------------------|-------------------|----------------------------|--------------------------|------------------------|---------------------------------------------|-----|

| **Client Connection** | Client not connected | Connection attempt failed | Client connected but with issues | Client connected correctly | Client connected and documented well |     |
|-----------------------|----------------------|---------------------------|----------------------------------|----------------------------|--------------------------------------|-----|

| **Print Services Role Installation** | Role not installed | Role installed with issues | Role installed correctly | Role installed and configured | Role installed, configured, and documented thoroughly |     |
|--------------------------------------|--------------------|----------------------------|--------------------------|-------------------------------|-------------------------------------------------------|-----|

| **Printer Installer Conversion** | No installer found | Installer conversion attempted but failed | Installer converted but not used | Installer converted and used | Installer converted, used, and documented well |     |
|----------------------------------|--------------------|-------------------------------------------|----------------------------------|------------------------------|------------------------------------------------|-----|

| **Network Printer Deployment** | Printer not deployed | Deployment failed | Printer deployed but not functional | Printer deployed correctly | Printer deployed, tested, and documented well |     |
|--------------------------------|----------------------|-------------------|-------------------------------------|----------------------------|-----------------------------------------------|-----|

| **Part 2: Monitoring Print Services** |     |     |     |     |     |     |
|---------------------------------------|-----|-----|-----|-----|-----|-----|

| **Event Viewer Usage** | Event Viewer not opened | Opened but no logs reviewed | Logs reviewed but superficial | Logs reviewed with some analysis | Logs reviewed with thorough analysis and documentation |     |
|------------------------|-------------------------|-----------------------------|-------------------------------|----------------------------------|--------------------------------------------------------|-----|

| **Performance Monitor Usage** | Performance Monitor not opened | Opened but no metrics monitored | Metrics monitored but not analyzed | Metrics monitored with some analysis | Metrics monitored, analyzed, and documented thoroughly |     |
|-------------------------------|--------------------------------|---------------------------------|------------------------------------|--------------------------------------|--------------------------------------------------------|-----|

| **Print Management Console Usage** | Console not opened | Opened but functionality not used | Active jobs viewed superficially | Active jobs viewed with some detail | Active jobs viewed and documented thoroughly |     |
|------------------------------------|--------------------|-----------------------------------|----------------------------------|-------------------------------------|----------------------------------------------|-----|

| **Part 3: Exploring Third-Party Tools** |     |     |     |     |     |     |
|-----------------------------------------|-----|-----|-----|-----|-----|-----|

| **Research on Tools** | No tools researched | Research incomplete | Research on one tool completed | Research on two tools with some analysis | Research on two tools, detailed analysis, and comparison |     |
|-----------------------|---------------------|---------------------|--------------------------------|------------------------------------------|----------------------------------------------------------|-----|

| **Installation and Configuration** | Tool not installed | Installation failed | Tool installed but not configured | Tool installed and configured with issues | Tool installed, configured, and documented thoroughly |     |
|------------------------------------|--------------------|---------------------|-----------------------------------|-------------------------------------------|-------------------------------------------------------|-----|

| **Reporting Findings** | No report generated | Report lacks detail | Report generated but lacks analysis | Report generated with some analysis | Comprehensive report with thorough analysis and documentation |     |
|------------------------|---------------------|---------------------|-------------------------------------|-------------------------------------|---------------------------------------------------------------|-----|
