![image](https://github.com/user-attachments/assets/caf5724c-1f84-4573-9156-cd13aab2fd3a)

# SYSADM1 – Introduction to File Systems in Windows and Linux
# Requirement: 
- A virtual machine running Linux and Windows OS
# Instructions: 
**Part A: Windows File System**

1. **Open File Explorer:** Click the File Explorer icon on your desktop or press the Windows key + E.
1. **Navigate to your Documents folder:** This is usually the default location for user files.
1. **Create a new folder:** Right-click in an empty space, select "New," then "Folder." Name it "Lab1\_Windows."

  ![image](https://github.com/user-attachments/assets/9518b27c-3b51-4835-a0be-b8a1336cac5e)


1. **Create a text file:** Right-click in the "Lab1\_Windows" folder, select "New," then "Text Document." Rename it to "info.txt."

  ![image](https://github.com/user-attachments/assets/beb48221-9d29-43fd-bcc3-b8439bd6780c)


1. **Open the text file:** Double-click the "info.txt" file to open it in Notepad.
1. **Type some text:** Write a short paragraph about yourself or the purpose of the file.

  ![image](https://github.com/user-attachments/assets/164ba566-0526-4f88-b9f5-156faf543c50)


1. **Save the file:** Close the Notepad window and save the changes.
1. **Create a subfolder:** Create a new folder inside "Lab1\_Windows" called "Data."

  ![image](https://github.com/user-attachments/assets/ea84efdb-0881-4d47-9677-e9a80538ab54)


1. **Copy the text file:** Copy the "info.txt" file to the "Data" subfolder.

  ![image](https://github.com/user-attachments/assets/7c03491a-357e-492a-a4dc-e82d07f179b3)


1. **Rename the copied file:** Rename the copied file to "data.txt.

  ![image](https://github.com/user-attachments/assets/461a17d1-3dff-47c5-98fd-9e782954cde8)


1. Create a folder named "LabFiles" with subfolders for each file type. Use the internet for the resources of the files listed below. 

   **LabFiles** 

   1. **Text** 
      1. large\_text.txt
      1. small\_text.txt
      1. code.cpp
   1. **Images** 
      1. image1.jpg
      1. image2.png
      1. image3.bmp
   1. **Audio** 
      1. song.mp3
      1. speech.wav
   1. **Video** 
      1. clip.mp4



![image](https://github.com/user-attachments/assets/beccb9d9-3a2a-42ee-bd9a-86f895609f00)
![image](https://github.com/user-attachments/assets/07c488e5-d188-4686-80b3-8ddccbe93fb9)



1. **Check file properties:** Right-click on the "info.txt" file and select "Properties." Explore the General, Details, and Security tabs to understand file attributes like creation date, size, and read-only status.

  ![image](https://github.com/user-attachments/assets/0e25451e-d5ab-4665-8a60-1edb5536bf40)
  ![image](https://github.com/user-attachments/assets/93ec867a-1e81-4645-9983-d53c216040e2)
  ![image](https://github.com/user-attachments/assets/550e5884-499d-4a4a-a866-01edb30b8cf0)


1. **Change file attributes:** Try changing the file attributes (e.g., read-only, hidden) using the Properties dialog. Observe the changes in File Explorer.

   ![image](https://github.com/user-attachments/assets/bba51729-772a-4094-b5d8-6a9c36679271)


1. **Share the folder:** Right-click on the "Lab1\_Windows" folder, select "Properties," and then the "Sharing" tab. Share the folder with a specific user or group, setting appropriate permissions (e.g., Read, Write, Full control)

   ![image](https://github.com/user-attachments/assets/1902c5ce-0164-4ec8-a8ba-10046821e967)


1. **Create an archive:** Use WinRAR or 7-Zip to create a compressed archive of the "Lab1\_Windows" folder.

  ![image](https://github.com/user-attachments/assets/2208a27e-fc4e-46c1-b41e-5a8286e9a47a)

1. ` `**Extract an archive:** Create a new folder, then extract the created archive into it.

   ![image](https://github.com/user-attachments/assets/7ad5dce8-aa5a-4c5f-8e71-aa94d7d53f01)


Part B. Create a log report structure

|<p></p><p>***LOG REPORT FOR ( FGE\_LW1 )***</p><p></p>||||||
| :-: | :- | :- | :- | :- | :- |
|**Name**|**Location**|**Date Modified**|**Type**|**Size**|**Status / Attributes**|
|**Lab1\_Windows**|Z:\FGE\_LW|<p>22/08/2024 </p><p>9:26 am</p>|File Folder|50\.5MB|Added “Full Control” for Arvin Padilla|
|**Data**|<p>Z:\FGE\_LW\Lab1\_Windows</p><p></p>|<p>22/08/2024</p><p>9:26 am</p>|File Folder|50\.5MB|Default|
|**info**|<p>Z:\FGE\_LW\Lab1\_Windows</p><p></p>|<p>22/08/24</p><p>8:34 am</p>|Text Document ( .txt )|426 byte|<p>Read-only</p><p>Hidden</p>|
|**LAB FILES**||||||
|**LabFiles**|Z:\FGE\_LW\Lab1\_Windows\Data|<p>22/08/24</p><p>8:34 am</p>|File Folder|50\.4 MB|Default|
|**data**|Z:\FGE\_LW\Lab1\_Windows\Data|<p>22/08/24</p><p>9:26 am</p>|Text Document ( .txt )|426 byte|Default|
|**Audio**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles|<p>22/08/24</p><p>9:26 am</p>|File Folder|40\.3 MB|Default|
|**Song**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Audio|<p>22/08/24</p><p>8:54 am</p>|MP3 File (.mp3)|168 KB|Default|
|**speech**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Audio|<p>22/08/24</p><p>8:58 am</p>|WAV File (.wav)|40\.1 MB|Default|
|**Images**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles|<p>22/08/24</p><p>9:26 am</p>|File Folder|8\.15 MB|Default|
|**Image1**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Images|<p>22/08/24</p><p>8:41 am</p>|JPG File (.jpg)|103 KB|Default|
|**Image2**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Images|<p>22/08/24</p><p>8:43 am</p>|PNG File (.png)|1\.01 MB|Default|
|**Image3**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Images|<p>22/08/24</p><p>8:44 am</p>|BMP File (.bmp)|7\.03 MB|Default|
|**Text**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles|<p>22/08/24</p><p>9:26 am </p>|File Folder|246 bytes|Default|
|**code**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Text|<p>22/08/24</p><p>9:00 am</p>|C++ Source File (.cpp)|94 bytes|Default|
|**Large\_text**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Text|<p>22/08/24</p><p>9:05 am</p>|Text Document (.txt)|76 bytes|Default|
|**Small\_text**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Text|<p>22/08/24</p><p>9:05 am</p>|Text Document (.txt)|76 bytes|Default|
|**Video**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles|<p>22/08/24</p><p>9:26 am</p>|File Folder|2\.01 MB|Default|
|**Clip**|Z:\FGE\_LW\Lab1\_Windows\Data\LabFiles\Video|<p>22/08/24</p><p>8:53 am</p>|MP4 File (.mp4)|2\.01 MB|Default|



|**Extracted (Zipped)**|||||||
| :-: | :- | :- | :- | :- | :- | :- |
|**Extracted File**|Z:\FGE\_LW|<p>22/08/2024 </p><p>9:28 am</p>|File Folder|94\.0MB|Default||
|**Lab1\_Windows\_ExtractedFile**|Z:\FGE\_LW\Extracted File|<p>22/08/2024</p><p>9:34 am</p>|File Folder|50\.4 MB|Default||
|**Lab1\_Windows**|Z:\FGE\_LW\Extracted File|<p>22/08/2024</p><p>9:25 am</p>|Compressed (zipped) Folder|43\.5 MB|Can’t Open (due to W11 bug||
|**Extracted (Zipped) LabFile**|||||||
|**LabFiles**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data|<p>22/08/24</p><p>8:34 am</p>|File Folder|50\.4 MB|Default||
|**data**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile|<p>22/08/24</p><p>9:26 am</p>|Text Document ( .txt )|426 byte|Default||
|**info**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile|<p>22/08/24</p><p>8:34 am</p>|Text Document ( .txt )|426 byte|<p>Read-only</p><p>Hidden</p>||
|**Audio**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles|<p>22/08/24</p><p>9:26 am</p>|File Folder|40\.3 MB|Default||
|**Song**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Audio|<p>22/08/24</p><p>8:54 am</p>|MP3 File (.mp3)|168 KB|Default||
|**speech**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Audio|<p>22/08/24</p><p>8:58 am</p>|WAV File (.wav)|40\.1 MB|Default||
|**Images**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles|<p>22/08/24</p><p>9:26 am</p>|File Folder|8\.15 MB|Default||
|**Image1**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Images|<p>22/08/24</p><p>8:41 am</p>|JPG File (.jpg)|103 KB|Default||
|**Image2**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Images|<p>22/08/24</p><p>8:43 am</p>|PNG File (.png)|1\.01 MB|Default||
|**Image3**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Images|<p>22/08/24</p><p>8:44 am</p>|BMP File (.bmp)|7\.03 MB|Default||
|**Text**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles|<p>22/08/24</p><p>9:26 am </p>|File Folder|246 bytes|Default||
|**code**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Text|<p>22/08/24</p><p>9:00 am</p>|C++ Source File (.cpp)|94 bytes|Default||
|**Large\_text**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Text|<p>22/08/24</p><p>9:05 am</p>|Text Document (.txt)|76 bytes|Default||
|**Small\_text**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Text|<p>22/08/24</p><p>9:05 am</p>|Text Document (.txt)|76 bytes|Default||
|**Video**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles|<p>22/08/24</p><p>9:26 am</p>|File Folder|2\.01 MB|Default||
|**Clip**|Z:\FGE\_LW\Extracted File\Lab1\_Windows\_ExtractedFile\Data\LabFiles\Video|<p>22/08/24</p><p>8:53 am</p>|MP4 File (.mp4)|2\.01 MB|Default||

`	`Page 13** of 13**	
