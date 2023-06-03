-   Files and folders in Linux have different **permission** sets to **restrict unauthorized** access
-   There are three types of permissions: read, write, and execute
	-  **Read** - this allows someone to read the contents of a file or folder. 
	-  **Write** - this allows someone to write information to a file or folder.
	-  **Execute** - this allows someone to execute a program.
-   The **ls** command with long flags can be used to view the permissions of a file or folder
-   Permissions are represented by **10 bits**: the **first bit** represents the **file type** and the **remaining nine bits** represent the **permissions**
-   Permissions are grouped in **sets of three**: the **first set** is for the **owner**, the **second set** is for the **group**, and the **third set** is for **everyone else**
-   **"r"** stands for **readable**, **"w"** stands for **writable**, and **"x"** stands for **executabl**e
-   A dash **("-")** means the permission is **disabled**, and any other character means the permission is enabled
-   Permissions can be **customized** based on roles such as **owner**, **group**, or **everyone else**
-   The first set of permissions (rwx) refers to the owner's permissions, the second set refers to the group's permissions, and the third set refers to everyone else's permissions![[permissions-linux.png]]
-   The owner, group, and permissions can be seen with the **ls -l** command
-   It might take some time to get used to reading permissions, but it will become easier with practice.

#permissions #linux #read #write #execute #course3-module2 