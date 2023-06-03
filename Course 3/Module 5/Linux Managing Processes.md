-   **Terminating Processes**
    -   Use the `kill` command with **process ID (PID)** to terminate a process
    -   `kill` command without any flags sends a **SIGTERM** signal, giving the process time to **clean up** resources
    -   Using **SIGKILL** signal (`kill -KILL`) will kill the process **immediately** **without cleaning up** resources
    -   Use SIGKILL as a **last resort** since it could cause harm to files
-  **Suspending Processes**
    -   Send the **SIGTSTP** signal to **suspend** a process using `kill -TSTP` or keyboard combination `Ctrl-Z`
    -   Use **SIGCONT** signal to resume the execution of the process
-   Common signals to work with processes in Linux
    -  **SIGTERM**, **SIGKILL**, **SIGTSTP**, and **SIGCONT**
-   Using signals to manage processes can help utilize resources efficiently.

#linux #process-management #course3-module5 