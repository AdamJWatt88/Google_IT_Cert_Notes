-   **OpenLDAP is a free and open source directory service similar to Active Directory**
-   It uses **LDAP notation or LDIF** to add, remove, and authenticate users, groups, and computers in a directory service
-   It can be used on **any operating system** including **Linux**, **macOS**, and **Microsoft Windows**
-   **Recommended to use Active Directory on Windows** as it's Microsoft's proprietary software for directory services
-   Ways to **interact with OpenLDAP**: **command line interface** and **phpLDAP** admin tool
-   To **install OpenLDAP on Linux**, use the command: `sudo apt-get install slapd ldap-utils`
-   After installing, it prompts to enter an administrator password for LDAP
-   To reconfigure OpenLDAP package, run the command: `sudo dpkg-reconfigure slapd`
-   It asks a series of questions to fine-tune the OpenLDAP settings, including:
    -   Omitting OpenLDAP server configuration (choose no)
    -   DNS domain name (organization domain, e.g., example.com)
    -   Organization name (e.g., example)
    -   Administrator password
    -   Database (choose MDB)
    -   Removing the database when slapd purge (choose no)
    -   Allowing LDAP Version 2 protocol (choose no)

# Supplemental Reading for OpenLDAP

For more information about installing and configuring **OpenLDAP** and phpLDAPAdmin on Ubuntu 16.04, click [here](https://www.digitalocean.com/community/tutorials/how-to-install-and-configure-openldap-and-phpldapadmin-on-ubuntu-16-04) or check out this article on [openldap.org](https://www.openldap.org/doc/admin24/slapdconf2.html).

#LDAP #openLDAP #linux #course4-module4 