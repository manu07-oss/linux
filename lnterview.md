1 & 2 & 17 & 21. Disk space usage?

Command: df -h
Answer (20 words):
Use df -h to check disk usage. It shows filesystem, used, available space in human-readable format for quick monitoring.

3 & 4 & 30. Where are system logs stored?

Answer (20 words):
System logs are stored in /var/log directory. Important files include syslog, messages, auth.log for system, authentication, and application logs.

5 & 38. Server not starting?

Answer (20 words):
Check logs in /var/log, use journalctl, verify services, disk space, configuration errors, and restart services to identify root cause.

6 & 18. Disk full troubleshooting?

Answer (20 words):
Use df -h, du -sh, find large files, delete unnecessary logs, clean temp files, and monitor disk usage regularly.

7. File permissions + execute permission?

Command: chmod u+x file
Answer (20 words):
Linux permissions include read, write, execute. Use chmod u+x to give execute permission to user for running scripts or binaries.

8. Change file permissions?

Command: chmod 755 file
Answer (20 words):
Use chmod command to change permissions. It supports symbolic and numeric modes to control read, write, execute access for users.

9. What is 777?

Answer (20 words):
777 means read, write, execute permissions for owner, group, and others. It gives full access, but is insecure in production environments.

10. Numeric values?

Answer (20 words):
Read equals 4, write equals 2, execute equals 1. Combined values define permissions like 7 equals full access for users.

11. Default permissions?

Answer (20 words):
Default file permission is 644 and directory is 755. Controlled by umask value, which restricts default permission settings.

12. Change ownership?

Command: chown user:group file
Answer (20 words):
Use chown to change file ownership. It assigns user and group ownership for access control and proper permission management.

13. Root cannot create file?

Answer (20 words):
Check disk space, file system mounted read-only, inode exhaustion, or permission issues. Root usually has access unless system limitations exist.

14 & 15. Create user + group?

Command:

useradd user
usermod -aG group user

Answer (20 words):
Use useradd to create user and usermod -aG to assign group. Helps manage access and permissions in multi-user environments.

16. User details stored?

Answer (20 words):
User details are stored in /etc/passwd, encrypted passwords in /etc/shadow, and group information in /etc/group for system authentication.

19. Disk free but cannot perform?

Answer (20 words):
Check inode usage using df -i. Even if space is free, inode exhaustion prevents file creation or modification in system.

20. Largest files?

Command:

du -ah . | sort -rh | head -10

Answer (20 words):
Use du, sort, head commands to find largest files. Helps identify disk-consuming files for cleanup and storage optimization.

22. CPU, memory, processes?

Command: top
Answer (20 words):
Use top command to monitor CPU, memory, and processes in real time. Helps identify high resource-consuming applications.

23. Memory usage?

Command: free -h
Answer (20 words):
Use free -h to check memory usage. It shows total, used, free, and available memory in human-readable format.

24. CPU usage?

Command: top / mpstat
Answer (20 words):
Use top or mpstat to monitor CPU usage. Helps analyze load, performance bottlenecks, and running processes affecting CPU.

25. What is free?

Answer (20 words):
Free command displays memory usage including total, used, free, shared, and buffer/cache memory. Useful for monitoring system performance.

26. top vs htop?

Answer (20 words):
Top is default CLI tool. Htop is advanced, interactive, user-friendly with colors, sorting, and easier process management features.

27. Slow server?

Answer (20 words):
Check CPU, memory, disk usage, running processes, logs, network latency, and restart problematic services to identify performance bottlenecks.

28. Memory issue commands?

Answer (20 words):
Use free -h, top, vmstat, and ps commands to analyze memory usage and identify processes consuming excessive memory.

29. Zombie process?

Answer (20 words):
Zombie process is completed process with entry in process table. It occurs when parent doesn’t read exit status properly.

31. /var/log/messages?

Answer (20 words):
Contains system messages, kernel logs, hardware, and service-related logs. Useful for troubleshooting system issues and monitoring server health.

32. Live logs?

Command: tail -f file.log
Answer (20 words):
Use tail -f to monitor logs in real time. Helps track application behavior and debug issues instantly on servers.

33. Cannot SSH?

Answer (20 words):
Check network connectivity, SSH service status, firewall rules, port 22, credentials, and logs to identify connection issues.

34. Network connectivity?

Command: ping, telnet, nc
Answer (20 words):
Use ping, telnet, or nc commands to test connectivity between servers. Helps identify network issues or blocked ports.

35. Listening ports?

Command: netstat -tulnp or ss -tulnp
Answer (20 words):
Use netstat or ss command to check listening ports and services. Helps verify application availability and troubleshoot network issues.

36. Networking commands?

Answer (20 words):
Common commands include ping, traceroute, netstat, ss, curl, and nslookup. Used for diagnosing connectivity and DNS-related issues.

37. Server not coming up?

Answer (20 words):
Check boot logs, disk issues, services, configuration errors, and use rescue mode or journalctl to identify startup problems.

39. Crontab failing?

Answer (20 words):
Check cron logs, script permissions, environment variables, paths, and manually execute script to debug scheduling issues.

40. #!/bin/bash?

Answer (20 words):
Shebang defines interpreter for script execution. /bin/bash ensures script runs using Bash shell regardless of environment settings.

41. Pass arguments?

Answer (20 words):
Use $1, $2 variables to access arguments in script. Helps pass dynamic inputs while executing shell scripts.

42. Execute script?

Command: chmod +x script.sh && ./script.sh
Answer (20 words):
Make script executable using chmod and run using ./script.sh. Ensures proper execution with defined interpreter.

43. -e in shell?

Answer (20 words):
Set -e exits script immediately if any command fails. Useful for avoiding unexpected errors in automation scripts.

44. Script example?

Answer (20 words):
Used shell script for log cleanup, automation, backups, and monitoring tasks. Scripts help reduce manual effort and improve efficiency.

45. Create file?

Command: touch file
Answer (20 words):
Use touch command to create empty file quickly. Useful for logs, configs, and testing file operations.

46. Create directory?

Command: mkdir dir
Answer (20 words):
Use mkdir to create directory. With -p option, it creates nested directories efficiently without errors.

47. Soft vs Hard link?

Answer (20 words):
Soft link is shortcut, can cross filesystems. Hard link shares inode, cannot cross filesystem, remains even if original deleted.

48. hostnamectl?

Answer (20 words):
Hostnamectl shows or sets system hostname and related information like OS, kernel, architecture in systemd-based Linux systems.

49. Top Linux commands?

Answer (20 words):
Common commands include ls, cd, cp, mv, rm, grep, find, top, df, du, chmod, chown for daily system operations.

🔥 Tip for YOU

In interviews:

First say command
Then explain in simple words
Add real-world usage