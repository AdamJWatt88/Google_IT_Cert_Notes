-   **PuTTY** is free open-source software for remote connections on Windows
-   You can download the entire software package with the Microsoft installer or a specific executable like **PuTTY.exe**
-   Launch PuTTY and enter the **host name** or **IP address** of the computer you want to connect to, then click open to start a new **SSH session**
-   PuTTY can also be used on the **command line**, with the -ssh option and specifying user, IP address, and port
	  `putty.exe -ssh cindy@104.131.122.215 22`
-   PuTTY includes a tool called **plink** for remote SSH connections
-   **Microsoft Remote Desktop Protocol (RDP)** is another way to connect to Windows computers
-   **RDP** provides a **graphical user interface** to remote computers, with a client program called mstsc.exe
-   To **enable remote connections** on a Windows computer, **open properties** and select **remote settings**, but only let trusted users access it
-   Launch **RDP** client with `mstsc` command or look it up in the **start menu**
-   Enter the **name** or **IP address** of the computer you want to connect to, with optional parameters like **"/admin"** for administrative credentials.

# Supplemental reading for Remote Connections in Windows

# Remote Connections in Windows

Connecting securely to remote machines is an important task for deploying services. Secure Shell (SSH) was developed in the 1990s to address this issue. This reading will cover what SSH is, the features it enables, and common SSH clients and their key features in Windows.

# SSH

Secure Shell (SSH) is a network protocol that gives users a secure way to access a computer over an unsecured network. SSH enables secure remote access to SSH-enabled network systems or devices and automated processes. It also allows for secure remote access to transfer files, use commands and manage network infrastructure.

## OpenSSH

OpenSSH is the open-source version of the Secure Shell (SSH) tools used by administrators of Linux and other non-Windows for cross-platform remote systems management. OpenSSH has been added to Windows (as of autumn 2018) and is included in Windows Server and Windows client.

# Common SSH Clients

An SSH client is a program that establishes secure and authenticated SSH connections to SSH servers. The following common SSH clients are Windows compatible:

**PuTTY** is a terminal emulator and the inspiration for all subsequent remote access systems. 

-   **Features:** This tool offers Telnet, SSH, Rlogin (A remote login tool for use with UNIX-based machines on your network), and raw socket connections plus Secure File Transfer Protocol (SFTP) and Secure Copy Protocol (SCP) for file transfers between two hosts.
    
-   **Protocols**: SCP, SSH, Telnet, rlogin, and raw socket connection.
    

**SecureCRT** is a remote access system available for macOS, Linux, iOS, and Windows. 

-   **Features:** It offers terminal emulation and file transfer through an SSH tunnel. It enables connections through many protocols and has usability features like tabbed sessions and customizable menus.
    
-   **Protocols**: SSH1, SSH2, Telnet, and Telnet/SSL
    

**SmarTTY** is a free SSH client with a multi-tabbed interface to allow multiple simultaneous connections. 

-   **Features:** This tool includes SCP capabilities for file transfers. It also includes usability features like auto-completion, file panel, and package management. 
    
-   **Protocols**: SSH and SCP
    

**mRemoteNG** is a remote desktop system with a tabbed interface for multiple simultaneous connections. 

-   **Features:** The system enables connections with Remote Desktop Protocol (RDP), Telnet (two-way text communication via virtual terminal connections), Rlogin, Virtual Network Computing (VNC, a graphics-based desktop sharing system), and SSH.
    
-   **Protocols**: RDP, VNC, SSH, Telnet, HTTP/HTTPS, rlogin, Raw Socket Connections, Powershell remoting
    

**MobaXterm** is a remote access system built for Unix and Linux, and Windows. 

-   **Features:** Features include an embedded X server (a graphical interface akin to windows), X11 forwarding (a way to run applications over a remote connection), and easy display exportation to let X11 applications know which screen to run on.
    
-   **Protocols**: SSH, X11, RDP, VNC
    

# Key Takeaways

Secure Shell(SSH) is a way to securely connect two remote machines over an unsecured network.

-   You can use SSH to remotely control, transfer files from, and manage network resources for SSH-enabled clients.
    
-   OpenSSH is an open-source version for cross-platform management.
    
-   There are many common Window-compatible SSH clients with various features to fit any need, including PuTTY, SecureCRT, SmarTTY, mRemoteNG, and MobaXterm.
    

# Resources

-   [Download PuTTY](https://www.putty.org/)
    
-   [Download SecureCRT](https://www.vandyke.com/cgi-bin/releases.php?product=securecrt)
    
-   [Download SmarTTY](https://sysprogs.com/SmarTTY/download/)
    
-   [Download mRemoteNG](https://mremoteng.org/download)
    
-   [Download MobaXterm](https://mobaxterm.mobatek.net/download.html)

#remote-connections #putty #microsoft-remote-desktop-protocol #RDP #course3-module6