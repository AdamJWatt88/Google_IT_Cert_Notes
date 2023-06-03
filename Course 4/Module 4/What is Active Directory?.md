-   **Active Directory (AD**) is the **native** directory service for **Microsoft Windows** used to **centrally manage networks** of computers since Windows Server 2000.
-   **AD** works **similarly** to **OpenLDAP** and can **inter-operate** with **Linux**, **OSX** and other **non-Windows hosts** using that protocol.
-   **AD** does more than just provide directory services and centralized authentication. It is **also** the **central repository of group policy objects (GPOs)** which are ways to **manage** the **configuration of Windows machines**.
-   AD **administration** **relies** on a **suite** of **tools** and **utilities** **including** the **Active Directory Administrative Center (ADAC)** which is used for everyday tasks.
-   **Directory services** are **hierarchical**, and **everything in AD is an object**. **Some** **objects** are **containers** which can **contain other objects**, and there are **two types of containers**: **ordinary containers** and **organizational units (OU)**. **OUs** are used for **organizing objects** within a **centralized management system**.
-   **Common parts of AD include the domain**, which has a short name and a **DNS name**; **computers**, which is where **new AD computer accounts are created;** **domain controllers**, which are **created by default**; and **users**, which is where **new AD users** and **groups** are **created** by default.
-   **Domain controllers** host a replica of the **Active Directory database** and **group policy objects**. They also serve as **DNS service** to provide **name resolution** and **service discovery** to clients and provide **central authenticatio**n through a network security protocol called **Kerberos**.
-   Most **domain controllers** in Active Directory network are **read-write replicas**, meaning that **each has a complete copy of the database** and **can make changes to it**. **Replication** is quick, and the **last change wins in almost all cases.** **Some changes** to the AD database can only be safely made by **one DC at a time**.
-   Joining a computer to Active Directory means that AD knows about the computer and has provisioned a computer account for it. The computer also knows about the Active Directory domain and can authenticate with it.

# Supplemental Reading for Active Directory

- For more information about **Active Directory**, check out the link [here](https://technet.microsoft.com/en-us/library/cc961936.aspx).

#active-directory #active-directory-administrative-center #ADAC #directory-services #domain-controller #group-policy-objects #GPO #ordinary-container #organizational-unit #course4-module4 