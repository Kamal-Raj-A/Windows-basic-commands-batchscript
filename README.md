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
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/88934ef7-61d9-4d38-8bb5-acb28102092f)


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.
```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/815bbd8b-5aa7-4a85-9464-8e932c08da95)
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/438cf7cf-5ec6-4c41-92c2-d1315208b55f)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/d4845d17-ac2f-408f-a1b9-045c473ca93a)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
mkdir %userprofile%\Desktop\Backup

copy MyFile.txt %userprofile%\Desktop\Backup
```
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/15572011-cd8c-44f4-a19d-9ad7321e37a5)
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/02f5e392-fb08-4ddd-9258-459225120f3f)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
mv Myfile.txt %userprofile%\Documents
```
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/0d37a654-4787-41a5-9f50-51d6cf80d3bc)



## COMMAND AND OUTPUT


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
![image](https://github.com/Kamal-Raj-A/Windows-basic-commands-batchscript/assets/145742556/aafb2e10-7a0a-4ea9-99f9-529dc2932974)
# RESULT:
The commands/batch files are executed successfully.

