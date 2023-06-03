-   **PuTTY** supports **SCP** protocol for **file transfer**
-   PuTTY package has **PuTTY Secure Copy Client (pscp.exe)** tool for copying files
-   Using `pscp.exe` inside Powershell or command prompt to **copy files** is similar to using the Linux SCP command
	`pscp.exe C:\Users\cindy\Desktop\my_file.txt cindy@104.131.122.215`
-  **Sharing folders** in Windows is an alternative way to transfer files
-   Shared folders allow users to access files by sharing a folder with them
-   To **share a folder** in Windows, **right-click** on the **folder,** select **"Share with"** > **"Specific people"**, and **add users** or **groups** to share with
-   Access shared folders on other computers by **mapping the folder** with the **"Map network drive"** option or accessing it directly from the run box using the **computer name** and **folder name**
-   The `net share` command can also be used to share folders from the command line
	Example using an elevated/administrator level Powershell prompt to give everyone full permission access to a folder called SharedFolder:
	`net share SharedFolder=C:\Users\cindy\Desktop\SharedFolder /grant:everyone,full`
-   `net share` command requires specifying permissions for users and can be used to list currently shared folders on the computer
-   For more information on `net share`, refer to the documentation in the supplemental reading

# Supplemental Reading for Remote Connection File Transfer in Windows

## For more information about managing shared resources in Windows, check out the link [here](https://technet.microsoft.com/en-us/library/hh750728(v=ws.11).aspx).

#remote-connections #file-transfer #shared-folders #windows #course3-module6 