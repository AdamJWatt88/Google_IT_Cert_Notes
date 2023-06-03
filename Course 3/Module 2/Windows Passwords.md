## Resources
More information from Microsoft on passwords [here](https://msdn.microsoft.com/en-us/library/cc875839.aspx)

-   **Passwords** add security to user accounts and machines
-   Passwords ensure that only the user knows the magic secret to access their account
-   When managing other people's accounts, you shouldn't know their password
-   To **reset** a password in **GUI**:
    -   Go to **computer management tool **> **Local Users and Groups**
    -   Right-click on a **username** > **Propertie**s
    -   Check "User must change password at next login"
    -   Apply and hit "Okay"
-   To set a password **manually** in GUI:
    -   Right-click on **username** > **"Set password"**
-   To change a local password in **PowerShell**:
    -   Use the DOS style Net command
    -   The command is **"net user"** followed by the** username** and **password**
    -   Use an **asterisk** instead of writing the password on the command line
    -   Net will pause and ask you to enter your password
-   It's best not to log passwords in a log file
-   To **force a user** to change their default password on their **next login**:
    -   Use the **"/logonpasswordchg:yes"** parameter with the Net command
    -   Example: "net user victor/logonpasswordchg:yes"

#passwords #windows 