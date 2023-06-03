-   To **change** your **password** in Linux, run the **"passwd"** command
-   The password is securely **scrambled** and stored in the **/etc/shadow** file
-   The /etc/shadow file can only be read by **root**
-   Even with access, passwords in the file cannot be descrambled
-   To **force a user** to change their password, use the **"-e"** or "expire" flag with the **"passwd**" command
-   Example: "sudo passwd -e username"
-   This immediately expires the user's password and forces them to set a new password upon login

#passwords #linux #course3-module2 