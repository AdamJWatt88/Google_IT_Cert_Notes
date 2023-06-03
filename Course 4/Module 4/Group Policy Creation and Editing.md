-   The **Group Policy Management Console** or **GPMC** is the primary tool used to create and view **Group Policy Objects (GPOs)**. It can be accessed through the **Tools menu of Server Manager** or by running `gpmc.msc` from the command line.
-   **GPMC's GUI** has **several containers**: Active Directory (AD) containers, such as the Group Policy Objects container that holds all defined GPOs in the domain, and management interfaces specific to GPMC.
-   The **WMI filters** container uses **Windows Management Instrumentation** to decide if a GPO should apply to a specific computer, while the **Group Policy results container is used for troubleshooting**, and the **Group Policy modeling container is used for predicting** which GPOs will apply to a computer or user.
-   **User** and **computer** containers **are not Organizational Units (OUs)** and can only be targeted with GPOs linked to domains and sites, so it is recommended to organize user and computer accounts into OUs to target them with specific GPOs.
-   The **Default Domain Policy** and **Default Domain Controller Policy** are two GPOs that are **automatically created in a new Active Directory domain**. The former is a default GPO linked to the domain and applies to all computers and users, while the latter applies to domain controllers.
-   **GPOs contain two sections**: **computer configuration** and **user configuration**, each with policies and preferences that are divided into hierarchal trees.
-   There are **thousands of settings** that can be controlled with GPOs, and it may take some research to find the right setting to make a specific change. The **Microsoft Group Policy** settings reference is a useful resource for finding GPO policies and preferences.
-   **It is recommended to make a backup of a GPO before making changes to it**. The GPO Editor can be used to change settings, but the settings report in GPMC provides an overview of the configuration of the GPO.

#group-policy-objects #GPO  #group-policy-management-console #GPMC #course4-module4 