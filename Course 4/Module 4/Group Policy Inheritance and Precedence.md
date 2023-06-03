-   Creating specific GPOs to address specific needs can result in a lot of policies linked at many levels of an active directory hierarchy, especially for GPOs that control security settings.
-   To ensure a **secure IT infrastructure**, a **restrictive GPO** with **secure conservative security policies** can be created and **linked** to the **whole domain** as a **default policy.** However, some users may not be able to perform certain tasks with these policies in place.
-   To **allow exceptions**, GPOs can be created that relax some of the security settings or policies in the OUs that contain those users or computers.
-   If **contradictory GPOs** are applied to the same computer, they are applied in a **specific order based** on a set of **precedence rules**.
-   GPOs linked to the **least specific** or **largest container are applied first**, and GPOs linked to the **most specific** or **smallest container are applied last**.
-   **If more than one policy** tries to set the same policy or preference, then **the most specific policy wins**.
-  **GPO link order determines** which GPO takes precedence, with the **highest number being the lowest ranked GPO**.
-   The **resultant set of policy (RSOP)** is the **combination of all group policies** applied to a specific machine, taking into account precedence rules.
-   **RSOP** reports can be generated to troubleshoot group policy issues.
-   The **Group Policy Results Wizard** can be used to generate a resultant set of policy report for a specific computer and user.

#group-policy-inheritance #GPO #group-policy-objects #resultant-set-of-policy #RSOP #course4-module4 