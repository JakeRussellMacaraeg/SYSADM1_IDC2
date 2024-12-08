![image](https://github.com/user-attachments/assets/7e4587e5-3aa2-46e2-b1fe-a0867bfafbe9)

# SYSADM1 – Kerberos Lab Activity: A step-by-step Guide

**Objective:**

Set up a basic Kerberos authentication system to understand how Kerberos manages secure logins through ticket-based access.

**Setup Requirements:**

- Two VMs in Oracle VM, both running a Linux distribution like Ubuntu or CentOS.
- VM1: Kerberos Server
- VM2: Kerberos Client

**Step 1: Initial Setup and Package Installation**

1. **Update Packages on Both VMs:**
   1. Open a terminal on each VM and run:

*bash*

*sudo apt update && sudo apt upgrade –y*
*LinuxCLNT:*
![image](https://github.com/user-attachments/assets/fc9bc4c7-e66b-4ec2-8cd3-f116b32a2608)


*LinuxSRVR:*
![image](https://github.com/user-attachments/assets/2e53e3a4-03a2-478b-b0f6-83f8a2f3b95e)

1. **Install Kerberos Server Packages on VM1 (Kerberos Server):**
   1. In VM1, install the Kerberos Key Distribution Center (KDC) and admin server:

*bash*

*sudo apt install krb5-kdc krb5-admin-server –y*
![image](https://github.com/user-attachments/assets/68ab91ef-186e-4093-abe9-add1db697f45)



1. **Install Kerberos Client Package on VM2 (Kerberos Client):**
   1. In VM2, install the Kerberos client software:

*bash*

*sudo apt install krb5-user -y*
![image](https://github.com/user-attachments/assets/d631f5dd-fbbb-49bb-b57c-f0914a814f07)


1. During installation, when prompted, enter the Kerberos realm you plan to set up, e.g., MYLAB.LOCAL.
![image](https://github.com/user-attachments/assets/4ba945cb-4197-497b-87be-f265fc36e2d5)


-----
**Step 2: Configure the Kerberos Server (VM1)**

1. **Edit the Kerberos Configuration File:**
   1. Open /etc/krb5.conf for editing:

*bash*

*sudo nano /etc/krb5.conf*
![image](https://github.com/user-attachments/assets/eadb30b8-493d-4716-9f89-9c216cb85bf2)


1. Set the realm as MYLAB.LOCAL. You should also specify the KDC and admin server as VM1’s hostname or IP address:

ini

[libdefaults]

`    `default\_realm = MYLAB.LOCAL

[realms]

`    `MYLAB.LOCAL = {

`        `kdc = <VM1\_IP\_or\_hostname>

`        `admin\_server = <VM1\_IP\_or\_hostname>

`    `}

![image](https://github.com/user-attachments/assets/07ff512f-17b6-4492-b7a3-845c7f1b9ce2)


1. Save and close the file (Ctrl+X, then Y, and Enter to confirm).
1. **Initialize the Kerberos Database:**
   1. Create the database for the Kerberos realm:

*bash*

*sudo krb5\_newrealm*
![image](https://github.com/user-attachments/assets/d5e61787-ef8f-435b-a97e-e0645e0a2547)

1. You will be prompted to set a password for the Kerberos database.

![image](https://github.com/user-attachments/assets/fe2b8952-0421-48d1-bc84-2b3bdb387609)

1. **Start and Enable the Kerberos Services:**
   1. Start the KDC and admin server, and ensure they start automatically on boot:

*bash*

*sudo systemctl start krb5-kdc*

*sudo systemctl start krb5-admin-server*

*sudo systemctl enable krb5-kdc*

*sudo systemctl enable krb5-admin-server*

![image](https://github.com/user-attachments/assets/9cc9c262-d7a5-4a1f-81fe-4847b7e97953)


-----
**Step 3: Set Up a Kerberos User Principal**

1. **Create a New User Principal:**
   1. Run the following command to create a test user in the Kerberos realm:

*bash*

*sudo kadmin.local -q "addprinc <testuser@MYLAB.LOCAL>"*

![image](https://github.com/user-attachments/assets/9ed97325-81c5-49aa-981c-b9e31c2ddb8f)


1. **Verify the User Principal:**
   1. To confirm the principal is created, list all principals:

*bash*

*sudo kadmin.local -q "listprincs"
![image](https://github.com/user-attachments/assets/63eb8def-8890-4f0f-a3a1-35e9c6921615)


-----
**Step 4: Configure the Kerberos Client (VM2)**

1. **Edit the Kerberos Configuration File on VM2:**
   1. Open /etc/krb5.conf for editing on VM2:

*bash*

*sudo nano /etc/krb5.conf*

1. Set the default realm to MYLAB.LOCAL and point to the KDC and admin server on VM1. The configuration should match what you set on VM1.

![image](https://github.com/user-attachments/assets/0bda0d34-ca4b-4aba-85e0-0af98f99004e)


-----
**Step 5: Test Kerberos Authentication**

1. **Request a Kerberos Ticket for the User on VM2:**
   1. In the terminal on VM2, request a ticket for testuser:

*bash*

*kinit testuser@MYLAB.LOCAL*

1. Enter the password you set for testuser.
1. **Verify the Ticket:**
   1. Check if the ticket was issued by listing active Kerberos tickets:

*bash*

*klist*

1. You should see details about the ticket, such as the principal and expiration time, confirming successful Kerberos authentication.

`	`Page 8** of 8**	
