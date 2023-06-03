-   **Logs** in Linux are stored in the **/var/log directory**, which stands for **"variable"** files that constantly change.
-   **/var/log directory** contains various **log files,** each storing specific information, identified by their filenames.
-   Some **common log files** in **/var/log** directory are:
    -   **/var/log/auth.log**: Authorization and security-related events.
    -  **/var/log/kern.log**: Kernel messages.
    -   **/var/log/dmesg**: System startup messages.
    -  **/var/log/syslog**: The most comprehensive log file that logs almost everything on the system.
-   Linux uses **log rotation** to clean out old logs and make room for new ones. The utility to rotate logs is called **logrotate**.
-   **Unix** or **epoch time** is a timestamp format used in some logs, representing the number of seconds since midnight on **January 1, 1970**, which is the **zero hour** for **Unix-based** computers to anchor their concept of time.

# Supplemental Reading for Linux Logs

- For more information about _logrotate_, or the command to manage large numbers of log files in Linux, check out the link [here](http://manpages.ubuntu.com/manpages/zesty/man8/logrotate.8.html).

#linux #system-logs #log-rotation #logrotate #epoch-time #course3-module6 