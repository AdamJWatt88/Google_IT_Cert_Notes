-   To **close a process** before it fully completes, we use a **signal** to tell a process to quit at the **system level**.
-   A signal is a way to tell a process that something has just happened, and can be generated with special characters on the keyboard or through other processes and software.
-   One of the most common signals is called **SIGINT**, which stands for signal interrupt, and can be sent to a running process with the **Control+C** key combination.
-   In Windows, there are a few other signals that processes can send and receive, but there isn't an easy way for an end-user to issue arbitrary signal commands.

# Supplemental Reading for Windows Signal

- For more information about signal handling in Windows, check out the link [here](https://docs.microsoft.com/en-us/cpp/c-runtime-library/reference/signal).

#windows #signal #SIGINT #course3-module5 