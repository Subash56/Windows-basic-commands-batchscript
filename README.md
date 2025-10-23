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
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/be3a2a60-e96d-45cf-9418-23fe6b5d95f6)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/09ecfaee-f963-4b02-854e-b6a175471a10)

type nul > MyFile.txt

![image](https://github.com/user-attachments/assets/40eb4147-181c-452e-a721-ff86df22fe57)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/ff6d92a2-3a11-45df-9ff3-22035b636ebb)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/31a95ef7-0377-4e71-8371-479c8496df76)

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/71aeda84-71f4-4f3c-9854-32e4d691e579)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Documents
move MyLab Documents

![image](https://github.com/user-attachments/assets/d184b230-ca78-42d0-b702-52e521c85d9e)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
## COMMAND
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```
## OUTPUT

![image](https://github.com/user-attachments/assets/4cf3c508-ffe3-4b54-96a8-c9169988c893)

## COMMAND
```
  @echo off
  mkdir %userprofile%\Desktop\DocBackup
  copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
  del %userprofile%\Documents\*.docx
  echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/user-attachments/assets/3463040f-f83a-4484-a803-28558f5639de)

# RESULT:
The commands/batch files are executed successfully.

