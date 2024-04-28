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
![os 08 img 01](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/9e185419-03ae-4c89-aee2-b26c25767c15)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab
![os 08 img 02](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/c5b5bcd3-0114-4b56-9309-6f28c60ac8cc)
![os 08 img 03](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/c57ebf7d-6a02-49a9-893a-10c58a635636)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab
![os 08 img 04](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/705f8d20-4975-4f3a-ab6e-09c864ed63dd)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
![os 08 img 05](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/40c3ab6e-003c-4db7-b7c1-4278db126263)
![os 08 img 06](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/67658080-3d7a-4a67-a795-258825cdf314)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mv Myfile.txt %userprofile%\Documents
![os 08 img 07](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/f8ff6416-e83b-4ab3-949a-1249216e02de)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.
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


![os 08 img](https://github.com/pawan2006-png/Windows-basic-commands-batchscript/assets/150067867/28a040d2-a9fd-48f4-ad74-0e48f7bfed93)



# RESULT:
The commands/batch files are executed successfully.

