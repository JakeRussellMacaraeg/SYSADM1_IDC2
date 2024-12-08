![image](https://github.com/user-attachments/assets/c11d814a-64b0-4171-840a-b03539ac755f)

# SYSADM1 – Setting Up Webserver
p@ssword123 – p@ssword – changeme	
# Requirement: 
- A virtual machine running Linux and Windows OS

  Task Instructions:

1. Install IIS by adding it as a role, select necessary features, include monitoring tools

   **SS:**
![image](https://github.com/user-attachments/assets/68ba20a7-ba53-4192-b82e-743cea51e864)

1. Create a website by opening IIS Manager 
   1. Right-click on the server’s name and select Internet Information Services Manager.
   1. Right-click on Sites and select Add Website.
   1. Enter a name, description, physical path (where your website files will reside), IP address, port, and host name.

**SS:**
![image](https://github.com/user-attachments/assets/c8773258-6264-4b1c-8649-db547997b3a9)


1. Configure the Website:
   1. Right-click on your website and select Edit.
   1. Set the Default Document to the name of your main HTML file >default.html
   1. Configure other settings as needed (e.g., SSL certificates, authentication)

**SS:**

![image](https://github.com/user-attachments/assets/a0bbaa6c-9004-4a54-87fc-aa66f4d9dc4a)

![image](https://github.com/user-attachments/assets/e5ea1328-628f-46f3-a532-86d6391eeb4b)


1. Create a Web Page:
   1. Create an HTML file in the physical path you specified.
   2. 
![image](https://github.com/user-attachments/assets/2e7939e6-ab73-495a-b703-0e578f9ba77a)


1. Save it as default.html or your preferred name.
1. Test the Web Server:
   1. Open a web browser and enter the URL of your website (e.g., http://localhost).
   1. You should see your web page displayed.

**SS:**
![image](https://github.com/user-attachments/assets/9e5c0b0f-b16c-4df5-aeef-4d68836b4e60)

Grading Rubric

|**Criteria**|**Points**|**Description**|
| :- | :- | :- |
|Web Server Installation|15|Correctly installs IIS or another web server on the virtual machine.|
|Website Configuration|15|Successfully configures the website with the correct physical path, IP address, port, and default document.|
|Successful Access|15|Successfully accesses the web page from the client computer using the correct URL.|
|Troubleshooting|15|Demonstrates ability to troubleshoot common issues, such as network connectivity problems or configuration errors.|
|Documentation|10|Provides clear and concise documentation of the installation, configuration, and testing process.|
|Total|/70||

`	`Page 4** of 4**	
