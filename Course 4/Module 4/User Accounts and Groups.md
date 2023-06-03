-   There are **two mandatory settings** in the **new group window** in Active Directory: **group type** and **group scope**.
    
-   **Group type**: There are **two categories** of groups in Active Directory: **security group** and **distribution group**. 
	- **Security groups** are **used to grant or deny access to IT resources,** and they can **contain user accounts, computer accounts, or other security groups**. **Default groups** such as **Domain Users** and **Domain Admins** are **security groups**. 
	- **Distribution groups**, on the other hand, are **only designed to group accounts and contacts for email communication** and cannot be used for assigning permission to resources.
-   **Group scope**: Group scope is about the way **group definitions are replicated across domains in Active Directory**. There are **three types of group scopes**: **domain local, global, and universal**.
    
    -   **Domain local groups** are used to assign permission to a resource, such as a domain local group that has read access to a network share called Research Share Readers and another with write access called Research Share Writers.
        
    -   **Global groups** are used to group accounts into a role, such as researchers group.
        
    -   **Universal groups** are used to group global roles in a forest. In a multidomain forest, global groups in each domain are members of the universal group. Universal groups are replicated to all domains in a forest.
        
-   **Group membership**: Users can be added to a group using ADAC (Active Directory Administrative Center) or PowerShell commands that add or remove members from the group.
    
-   **Parent groups**: Parent groups can be created for a department, and then individual groups such as researchers can be added as members

# Supplemental Reading for Group Security Principles

- For more information on **Group Scope** check out the link [here](https://technet.microsoft.com/en-us/library/cc755692(v=ws.10).aspx) and for **Security Principles** click [here](https://technet.microsoft.com/en-us/library/cc780957%28v=ws.10%29.aspx?f=255&MSPPError=-2147217396).

#active-directory-groups #active-directory-users #active-directory-group-scope #course4-module4 