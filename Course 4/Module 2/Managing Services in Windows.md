-   Windows also allows system administrators to manage services on the system.
-   Windows update service is responsible for detecting software updates, downloading and preparing them for installation.
-   To **check the status of running services**, use the `Get-Service` command in **PowerShell** and type in the short name `wuauserv` for the Windows update service.
-   Running `Get-Service wuauserv | format list` provides more information about the service.
-   **Only administrators** can start or stop a service, not regular users.
-   To stop the Windows update service, open an administrative PowerShell and type in `Stop-Service wuauserv`.
-   To start the service again, use the `Start-Service wuauserv` command.
-   The **services management console** in Windows can also be used to manage services.
-   To access it, click on "Start" and search for "Services".
-   Find the Windows update service in the list and right-click to stop or start the service.

#services #manage-services #windows #course4-module2 