-  **Common issues: user unable to log in or authenticate to the domain.**
-   **Reasons for failure**: password entered incorrectly, account locked out, network connectivity issue, DNS misconfiguration, clock synchronization issue.
-   Start with the **simplest solution first** - network connectivity issue could be the cause.
-   **DNS is critical for finding domain controllers; SRV records must be present for the domain.**![[SRV_records.png]]
-   Use `Resolve-DNSName -Type SRV` to check for SRV records in PowerShell.
	`Resolve-DNSName -Type SRV -Name _ldap._tcp.dc._msdcs.example.com`
-   DNS servers hosting Active Directory domain records should be known and documented.
-   Local authentication may continue to work for a while even if the network is disconnected.
-   **Kerberos authentication protocol used by AD is sensitive to time differences**; UTC time must be synchronized within five minutes.
-   **Domain computers usually synchronize time with domain controllers** but can fail if disconnected from the network for too long or if the time is changed by software or a local administrator.
-   Use `w32tm/rsync` command to manually force domain computer to resync with a domain controller.

#group-policy-objects #Kerberos #troubleshooting #course4-module4 