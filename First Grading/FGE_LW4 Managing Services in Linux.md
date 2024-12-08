![image](https://github.com/user-attachments/assets/7ee9b588-5064-49f8-8cc5-62d7e2573458)

# SYSADM1 – Managing Services in Linux
# Requirement: 
- A virtual machine running Linux
  
![image](https://github.com/user-attachments/assets/63b66c72-8dd2-4d01-861a-59cc7807feaf)

Complete this lab as follows: 

- Use the service –status-all command to list all active and inactive services.

  List down active and inactive services in the table below. Provide five (5) services for each column.

|**Active**|**Inactive**|
| :-: | :-: |
|alsa-utils|bluetooth|
|anacron|console-setup.sh|
|apparmor|grub-common|
|apport|hwclock.sh|
|cron|Keyboard-setup.sh|

SS: ![image](https://github.com/user-attachments/assets/667490f4-478a-48b2-b400-587c510eb85b)

- Start the Bluetooth service using the systemctl command. 

  Ex. sudo systemctl start httpd

  ![image](https://github.com/user-attachments/assets/c28d494c-847c-4565-8a6a-f12e4f6a0680)


- Check the status of the Bluetooth service. What is its status? **Enabled** 

  SS: ![image](https://github.com/user-attachments/assets/afb2938c-448a-4203-9a48-84fd2db19f56)

- Check the status of the cups services. Since when was it running? **Thu 2024-09-12 09:55:31 (5min ago)**

  SS: ![image](https://github.com/user-attachments/assets/371bd96b-bcad-4be3-80f8-00f987c78916)

- Stop cups services.

 ![image](https://github.com/user-attachments/assets/892e90f4-ec0f-41d9-a382-ae6b73ea7cc6)


- Verify if the service was stopped. 

 ![image](https://github.com/user-attachments/assets/9b996a21-f429-4246-836a-f467a2c5bb03)

- Restart the cups services.

![image](https://github.com/user-attachments/assets/a416c58c-a5b8-4a81-8700-1bb78c88c284)

- Verify if the service was restarted. 

  ![image](https://github.com/user-attachments/assets/eadc1011-a389-447b-b917-de466334c231)

`	`Page 4** of 4**	
