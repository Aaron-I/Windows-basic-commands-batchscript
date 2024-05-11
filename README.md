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

```mkdir ~/Desktop/MyLab```

![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/c2167f00-49a5-42b7-83f3-19b3f5cafe49)


## COMMAND AND OUTPUT

Change to the "MyLab" directory and create an empty text file named "MyFile.txt" inside it.

```
cd ~/Desktop/MyLab
touch MyFile.txt
```

![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/be528485-21d1-4075-9bad-2436be613a1c)


## COMMAND AND OUTPUT

List the contents of the "MyLab" directory.
```
ls
```

![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/c804a30c-09da-4800-928b-e0f1c17c6c52)



## COMMAND AND OUTPUT

Copy "MyFile.txt" to a new folder named "Backup" on the desktop.
```
cp ~/Desktop/MyLab/* ~/Desktop/Backup/
```

![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/9805499b-99a1-4641-bdf3-58498bcb86f0)


## COMMAND AND OUTPUT

Move the "MyLab" directory to the "Documents" folder.

```
cd
cd ~/Documents
```
![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/f0539ba4-d44a-4f43-968d-6b8af9e9ef07)


## COMMAND AND OUTPUT
Move the "MyLab" directory to the "Documents" folder.
```
mv ~/Desktop/MyLab/MyFile.txt ~/Desktop/Backup/
```

![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/4699e153-3dd9-42d6-a73e-477f053d9383)


## Exercise 2: Advanced Batch Scripting
Create a batch script named "BackupScript.bat" that creates a backup of files with the ".docx" extension from the "Documents" folder to a new folder named "DocBackup" on the desktop.

```
@echo off
mkdir %userprofile%\Desktop\DocBackup
copy %userprofile%\Documents\*.docx %userprofile%\Desktop\DocBackup
del %userprofile%\Documents\DocBackup\*.docx
echo Backup and deletion completed successfully!
```




## OUTPUT
![image](https://github.com/Aaron-I/Windows-basic-commands-batchscript/assets/139863034/49825b49-862a-4049-b052-111e84e79e80)





# RESULT:
The commands/batch files are executed successfully.

