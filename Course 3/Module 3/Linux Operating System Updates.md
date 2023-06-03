-   In Linux, use `apt update` and `apt upgrade` commands to update and upgrade software. apt upgrade may install security updates but not upgrade the core operating system.
-   In Linux, the kernel controls the core components of the operating system and includes security patches, new features, and bug fixes. To update the kernel and other packages, use `apt full-upgrade` after updating application sources with `apt update`.
-   Use `uname` command with `-r` flag to view the current kernel version.
-   After installing a new kernel, reboot the computer and verify the latest kernel version with `uname -r` command.
-   These skills are useful for IT support specialists to maintain and update software.

# Supplemental Reading for Linux Update

# Linux Update

Linux is a free, open-source operating system used on a wide variety of computing systems, such as embedded devices, mobile devices including its use in the Android operating system, personal computers, servers, mainframes, and supercomputers. The Linux kernel is the core interface between a device’s hardware and the rest of its processes. The kernel controls all the major functions of hardware running the Linux operating system. To keep the core operating system up to date with current security patches, new features, and bug patches, you need to update the Linux kernel. This reading covers how the Linux kernel functions and how to update Ubuntu, the most common Linux distribution. 

# Linux kernel

The Linux kernel is the main component of a Linux operating system (OS). The kernel is software located in the memory that tells the central processing unit (CPU) what to do. The Linux kernel is like a personal assistant for the hardware that relays messages and requests from users to the hardware. 

The kernel has four main jobs:

1.  **Memory management** tracks how much memory is being used by what and where it is stored. 
    
2.  **Process management** determines which processes can use the central processing unit (CPU), when, and for how long.
    
3.  **Device drivers** act as an interpreter between the hardware and processes.
    
4.  **System calls and security** receives requests for service from the processes.
    

To ensure that Linux distribution is running the most current version of the operating system, you will need to update it regularly. 

# Updating Ubuntu Linux distribution

A Linux distribution is an operating system (OS) that includes the Linux kernel and usually a package management system. There are almost one thousand Linux distributions, and each distribution has a slightly different way of updating.

The Ubuntu distribution is one of the most popular since it is easy to use. There are two ways to update the Ubuntu distribution:

-   **Update Manager** is a graphical user interface (GUI) that is nearly 100% automated. When updates are available, it will open on your desktop and prompt you to complete the updates. It checks for security updates daily and nonsecurity updates weekly. You can also choose to check for updates manually.
    
-   **Apt** is the Ubuntu package management system that uses command line tools to update a Ubuntu distribution. Apt does not check for updates automatically, you must manually run it to check for updates. You can use the following commands to check for updates and upgrade:
    

1.  apt-get update To update with apt, open the terminal and use the command apt-get update**.** This command prompts you to enter your password, then it updates the list of system packages. 
    
2.  apt-get upgrade Once the package list is up to date, use the command apt-get upgrade to actually download and install all updated versions for the packages in the list.
    

# Key Takeaways

Linux is a free open-source operating system used on a wide variety of computing systems.  

-   The kernel is a part of the operating system of Linux and runs communications between the computer’s hardware and its processes. 
    
-   Unbuntu is the most popular distribution because it is easy to use and update with the update manager or the command sudo apt-get upgrade.
    
-   As improvements to the processes are released, Linux needs to be updated to ensure the kernel communicates the right information to the hardware about the process. 
    

# Resources for more information

For more information on updating various distributions of Linux, visit this [Linux Foundation article.](https://www.linuxfoundation.org/blog/classic-sysadmin-linux-101-updating-your-system/) 

For more complete command information for using apt in Ubuntu, visit [Ubuntu’s guide here](https://manpages.ubuntu.com/manpages/bionic/en/man8/apt.8.html).