
-   VirtualBox is an open-source virtualization software
-   Setting up an Ubuntu instance on a Windows machine
-   To install a virtual instance:
    -   Click the "New" button to create a new VM
    -   Give the VM a name and select the type and version of the OS
    -   Allocate RAM and hard-drive space
    -   Click "Create"
    -   Select the image to launch the installation
-   To modify hardware resource allocation:
    -   Right-click on the VM and click "Settings"
    -   Change the RAM allocation or other settings as needed
-   To remove a virtual instance:
    -   Right-click on the VM and select "Remove"
    -   Choose whether to remove all files or just remove from the list of VMs

# Supplemental reading for Virtual Machines

# Virtual Machines

Virtualization creates a simulated computer environment for running a complete operating system (OS). The simulated computer environment is called a virtual machine (VM). On a VM, you can run an OS as if it were running directly on your physical hardware. This reading explains how virtual machines work and introduces some tools for creating a VM.

# How VMs work

Virtual machine software creates a virtualized environment that behaves like a separate computer system. The VM runs in a window on the operating system of your physical computer. The operating system that runs on your physical computer is called the “host” OS. Any operating systems running inside a VM are called “guests.” In the virtual environment, you can install your guest OS, and it will function like it’s running on a physical machine. Whenever you want to use the guest OS, open your VM software and run the guest OS in a window on your host desktop.

Using a virtual machine lets you experiment with different operating systems without having to uninstall or replace your host OS. For example, you can try a Linux OS as a VM on your Windows computer to see how the two OSs compare, or you can use a VM on your Linux system to run a Mac software package. 

Another advantage of VMs is that they are isolated from the rest of your system. Software running inside a VM doesn’t affect the host OS or other VMs on your system. This isolation makes VMs a safe place to test software even when there is a risk of negative effects on a system.

A key advantage of VMs is significant reduction in hardware and electricity costs. You can run many VMs on a single host by dividing available hardware resources among each virtualized environment. Modern computer hardware offers a lot of computing power in a single device. But a typical OS will require only a fraction of the computing resources available in a computer. This means you won’t have to run those systems on several physical computers that are only partially used.

VM software divides hardware resources among virtualized environments by designating a portion of resources as virtual resources. When you create a VM you may be asked to specify the amount of physical hard drive space you want to set apart for your VM to use. The VM software will create a virtual hard drive for your VM of the specified size. VM software may have you also specify the amount of RAM you want to allocate for your VM. After you create the VM, you can usually adjust resource allocations. If you want more drive space or RAM for your VM, you can adjust the settings in the VM software to allocate more of those resources.

# VM software

Some common Virtual Machine software used to create VMs:

-   **VirtualBox** runs on Windows, Linux, Macintosh, and Solaris hosts. VirtualBox supports various guest operating systems, including Windows, Linux, Solaris, OpenBSD, and macOS. VirtualBox is open-source software available for free on the [VirtualBox download page](https://www.virtualbox.org/wiki/Downloads).
    
-   **Hyper-V** is Microsoft's virtualization platform. It is available as an integrated feature on the Windows operating system. Hyper-V supports Windows, Linux, and FreeBSD virtual machines. It does not support macOS. See [Microsoft’s Hyper-V for Windows documentation](https://docs.microsoft.com/en-us/virtualization/hyper-v-on-windows/) for information on how to access Hyper-V on recent versions of Windows.
    
-   **VMware** desktop software runs on Windows, Linux, and macOS hosts. VMware Workstation Player is the VMware software that lets users run multiple operating systems on a single physical personal computer. It is freely available for non-commercial use on the [VMware Workstation Download](https://www.vmware.com/products/workstation-player/workstation-player-evaluation.html) page.
    
-   **Red Hat Virtualization (RHV)** is a business-oriented platform developed for virtualization in enterprise computing contexts. RHV supports a variety of guest systems. Red Hat charges an annual subscription fee for product access, updates, patches, and technical support. See [Red Hat’s RHV Datasheet](https://www.redhat.com/en/resources/red-hat-virtualization-datasheet) for information on how to implement RHV on existing hardware infrastructures.
    

# Key takeaways

Virtualization lets you create a simulated computer environment for running a complete operating system. 

-   Virtual machine (VM) software creates a virtualized environment that behaves like a separate computer system.
    
-   Virtualization lets you experiment with different operating systems without having to uninstall or replace your host OS and provides a safe place to test software.
    
-   VM software divides hardware resources among virtualized environments by allocating  portions of available resources as virtual resources.
    
-   A variety of Virtual Machine software are available for creating VMs.
    

# More resources

For step-by-step instructions on how to create a virtual machine using VirtualBox, see the [VirtualBox manual](https://www.virtualbox.org/manual/ch01.html).

#virtual-machine #course3-module6 