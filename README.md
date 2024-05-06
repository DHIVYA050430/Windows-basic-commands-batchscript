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

mkdir %userprofile%\Desktop\Mylab

![COM 1](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/f3f94b18-b3ae-4a9b-8d9d-cf0728129c2c)
Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

cd %userprofile%\Desktop\MyLab
![COM 2 1](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/eb63632e-399d-414f-8cd5-58bfa2cbe9c5)
![COM 2 2](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/97315119-fc06-4940-89d3-aeaeed1184a3)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
dir %userprofile%\Desktop\MyLab
![COM 3](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/43b2c284-d36f-4f60-9289-ed9f1e0d0331)



## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
mkdir %userprofile%\Desktop\Backup
copy MyFile.txt %userprofile%\Desktop\Backup
![COM 3 2](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/cd0c480b-a552-44b4-9ede-ea6740f9f5f9)

![COM 4](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/7f240e98-4c72-4b2b-ae87-27b01db5794d)

## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![7](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/ff76c4f1-bdcd-4a43-a5d0-d3fd3451b9d7)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the
"Documents" folder to a new folder named "DocBackup" on the desktop.
```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
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
![OUTPUT COM](https://github.com/DHIVYA050430/Windows-basic-commands-batchscript/assets/147141546/e2960f41-c52c-45ec-9701-586a6ca42eae)



# RESULT:
The commands/batch files are executed successfully.

