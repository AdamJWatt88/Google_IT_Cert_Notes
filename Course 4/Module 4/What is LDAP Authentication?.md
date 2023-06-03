-   **LDAP** stands for **Lightweight Directory Access Protocol**, used to **access information in directory services over a network**.
-   **Two popular** directory services that use **LDAP** are **Active Directory and OpenLDAP.**
-   **Different operations** that can be performed using **LDAP** include **adding, deleting, and modifying entries** in the **directory server database**.
-   An **LDAP** **entry** consists of a **unique entry name (distinguished name)** and **attributes/values associated with it**.
-   Authentication levels can be used to restrict access to certain directories, similar to public or private phone directories.
-   **Bind** operation is used to authenticate clients to the directory server.
-   There are **three common ways** to **authenticate**: **anonymous**, **simple**, and **SASL (Simple Authentication and Security Layer)**.
-   **Anonymous binding** allows **anyone** to **access the directory**, while **simple authentication requires** the **entry name** and **password**, sent in plain text.
-   **SASL** authentication is **commonly** used and can employ **security protocols** like **TLS** and **Kerberos**.
-   **Kerberos** is a **network authentication protocol** used to **authenticate** user **identity** and **secure** the transfer of **user credentials**.
-   Once the client is authenticated, they are authorized to use the access levels they have.

# Supplemental Reading for Kerberos

- For more information on **Kerberos reading** check out the link [here](https://technet.microsoft.com/en-us/library/cc780469(v=ws.10).aspx).

#LDAP #active-directory #openLDAP #Kerberos #course4-module4 