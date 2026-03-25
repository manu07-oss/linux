📘 Linux Practice Tasks – Task 2
📂 File and Folder Copy Operations
🎯 Objective

Learn how to copy files and directories in Linux using different scenarios and commands.

🧩 Task 2.1: Copy All Files and Folders
📌 Requirement
You have two folders: folder1 and folder2
folder1 contains files and subfolders
Copy all contents from folder1 to folder2
💻 Command Used
cp -r folder1/* folder2/
📖 Command Explanation
🔹 cp
Used to copy files and directories
🔹 -r (recursive)
Copies directories along with their contents
🔹 folder1/*
Selects all files and folders inside folder1

👉 Why we use it:
To copy complete directory content including subfolders in one command, which is very common in deployments and backups.

🌍 Real-World Use Case
Copying application code from one directory to another
Backing up project files
Moving build artifacts in CI/CD pipelines
🧩 Task 2.2: Copy Data from One File to Multiple Files
📌 Requirement
You have 5 files: file1, file2, file3, file4, file5
file1 contains data
Copy the same data into the other 4 files at once
💻 Command Used
tee file2 file3 file4 file5 < file1
📖 Command Explanation
🔹 tee
Reads input and writes to multiple files simultaneously
🔹 < file1
Takes input (data) from file1

👉 Why we use it:
Instead of copying manually into each file, tee allows writing the same content to multiple files in one command.


🌍 Real-World Use Case
Creating multiple config files with same content
Distributing logs or templates
Writing output to multiple destinations in automation scripts
🧩 Task 2.3: Copy File from One Folder to Another
📌 Requirement
You have two folders: folder1 and folder2
folder1 contains a file with data
Copy that file to folder2
💻 Command Used
cp folder1/* folder2/
📖 Command Explanation
Copies all files from folder1 to folder2

👉 Why we use it:
Simple and commonly used command to transfer files between directories.

📂 Alternative (Specific File)
cp folder1/filename folder2/
🌍 Real-World Use Case
Moving configuration files between environments
Copying logs or reports
Deploying application files to target directories
🔍 Verification
ls folder2
📈 Key Learnings
Use of cp for file and directory copying
Importance of -r for recursive operations
Using tee for multi-file writing
Understanding file movement across directories