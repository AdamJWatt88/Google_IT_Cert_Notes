
## Resources
- For more information about access control lists (ACL) in Windows, check out the link [here](https://msdn.microsoft.com/en-us/library/windows/desktop/aa374872(v=vs.85).aspx).


## Notes 

-   **File permissions** are important for **computer security**.
-   Windows uses **access control lists (ACLs)** to assign file and directory **permissions**.
-   **DACLs (discretionary access control lists)** specify who can use a file and what they can do with it.
-   **Each file or folder** has an owner and one or more **DACLs**.
-   Windows, files, and folders can also have **system access control lists or SACLs** assigned to them. SACLs are used to tell Windows that it should use an event log to make a note of every time someone accesses a file or folder.
-   The **Security tab** in Windows Explorer shows the **permissions assigned** to **users** and **groups** for a file or folder.
-   **Permissions include** Read, Read and execute, List folder contents, Write, Modify, and Full control.
	-   **Read** - Let's you see that a file exists and allows you to read its contents. It also lets you read the files and directories in a directory. 
	-  **Read and execute**- Let's you read files and if the file is an executable, you can run the file. Read and Execute includes read, so if you select Read and Execute, read will automatically be selected. 
	-   **List folder contents** - List folder contents is an alias for Read and Execute on a directory. Checking one will check the other. It means that you can read and execute files in that directory. 
	-   **Write** - Lets you make changes to a file. You can have write access to a file without having read permission to that file. The Write permission also lets you create subdirectories and write to files in the directory. 
	-  **Modify** - The Modify permission is an umbrella permission that includes read, execute, and write. 
	-   **Full control** - A user or group with full control can do anything they want to the file. It includes all the permissions of Modify and adds the ability to take ownership of a file and change its ACLs.
-   **icalcs** is a utility used to view and change **ACLs**.
-   The letters in icalcs represent each permission, and some indicate **inheritance**.![[icacls.png]]
-   **Object inherit (OI)** and **container inherit (CI)** mean that new files or objects created inside a folder will inherit the **DACL**.
-   For help on what these letter mean use the `icacls /?` command

#permissions #windows #DACL #ACLS #SACLS #course3-module2 