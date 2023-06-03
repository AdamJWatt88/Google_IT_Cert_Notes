-   **Processes are programs** in motion that represent how operating systems work.
-   The operating system turns resting code into a running, responding, working application, which becomes a process.
-   Processes are interacted with, launched, and halted on computers all the time, although the OS usually handles it behind the scenes.
-   Understanding processes gives a peek behind the curtain at how operating systems really work and is fascinating and powerful, especially when applied by an IT support specialist to solve problems.
-   The **task manager** or `taskmgr.exe` is one method of obtaining process information. You can open it with the **Ctrl+Shift+Esc** key combination or by locating it using the **start menu**.
-   The **processes tab** in the **task manager** displays a list of processes that the current user is running along with a few **system-level processes** that the user can see.
-   To **kill a process**, you can select any of the process rows and click the end task button in the lower right corner.
-   The details menu option in the task manager displays a whole bunch of other information, including the **PID**.
-   Using the **PID** in combination with `taskkill` in the **command line prompt**, you can end tasks
-   From the **command prompt**, you can use the utility called `tasklist` to show all the running processes.
-   From a **PowerShell prompt**, you can use the command list called `Get-Process` to do the same.

# Supplemental Reading for Reading Process Information in Windows

For more information about _get-process_, or using PowerShell to get the processes that are running on a computer, check out the link [here](https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.management/get-process?view=powershell-5.1).

#processes #task-manager #PID #taskkill #command-prompt #windows #course3-module5 