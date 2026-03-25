📘 Linux Practice Tasks
📂 Task 1: Create Nested Directories and File
🎯 Objective

Learn how to create nested directories and files using basic Linux commands.

📌 Requirement
Create a folder structure:
folder1/folder2/folder3
Create a file named devops inside folder3
💻 Commands Used
# Create nested directories
mkdir -p folder1/folder2/folder3

# Create a file inside folder3
touch folder1/folder2/folder3/devops
📖 Command Explanation
🔹 mkdir -p
mkdir → Command used to create directories
-p → Creates parent directories if they don’t exist

👉 Why we use it:
Normally, mkdir fails if parent directories don’t exist.
Using -p ensures the entire directory structure is created in one command without errors.

🔹 touch
Used to create an empty file

👉 Why we use it:

Quickly create files
Create log files
Initialize configuration files in projects
📂 Output Structure
folder1/
 └── folder2/
      └── folder3/
           └── devops



Verification
ls folder1/folder2/folder3

Expected Output:

devops           