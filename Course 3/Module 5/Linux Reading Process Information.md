-   Use `ps` command to view the processes running on the system
-   Use `ps -x` command to view a snapshot of the current processes running on the system
-   Fields in the `ps` output:
    -   **PID**: Process ID
    -   **TTY**: Terminal associated with the process
    -   **STAT**: Process status (e.g., R for running, T for stopped, S for interruptible sleep)
    -   **Time**: Total CPU time taken up by the process
    -   **Command**: Name of the command that is running
	![[ps-x-command-linux.png]]
-   Use `ps -ef` command to view all processes and their full details, including:
    -   **UID**: User ID of the person who launched the process
    -  **PPID**: Parent ID of the process that launched it
    -   **C**: Number of children processes that this process has
    -   **S time**: Start time of the process
    -   **TTY**: The terminal associated with the process.
    -   **Time**: Is the total CPU time that the process has taken up. 
    -   **CMD or Command**: The name of the command that we're running.
    ![[ps-ef_linux_command.png]]
-   Use `grep` command to search for specific processes by name
	`ps -ef | grep Chrome`
-   Processes in Linux are files, located in the **"/proc"** directory
	`ls -l /proc`
-   Each process has a directory in **"/proc"** that contains information about the process
	`cat /proc/1805/status`
-   Use `ps -ef` command for practical troubleshooting purposes

With these commands and concepts, we can easily view and understand the processes running on our Linux system.

# Supplemental Reading for Reading Process Information in Linux

- For more information about _ps_, or the command to read current processes in Linux, check out the link [here](http://man7.org/linux/man-pages/man1/ps.1.html).

#linux #processes #ps_command #ps_-ef_command #course3-module5 