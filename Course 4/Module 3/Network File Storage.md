-   **FAT32** is a popular file system that's compatible with **Windows**, **Linux**, and **Mac** OS's but has **severe limitations** on the amount of data you can store on a volume
-   **Network file system (NFS**) is a **protocol** that enables files to be **shared over a network** and is **compatible** with all **major operating systems**
-   Setting up an **NFS** server is **easiest** in a **Linux** environment by installing the NFS server software and modifying the configuration files for the directories you want to allow shared access to
-   On each client machine that wants to access the server, you just **mount the file system** the way you would any other file system except, you'd use the **host name** instead of a **physical disk device**.
-   NFS is a good solution for file-sharing within a network but heavy usage will slow down the file system, and **interoperability issues** may arise with **Windows**
-   **Samba** services are **similar** to **NFS** and allow you to centrally share and manage file services with **interoperability across all major operating systems**, making it a **better** option for organizations that primarily use **Windows** machines
-   **SMB is a protocol that Samba implements**, and when you create a Windows shared folder, it's actually using the SMB protocol
-   **Network Attached Storage (NAS)** is a relatively affordable solution for file storage hardware that is optimized for file storage and comes with lots of storage space
-   Central file storage and management is an important part of IT infrastructure for any organization

# Supplemental Reading for Network File Storage

- For more information on **SMB** click [here](https://technet.microsoft.com/en-us/library/hh831795(v=ws.11).aspx) and for **NFS server software** click [here](http://www.linuxfromscratch.org/blfs/view/cvs/basicnet/nfs-utils.html).

#NAS #samba #SMB #NFS #course4-module3 