<table>
<colgroup>
<col style="width: 48%" />
<col style="width: 35%" />
<col style="width: 15%" />
</colgroup>
<tbody>
<tr class="odd">
<td colspan="3"><p><img src="media/image1.png"
style="width:2.4in;height:0.58819in" /></p>
<p>SCHOOL OF INFORMATION AND TECHNOLOGY</p></td>
</tr>
<tr class="even">
<td>NAME: <strong>MACARAEG, JAKE RUSSELL</strong></td>
<td>DATE PERFORMED: <strong>26/09/24</strong></td>
<td rowspan="2">/50 </td>
</tr>
<tr class="odd">
<td>Section: <strong>IDC2</strong></td>
<td>DATE SUBMITTED: <strong>03/10/24</strong></td>
</tr>
</tbody>
</table>

# SYSADM1 -- Monitoring Print Services in Windows Server 2019 {#sysadm1-monitoring-print-services-in-windows-server-2019}

# Requirement:  {#requirement}

- A virtual machine running Linux and Windows OS

Part 1: Setting Up Print Services

1.  Install and configure **print.srv** domain

> ![](media/image2.png){width="2.802474846894138in"
> height="0.4375612423447069in"}

2.  Connect one client to the recently created domain

> ![](media/image3.png){width="3.0782294400699914in"
> height="0.8255249343832021in"}

3.  Install Print Services Role:

> ![](media/image4.png){width="3.604669728783902in"
> height="1.6252263779527558in"}

4.  Search the internet for any printer installer and convert it to iso

> ![](media/image5.png){width="4.604809711286089in"
> height="0.8542858705161854in"}

5.  Install and deploy it as network printer

> ![](media/image6.png){width="5.823729221347332in"
> height="1.1459930008748906in"}
> ![](media/image7.png){width="5.723194444444444in"
> height="2.5982042869641293in"}

Part 2: Monitoring Print Services

Objective: Familiarize yourself with monitoring tools available in
Windows Server 2019.

1.  Event Viewer:

    - Open Event Viewer (run eventvwr.msc).

**SS:**

![](media/image8.png){width="4.911820866141732in"
height="3.4633694225721783in"}

- Navigate to Applications and Services Logs \> Microsoft \> Windows \>
  PrintService.

**SS:**

![](media/image9.png){width="4.846229221347332in"
height="3.3936537620297464in"}

- Review logs for print jobs, errors, and warnings.

**SS:**

![](media/image10.png){width="4.910982064741908in"
height="1.1484481627296588in"}

![](media/image11.png){width="4.813171478565179in"
height="1.4793733595800524in"}

2.  Performance Monitor:

    - Open Performance Monitor (run perfmon).

**SS:**

![](media/image12.png){width="4.902594050743657in"
height="3.5145188101487315in"}

- In the left pane, expand Data Collector Sets \> System.

**SS:**

![](media/image13.png){width="4.9073031496062995in"
height="2.6097145669291337in"}

- Right-click System Performance and select Start.

**SS:**

![](media/image14.png){width="3.691858048993876in"
height="2.763659230096238in"}

- Monitor performance metrics related to print services.

**SS:**

![](media/image15.png){width="6.373884514435695in"
height="1.3350317147856519in"}

3.  Using Print Management Console:

    - Open Print Management from Server Manager.

**SS:**

![](media/image16.png){width="6.012549212598425in"
height="1.9857633420822398in"}

- View active print jobs and their status

- Use the Printers node to check the status of all printers.

![](media/image17.png){width="3.175667104111986in"
height="3.50538167104112in"}
![](media/image18.png){width="3.353885608048994in"
height="3.5351760717410325in"}

![](media/image19.png){width="3.253494094488189in"
height="3.405909886264217in"}

Part 3: Exploring Third-Party Monitoring Tools

1.  Research at least two third-party print monitoring tools

    - Consider factors such as features, pricing, and compatibility with
      Windows Server 2019.

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>PaperCut MF</strong></p>
<ul>
<li><p><strong>Features:</strong> Tracks print jobs by user, department,
or cost center, enforces print policies, and offers detailed reporting.
It supports print quotas, secure print release, and integrates with
multi-function devices.</p></li>
<li><p><strong>Pricing:</strong> Pricing varies depending on the
organization’s size and needs, but a trial version is available for
testing.</p></li>
<li><p><strong>Compatibility:</strong> Fully compatible with Windows
Server 2019 and supports various printer models.</p></li>
</ul>
<p><strong>Print Inspector</strong></p>
<ul>
<li><p><strong>Features</strong>: Provides real-time monitoring of print
jobs, logs detailed information on printing activities (user, document
name, page count), and offers automated alerts for issues. It also
allows for print job management, including pausing and
resuming.</p></li>
<li><p><strong>Pricing</strong>: Offers a one-time license fee, and a
free trial is available for testing.</p></li>
<li><p><strong>Compatibility</strong>: Works seamlessly with Windows
Server 2019, supporting both local and network printers.</p></li>
</ul></th>
</tr>
</thead>
<tbody>
</tbody>
</table>

2.  Install and Configure:

    - Choose one of the tools to install in your environment.

**SS:**

![](media/image20.png){width="4.39125in" height="3.763929352580927in"}

- Follow the installation instructions provided by the tool\'s
  documentation.

- Configure it to monitor your print services.

3.  Test and Report Findings:

    - Generate a report or dashboard from the tool.

    - Analyze the collected data (e.g., print volume, errors, user
      activity).

> ![](media/image21.png){width="5.06038167104112in"
> height="2.0538582677165356in"}![](media/image22.png){width="5.050833333333333in"
> height="1.9301881014873141in"}
>
> ![](media/image23.png){width="5.0967213473315836in"
> height="1.9285837707786526in"}
>
> ![](media/image24.png){width="5.117693569553806in"
> height="1.9916469816272966in"}
>
> ![](media/image25.png){width="5.187251749781277in"
> height="2.010003280839895in"}

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
