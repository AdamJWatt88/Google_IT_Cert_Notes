-   Unplugging a USB device without ejecting or unmounting it from the computer can cause data corruption because data may still be in the buffer or cache.
-   Data corruption can also occur due to system failures, software bugs, or sudden power outages.
-   **NTFS** file system has **built-in features** like **journaling** and **self-healing** that can minimize the risk of corruption and recover from it when it happens.
-   Journaling logs changes made to a file's metadata into a log file, creating a history of actions taken by the file system.
-   **Self-healing** mechanism **automatically** makes changes to **minor problems** and **corruption** on the disk in the background while Windows is running
-   If you want to check the **status** of the **self-healing** process on your computer, you can open up an **administrative command prompt** and use the `fsutil` tool
	example`fsutil repair query C:`
-  **Check disk utility** is available in emergencies for serious or catastrophic disk corruption like bad disk sectors or disk failures
-  To run check disk manually, you can open up an administrator command prompt and type check disk onto the command line
	`chkdsk /F D:`
-   The NTFS file system has robust measures and features in place to recover and prevent corruption from breaking your partitions.
-   In Linux, you can perform file system repairs using utilities like fsck and e2fsck.

#chkdsk #fsutil #windows #course3-module4 