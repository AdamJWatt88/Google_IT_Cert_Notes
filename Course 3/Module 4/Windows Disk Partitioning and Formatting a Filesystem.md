-   **Windows** has a **native tool** called **Disk Management Utility** to partition a disk and format a file system.
-   Launch the Disk Management Utility by **right-clicking "This PC"**, selecting the **"Manage"** option, and clicking the **"Disk Management"** console under the storage grouping.
-  **Disk Management** shows the disks and disk partitions, along with information about what type of file system they're formatted with, and the free and total capacity of disks and partitions.
-   To **partition** a USB drive using** Disk Management**, right-click on the partition and choose **"Format"**. Choose the volume label, the file system, and the allocation unit size. Choose between a quick or full format, and enable or disable file or folder compression.
-   Windows warns that formatting the volume will erase any data that might be on it. Once confirmed, it'll start the formatting process.
-   Disk manipulation can be done from the **command line** using a tool called **Diskpart.** Launch Diskpart by opening up a command prompt and typing `diskpart` into it.
	-  To see a list of available disks use the command `list disk`
	-  Select a disk from the list of disks by it's numerical value with the `select disk` command
	-  Wipe the disk using the `clean` command, 
	-  Create a partition using the `create partition primary` command
	-  Select the partition with the `select partition` command and the partition numerical value
	-  Mark the partition as active using the `active` command
	-  Format the disk using the `format FS=NTFS` command (the format type can be NTFS, FAT, FAT32, etc), followed by the label and the formatting type. 
		`format FS=NTFS label=my-thumb-drive quick`

# Supplemental Reading for Disk Partitioning and Formatting in Windows

# Disk Partitioning and Formatting in Windows

Disk partitioning enables more efficient management of hard disk space by breaking or “slicing” up the disk storage space into partitions. This breaking allows for each partition to be managed separately by reducing inefficient use of space. DiskPart is a disk partitioning utility on the Windows operating system which uses the command line to perform operations. This reading covers the component parts that make up a drive, common DiskPart commands, and how cluster size affects your usable drive space in the Windows OS. 

# DiskPart

The DiskPart command terminal helps you manage storage on your computer's drives. DiskPart utility can be used to manage partitions of hard disks including creating, deleting, merging, or expanding partitions and volumes. It can also be used to assign a file formatting system to a partition or volume. 

There are three main divisions of storage that you will find on a drive: cluster, volume, and partition. 

-   **Cluster** (allocation unit size) is the minimum amount of space a file can take up in a volume or drive.
    
-   **Volume** is a single accessible storage area with a single file system; this can be across a single disk or multiple. 
    
-   **Partition** is a logical division of a hard disk that can create unique spaces on a single drive. Generally used for allowing multiple operating systems.
    

To use DiskPart you will need to use specific commands to select and manage the parts of your drive you need to access. For a list of common DiskPart terminal commands visit [this helpful guide.](https://drive.google.com/file/d/1qDFyYB5uYLranPk9pZBz0heq0B5hmroH/view)

The commands let you work with partitions and volumes but the base storage unit called cluster size is set when initiating the volume or partition. 

# Cluster Size

Cluster size is the smallest division of storage possible in a drive. Cluster size is important because a file will take up the entire size of the cluster regardless of how much space it actually requires in the cluster. 

![Example of cluster storage space lost](https://d3c33hcgiwev3.cloudfront.net/imageAssetProxy.v1/sdNzM6Z8ToaTczOmfE6Gdw_f0855e888d6e4cf9af4fe347899318f1_clusterSize_diskpart.png?expiry=1682985600000&hmac=Ee_9sF0X2iNT1e5RynVAwfBZrs4CsM39uN9ngShHvsM)

For example, if the cluster size is 4kb (the default size for many formats and sizes) and the file you're trying to store is 4.1kb, that file will take up 2 clusters. This means that the drive has effectively lost 3.9 kb of space for use on a single file. 

When partitioning a disk, you should specify the cluster size based on your file sizes. If no cluster size is specified when you format a partition, a default is selected based on the size of the partition. Using defaults can result in loss of usable storage space.

It is important to remember when using DiskPart that the actions you take are permanent so be careful not to erase data accidentally.

## Key Takeaways

DiskPart is a tool that lets you manage your storage from a command line interface and is useful for a multitude of actions including creating, deleting, merging, and repairing drives.

-   The three main divisions of storage that you will find on a drive are cluster, volume, and partition. 
    
-   To use DiskPart you will need to use specific commands to select and manage the parts of your drive you need to access. 
    
-   Cluster size is the smallest division of storage possible in a drive. Cluster size is important because a file will take up the entire size of the cluster regardless of how much space it actually requires in the cluster.

#windows #disk-partitioning #disk-formatting #disk-partitioning #course3-module4 