-   Components of a storage disk that allow you to store and retrieve files: **partitions** and **partition tables**
-   A partition is a piece of the disk that you can manage; multiple partitions give the illusion of physically dividing a disk into separate disks
-   To add a file system to a disk, you first need to create a partition
-   A **partition table** tells the OS how the disk is partitioned, which partitions can be booted from, and how much space is allocated to each partition
-   **Two main** partition table schemes: **MBR (used mostly in Windows OS)** and **GPT (becoming the new standard for disks)**
-   **MBR** has limitations such as a volume size limit of **2 TB** and a maximum of **four primary partitions** on a disk
-  **GPT** allows for **larger volume sizes** and has only **one type of partition**, and you can **make as many partitions** as you want on a disk
-   **UEFI** booting requires the use of the GPT partition table
-   Partitioning a disk involves creating and managing partitions and partition tables
-   Next few lessons will cover how to partition and format a USB drive for each respective OS.

#disk-partitioning #file-systems #partition-table #course3-module4 