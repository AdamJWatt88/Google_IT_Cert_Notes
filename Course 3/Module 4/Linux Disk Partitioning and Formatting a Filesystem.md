-   Linux has multiple partitioning command-line tools, including "parted" that supports MBR and GPT partitioning
-   Parted can be used in two modes: interactive and command-line
-   To list disks connected to a computer, use `parted -l` command
-   In interactive mode, use `sudo parted /dev/sda` to select and partition the desired disk. /dev/sda will change and can be determined by looking at the path from the `parted -l` command as shown below
![[disk-dev-sda.png]]
-  Use the `print` command to view the disk you are currently in
- Use `mklabel gpt` to set the disk label as GPT
-   Use `mkpart` command to create a partition with partition type, file system, start and end points
	example `mkpart primary ext4 1MiB 5GiB`
-   Use `mkfs` command to format the partition with a file system
	example `sudo mkfs -t ext4 /dev/sda1`
-   Be careful when using the parted tool as it's powerful and modifying the wrong disk could cause damage
-   To use the disk, it needs to be mounted to a directory.

#command-line #linux #disk-partitioning #disk-formatting #course3-module4 