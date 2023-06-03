-   **Managing user accounts** is an **important** task for a **sysadmin** as they control access to IT resources in an organization.
-   **Poorly managed user accounts** can **waste time** and create **risks** for the organization.
-   **User accounts** can be created using the **Active Directory Administrative Center (ADAC)** by **right-clicking on users and selecting user**.
-   Only the fields with asterisks are required, such as the **full name** and **account name (also known as the SAM account name)**.
-   The **SAM** account name is the **username** that is stored in the **security account manager database in Windows**.
-   The **domain** is a part of the **account's full name**, and each user account must have a **unique username within the domain**.
-   A **password must be set**, and the option **"user must change password at next login"** should be checked.
-   **To create multiple user accounts quickly, you can write a script using PowerShell**.
-   **All actions taken in ADAC** are **done** in **PowerShell**, and the **commands** can be **viewed** in the **PowerShell history pane** at the bottom of the console.
-   **Active Directory groups** are used to **grant permissions to roles.**
-   **Groups** can be **created** in **ADAC by right-clicking on the users container** and selecting new group.
-   A **description** of the **group** should be provided, and initial users can be added.
-   PowerShell commands for creating groups include the same settings as those filled in ADAC.

#ADAC #active-directory-administrative-center #powershell #course4-module4 