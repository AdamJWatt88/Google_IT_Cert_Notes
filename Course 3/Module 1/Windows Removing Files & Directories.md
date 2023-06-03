-   In Windows, files and directories can be removed by right-clicking and selecting "delete". The files end up in the recycle bin, which can be accessed from the desktop.
-   In **PowerShell,** the command to **remove files** and directories is **"rm"** or "remove".
-   When using **"remove"** in **PowerShell**, caution should be taken as the files or directories are **permanently deleted** and not sent to the recycle bin.
-   To remove a file, use the command **"rm filename".** 
	`rm filename`
- To **remove a directory**, use 
	`rm -r directoryname`
-   The **"-Force"** parameter can be used to bypass safety measures and forcefully remove files, but should be used with caution.
-   If the file or directory belongs to someone else or requires administrator permission to remove, access to an administrator account may be necessary.
-   When removing a directory with the **"-r"** parameter, PowerShell will prompt the user to confirm if they want to remove all contents within the directory.

#windows-CLI #powershell #remove-files #course3-module1 