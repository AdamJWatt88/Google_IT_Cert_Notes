-   Computers can be joined or bound to Active Directory (AD).
-   **Joining a computer to AD means that**:
    -   AD knows about the computer and has provisioned a computer account for it.
    -   The computer knows about the AD domain and authenticates with it.
-   **Workgroup** computers are **not joined to a domain** and are **not centrally administered**.
-   **To join a computer to a domain**:
    -   Click **"Computer**" then **"System properties."**
    -   Click **"Change settings"** then **"Change."**
    -   Select **"Domain"** and enter the **domain name**.
    -   Enter the **username** and **password** to authorize the computer to be joined to the domain.
-   The **domain controller** creates a computer account in the domain for the joined computer, and the computer reconfigures itself to use AD authentication service. A reboot is required.
-   **Group policy** can be used to manage the joined computer.
-   Computers can also be joined to the domain from **PowerShell** using the `Add-Computer` cmdlet.
	`Add-Computer -DomainName 'example.com' -Server 'dc1'`
-   Active Directory has different functional levels that describe the features it supports.
-   **To find the functional level of a domain**:
    -   Check the properties of the domain in the Active Directory Administrative Center.
    -   Use PowerShell and the `Get-AdForest` and `Get-AdDomain` cmdlets to find the forest mode and domain mode properties.
-   Knowing the functional level of a domain helps in finding out the AD features it supports.

#active-directory-domain #domain-controller #powershell #course4-module4 