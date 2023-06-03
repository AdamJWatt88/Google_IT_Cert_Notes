-   Process creation and termination differ based on the operating system used
-   In Windows, the first non-kernel process that starts is the **Session Manager Subsystem (smss.exe)**, which sets up the OS and starts the login process and client server runtime subsystem
-   Windows processes require a parent to create them and inherit some settings and variables from the parent
-   Windows processes can operate independently of their parents
-   Killing the parent process does not necessarily stop the child process in Windows
-   Windows has a command prompt utility called `taskkill` to stop processes, which can use the **process ID (PID)** to identify and terminate a specific process
-   To terminate a process with `taskkill`, use the command `taskkill /pid pidNumber`

# Supplemental Reading for Process Creation and Termination in Windows

For more information about _taskkill_, or ending one or more tasks or processes in Windows CLI, check out the link [here](https://docs.microsoft.com/en-us/windows-server/administration/windows-commands/taskkill).

#process-management #processes #taskkill #windows #course3-module5 