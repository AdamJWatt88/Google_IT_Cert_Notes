-   Directory services are databases used to store information about objects in a network
-   **Group Policy Object (GPO)** is an object type in **Active Directory (AD)** that contains **policies** and **preferences** for a group of objects in the directory
-   **GPOs** can be used to **standardize user preferences** for different teams and make it more manageable to configure
-   GPOs can be **linked to domains, sites, or Organizational Units (OUs)** and applied to all the objects under them
-   **Group policies** can be made more selective using tools like security filtering and **WMI filters**
-   **GPOs can contain computer configuration, user configuration, or both**, and are applied at different times
-   **Policies** are **settings** that are **reapplied every few minutes** and are not meant to be changed even by **local administrators**
-   **Preferences** are meant to be a template for settings, but can be changed by users without being overwritten
-   **Domain joined computers** and users get GPOs when they sign into the domain by contacting a domain controller and downloading them from a **special folder called Sysvol**
-  The **Windows registry** is a hierarchical database of settings that Windows, and many Windows applications use for storing configuration data.
-   **GPOs make changes to the Windows registry**, a hierarchical database of settings used for configuration by Windows and Windows applications
-   **Group policy management is a huge topic**, and this lesson covers only the basics of it.

#GPO #group-policy-objects #active-directory #windows-registry #course4-module4 