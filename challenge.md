# Security Detective Challenge



## Q1. Current User and Directory



Commands:

- `whoami`

- `pwd`



Answer: Write your actual username and current directory.



## Q2. Hostname and Operating System



Commands:

- `hostname`

- `cat /etc/os-release | head -2`



Answer: Write your actual hostname and operating system details.



## Q3. Memory and Disk Space



Commands:

- `free -h`

- `df -h /`



Answer: Record the available memory and root filesystem disk-space information.



## Q4. Users Using Bash



Command:

- `grep '/bin/bash' /etc/passwd`



Answer: Record the users displayed by the command.



## Q5. Number of Processes



Command:

- `ps aux | wc -l`



Answer: Record the number returned by the command. This count includes the header line.



## Q6. Authentication Log



Command:

- `sudo grep lab5user /var/log/auth.log | tail -20`



Alternative if `auth.log` is unavailable:

- `sudo journalctl | grep lab5user | tail -20`



Answer: Record the relevant log entries if any are available. If no
