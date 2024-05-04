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
#### mkdir %username%\Desktop\MyLab
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_e7a24b01.jpg>)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
#### cd %username%\Desktop\MyLab
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_078b664c.jpg>)
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_c02b2de0.jpg>)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
#### dir %username%\Desktop\MyLab
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_615d31c5.jpg>)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
#### cp %username%\Desktop\Backup1
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_6e97fa93.jpg>)
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_74c1e5c2.jpg>)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
#### mv Myfile.txt %userprofile%\Documents
![alt text](<WhatsApp Image 2024-05-01 at 17.44.16_3e9050a7.jpg>)

## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

````
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
````
Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.
````
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
````
## OUTPUT

![alt text](<WhatsApp Image 2024-05-01 at 17.43.35_61c3e0af.jpg>)



# RESULT:
The commands/batch files are executed successfully.

