-   Linux user management access works similarly to Windows, with different user types having different privileges and grouping options.
-   **Standard users**, **administrators**, and **Root User** are the **main user types** in Linux, with the **Root User having all privileges** and being the **super user**.
-   The **sudoers file**, which is **protected** and can only be **read by root**, can be viewed using the **sudo command**.
-   If you don't want to use the sudo command every time, you can use the **su command** to log in as the root user.
	`sudo su -`
- To log out of **root user** use the exit command.9
-  You can log in as root and then run this command, but it can be really dangerous to always be in root. **Since root** has **unrestricted access** on the machine, if you make even one mistake, you could **delete** or **modify** something **important**.
-   Instead of logging in its root tell the shell to run commands using **sudo**
	`sudo cat etc/sudoers`
-   The **/etc/group** file can be used to view who has access to run sudo and to view **memberships for all groups**.
-   Each line in the /etc/group file **represents a different group**, with **four fields** separated by colons: **group name, group password, group ID, and a list of users in the group.**moo
-   The **/etc/passwd** file contains **user information**, with the first field being the user name, the second field being the user password (encrypted and stored in a different file), and the third field being the user ID or UID.
-   Root has a UID of zero.

#root #standard-user #administrator #root-user #course3-module2 