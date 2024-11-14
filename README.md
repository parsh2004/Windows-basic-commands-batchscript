# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file
Save each script in a file with a .bat extension.
Ensure you have the necessary permissions to perform the operations.
Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.
## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/2f772c7c-df81-4f10-876f-3ec3ea90d855)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT
~~~
cd %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/30afb10e-ed11-43c2-afd7-6e449702b809)
~~~
type nul > MyFile.txt
~~~
![image](https://github.com/user-attachments/assets/49543cb7-dc1b-4659-827e-372bcd0c7a60)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
~~~
dir %userprofile%\Desktop\MyLab
~~~
![image](https://github.com/user-attachments/assets/b52427ad-faca-485a-aac0-009cb5a9f192)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/2391f770-41a9-4e80-84b8-cfe0eeb870fd)
~~~
copy MyFile.txt %userprofile%\Desktop\Backup
~~~
![image](https://github.com/user-attachments/assets/2bf51fa4-adaf-4ffb-ae47-f6517be2ae0b)

Move the "MyLab" directory to the "Documents" folder.

## COMMAND AND OUTPUT
~~~
mkdir %userprofile%\Desktop\Documents
move MyLab Documents
~~~
![image](https://github.com/user-attachments/assets/b5954d6e-fbe9-4ace-aa9e-af958b976b16)




## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
~~~
![image](https://github.com/user-attachments/assets/faa61b99-b6b9-4ea1-972d-f0beb7a27d68)
## COMMAND:
~~~
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
~~~
## OUTPUT
![image](https://github.com/user-attachments/assets/79879eec-4e0f-4b12-bf35-d4bd0ca3f933)

## RESULT:
The commands/batch files are executed successfully.






# RESULT:
The commands/batch files are executed successfully.

