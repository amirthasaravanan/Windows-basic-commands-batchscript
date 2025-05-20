# Windows-basic-commands-batchscript
Ex08-Windows-basic-commands-batchscript

# AIM:
To execute Windows basic commands and batch scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Windows environment installed on the system or installed inside a virtual environment like virtual box/vmware 

### Step 2:

Write the Windows commands / batch file . Save each script in a file with a .bat extension. Ensure you have the necessary permissions to perform the operations. Adapt paths as needed based on your system configuration.
### Step 3:

Execute the necessary commands/batch file for the desired output. 

# WINDOWS COMMANDS:
## Exercise 1: Basic Directory and File Operations
Create a directory named "MyLab" on the desktop.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/84bf044a-5c1d-4ba3-b1a4-3ba51a13c18b)

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.


## COMMAND AND OUTPUT
cd %userprofile%\Desktop\MyLab

![Screenshot 2025-05-13 221558](https://github.com/user-attachments/assets/975a1835-bb3c-4ce7-b208-cec3f320a1e4)

type nul > MyFile.txt

![Screenshot 2025-05-13 221640](https://github.com/user-attachments/assets/d95cf2bd-a177-48b6-adb6-97684ffcb1b6)

List the contents of the "MyLab" directory.


## COMMAND AND OUTPUT
dir %userprofile%\Desktop\MyLab

![image](https://github.com/user-attachments/assets/15a2c38f-2bd5-49e5-9840-ac333873c9cb)

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.

## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/2a4bceb9-95a4-4072-91d4-90272c047645)

copy MyFile.txt %userprofile%\Desktop\Backup

![image](https://github.com/user-attachments/assets/1f5c440c-a33f-4c5d-b1a7-fc98496e2157)

Move the "MyLab" directory to the "Documents" folder.


## COMMAND AND OUTPUT
mkdir %userprofile%\Desktop\Documents

![image](https://github.com/user-attachments/assets/b3a17a37-68fe-4535-8e3d-57bfa9a3f8c3)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.


```

@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
echo Backup completed successfully!
```




## OUTPUT

![Screenshot 2025-05-13 222127](https://github.com/user-attachments/assets/109eba64-6182-4e9e-8250-ec69b28d6493)



# RESULT:
The commands/batch files are executed successfully.




