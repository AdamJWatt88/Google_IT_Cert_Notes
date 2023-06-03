-   `du` or "disk usage" command in Linux:
    
    -   Shows disk usage of a specific directory.
    -   Default to current directory if no directory is specified.
    -   Use the `-h` flag for human-readable format.
    -   Used to know how much disk space is being used by files in a directory.
-   `df` or "disk free" command in Linux:
    
    -   Shows free space available in the entire system.
    -   Use the `-h` flag for human-readable format.
    -   Used to know how much free space is available in the system.
-   In Windows, disk utilization can be checked using:
    
    -   Computer Management utility and Disk Management Console:
        -   Right-click on the partition and select Properties to view used and free space on the drive.
    -   DU command from Sysinternals tool suite:
        -   Provides text-based output and usage of a given disk, useful for creating scripts.
        -   Link to the tool is provided in supplemental reading.
    -   Disk Cleanup tool:
        -   Launches "cleanmgr.exe" program to delete temporary files, compress old files, clean up logs, and empty the recycle bin.
    -   Disk defragmentation:
        -   Reorganizes files on a given disk to make reading data easier.
        -   Less beneficial for solid-state drives, which can use the "trim" process to reclaim unused portions of the disk.
        -   In Windows, handled as a scheduled task, but can be manually run using the Disk Defragmenter tool.

# Supplemental reading for Linux Disk Usage

To learn more about why Linux doesn't need defragmentation, check out the article [here](https://www.howtogeek.com/115229/htg-explains-why-linux-doesnt-need-defragmenting/).

#linux #disk-management #disk-usage #course3-module4 