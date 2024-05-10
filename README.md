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
![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/1725791e-1140-4b73-9dc0-a5a4822f522f)


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
cd %userprofile%\Desktop\MyLab
```
![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/c113d6c2-db90-4787-8a1a-6429bfcb3adc)

```
type nul > MyFile.txt
```
![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/9467150c-bf17-45e2-9983-dbbd54ae13f3)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.

```
dir %userprofile%\Desktop\MyLab
```
![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/4037c955-e801-4656-b800-91626d64090d)

## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

```
mkdir %userprofile%\Desktop\Backup
```

![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/871b4d21-123a-4211-bfe2-97e2b3e948d3)

## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.
```
copy MyFile.txt %userprofile%\Desktop\Backup
```

![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/79cb52b2-b095-458d-b6e7-1270ce1e2b40)


## COMMAND AND OUTPUT

```
mkdir %userprofile%\Desktop\Documents

move MyLab Documents
```
![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/152cefea-a1a6-43b5-bf0b-030d266017bd)


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

![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/e584b2a0-dae3-4803-b790-4201b0a4ed15)

## COMMAND 

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\*.docx
echo Backup and deletion completed successfully!
```
## OUTPUT

![image](https://github.com/harinisaravanan10/Windows-basic-commands-batchscript/assets/149035598/8b3b5820-f771-46c9-8413-01091626c93e)


# RESULT:
The commands/batch files are executed successfully.

