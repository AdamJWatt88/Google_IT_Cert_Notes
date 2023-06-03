-   Network services are an important part of IT infrastructure, and file transfer services are commonly used in organizations.
-   There are **several file transfer protocol** services available, including **FTP, SFTP, and TFTP**.
-   **FTP (File Transfer Protocol**) is a legacy way to transfer files, and it is **not super secure** because it doesn't handle data encryption
	-   FTP service works much like SSH service. 
	-   Clients that want to access an FTP server have to install an FTP client. On the FTP server, we install the software that allows us to share information located in a directory on that server. 
	-   FTP is primarily used today to share web content. If you use a website host provider, you might see that they have an FTP connection already available for use. They can easily copy files to and from your website.
-  **SFTP (Secure File Transfer Protocol)** is a **secure** version of FTP, and data is sent through **SSH** and **encrypted**.
-   **TFTP (Trivial File Transfer Protocol)** is a simpler way to transfer files than FTP and **doesn't require user authentication**.
-   **TFTP** is often used to **host installation files**, particularly for **PXE (Pre Boot Execution)** or **pixie boot**.
-   Network file storage services are a good option for sharing files between computers in a secure way and accessing shared files without transferring them

# Supplemental Reading for FTP Clients

-  For more information on **PXE Boot** click [here](https://en.wikipedia.org/wiki/Preboot_Execution_Environment) and for **FTP Clients** click [here](https://en.wikipedia.org/wiki/Comparison_of_FTP_client_software).

**Heads up:** A big part of being successful in an IT role is the ability to be a self-led learner -- someone who finds key resources and reads up on the latest tech trends and solutions. The supplemental readings we’ve provided have been designed to show you just some of the support materials available to you online; they’re not meant to be considered a comprehensive list. Feel free to add to the conversation by posting other useful resources for learners to [this forum thread](https://www.coursera.org/learn/os-power-user/discussions/forums/Z4bUA0QoEeiObQoMm0s4jA/threads/tYJ-6kQvEeit7AqVmIofMg).

#FTP #SFTP #TFTP #pixie-boot #PXE #course4-module2 