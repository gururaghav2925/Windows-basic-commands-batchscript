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
```
mkdir %userprofile%\Desktop\MyLab
```
![Screenshot from 2024-04-29 01-11-33](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/6de9f905-8445-4890-8c5f-ad8d0071e397)

![Screenshot from 2024-04-29 01-11-49](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/f0bf605d-0bf9-4173-bb7b-fc7d212dc3f7)


Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
List the contents of the "MyLab" directory.
```
cd %userprofile%\Desktop\MyLab
```

![Screenshot from 2024-04-29 01-11-57](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/6a804ed6-4bd9-4ab2-98ce-dcde064d15aa)





## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
dir %userprofile%\Desktop\MyLab
```


![Screenshot from 2024-04-29 01-12-09](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/ecaacfdb-43bf-47ff-ae61-80760fecbd8f)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```

![Screenshot from 2024-04-29 01-12-23](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/627a6d92-09b2-495b-b843-d03e8cd56d52)


![Screenshot from 2024-04-29 01-12-47](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/79a36b04-c55a-4c14-9278-556f8fc96843)


## COMMAND AND OUTPUT

```
mv Myfile.txt %userprofile%\Documents
```

![Screenshot from 2024-04-29 01-12-55](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/00ad6588-0cc1-45dc-99ea-b68951d5ed29)

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

![Screenshot from 2024-04-29 01-19-58](https://github.com/gururaghav2925/Windows-basic-commands-batchscript/assets/151489500/271624c1-57b7-4335-9e86-2ce0fa59ff4a)




# RESULT:
The commands/batch files are executed successfully.

