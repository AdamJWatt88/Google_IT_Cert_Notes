-   Managing Active Directory is a huge topic that some system administrators dedicate all their time to.
-   When an **AD domain is first set up**, it includes a **default user account (Administrator)** and **several default user groups**.
-   The most **important groups** to know are:
    -   **Domain Admins**: administrators of the AD domain who can make any changes they want to the domain and become local administrators of all machines joined to the domain.
    -   **Enterprise Admins**: administrators of the AD domain who can make changes that affect other domains in a multi-domain forest.
    -   **Domain Users**: a group that contains every user account in the domain and can be used to grant access to network resources for everyone in the domain.
    -   **Domain Computers**: contains all computers joined to the domain except domain controllers.
    -   **Domain Controllers**: contains all domain controllers in the domain.
-   As a **systems administrator** or **IT support specialist**, you might also be a **domain** or **enterprise admin**, but you **should never use these accounts as your day-to-day user account** because it's **too easy** to make a **mistake** that **affects** the **entire organization**.
-   Your **normal user account** should have **restricted permissions** to only the **resources** you **need access to**.
-   **Delegation** can be used to give **specific accounts permission** to perform **administrative** **tasks** without giving them broad access to make changes in AD.
-   **ACLs (access control lists**) can be set up on **AD objects** to give accounts permission to perform specific tasks.

#active-directory #active-directory-domain #active-directory-administrator #course4-module4 