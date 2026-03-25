📘 Linux Practice Tasks – Task 3
📂 File Filtering Using find Command
🎯 Objective

Learn how to filter and list files based on time and size using Linux commands.

🧩 Task 3.1: List Files Not Modified in Last 7 Days
📌 Requirement
List all files that have not been modified in the last 7 days
💻 Command Used
find . -type f -mtime +7
📖 Command Explanation
🔹 find
Used to search for files and directories
🔹 .
Represents the current directory
🔹 -type f
Filters only files (not directories)
🔹 -mtime +7
Finds files modified more than 7 days ago

👉 Why we use it:
To identify old or unused files that may need cleanup or archiving.

🌍 Real-World Use Case
Cleaning up old log files
Identifying unused files in servers
Managing storage in production systems
Automating cleanup jobs using cron
🧩 Task 3.2: List Files Larger Than 1 MB
📌 Requirement
List all files that are greater than 1 MB in size
💻 Command Used
find . -type f -size +1M
📖 Command Explanation
🔹 -size +1M
Finds files larger than 1 Megabyte

👉 Why we use it:
Helps in identifying large files that consume disk space.

🌍 Real-World Use Case
Finding large log or dump files
Disk space monitoring and optimization
Identifying unnecessary large files in servers
Used in DevOps for storage management
🔍 Verification
ls -lh
📈 Key Learnings
Using find command for file filtering
Filtering files based on modification time
Filtering files based on size
Importance of file cleanup in system maintenance