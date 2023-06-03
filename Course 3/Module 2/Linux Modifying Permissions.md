-   In Linux, **change permissions** using **chmod** or change mode command.
-   Pick permission set to change: **owner (u)**, **group (g)**, or **other users (o)**.
-   Use **+** or **-** to **add** or **remove** permissions, respectively.**
-   Examples:
    -   **chmod u+x** my_cool_file (give executable permission to owner)
    -   **chmod u-x** my_cool_file (remove permission from owner)
    -   **chmod u+r+x** my_cool_file (add read and execute permissions to owner)
    -   **chmod ugo+r** my_cool_file (add read permission to owner, group, and all other users and groups)
-   **Symbolic format** uses **r, w, x**, and **ugo** to denote permissions and users in chmod.
-  **Numeric format** is faster: **4 for read**, **2 for write**, **1 for execute**. Add numbers to set permissions.
-   Example: chmod 754 my_cool_file (owner has read, write, and execute permissions; group has read and execute permissions; all other users have read permission)
-   Can **change owner** with **chown** command and **group** with **chgrp** command.
	```
	sudo chown test_user test-file.txt
	sudo chgrp group_name test-file.txt
	```
-   Permissions are important for computer security. Practice changing permissions on files.

#linux #modifying-permissions 