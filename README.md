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
**DEVELOPED BY:VAISHNAVIDEVI V**


**REGISTRATION NUMBER:212223040230**
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT

mkdir %userprofile%\Desktop\MyLab

![8 1](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/1028b168-24a5-411a-8602-7d0faca70549)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT

cd %userprofile%\Desktop\MyLab


![8 2](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/d8e6a87d-6772-4bd5-866f-266231b702ba)

![8 3](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/522d6b6e-a429-438c-a5ca-d149d31d8b6c)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![8 4](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/a2993d25-c490-4996-8acc-f9f0233424cd)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT


mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup

![8 5](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/920468fb-3aff-4117-8821-be1f85dbbbcc)

![8 6](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/4fd1a319-b3a6-4c63-acb6-c44cac9025a2)


Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT

mv Myfile.txt %userprofile%\Documents

![8 7](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/95c85ef3-27a0-4499-be81-a7822296bf31)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```

Modify the script to delete files with the ".docx" extension from the "Documents" folder after creating the backup.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```






## OUTPUT

![8 8](https://github.com/vaishnavidevi23013992/Windows-basic-commands-batchscript/assets/151864235/34848cd2-eea8-4f9d-9957-6154abdd7bf6)




# RESULT:
The commands/batch files are executed successfully.

