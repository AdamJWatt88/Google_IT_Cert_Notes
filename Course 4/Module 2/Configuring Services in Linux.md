-   As a **system administrator**, knowing how to query the status, stop and start services is important, but it's also **necessary to configure services** to meet the needs of the organization.
-   For instance, if running a DNS server, the DNS zones to be served must be configured, and for a web server, different sites and web applications need to be enabled.
-   **Specific security and backup policies should also be applied to all services**.
-   While most **services are enabled by default when installed**, not all default values are suitable for everyone, and **configuration files may need to be edited** before the service can go live.
-   In **Windows**, most configuration is **stored in the registry**, which can be modified using graphical wizards or using the `set service` command.
-   In **Linux, configuration files for installed services are located in the /etc directory**, and configuration is typically edited with a text editor.
-   To experiment with a simple ftp server like vsftpd, first install the service using `sudo apt install vsftpd`.
-   To **query the status of the service**, run `service vsftpd status`.
-   To **modify the configuration file** to allow anonymous connections, edit the configuration file located in **/etc/vsftpd.config** and change the "anonymous enable" setting from "No" to "Yes".
-   After making changes to the configuration file, the **service must be reloaded** to re-read the configuration without interrupting ongoing connections. This can be done using the command `sudo service vsftpd reload`.
-   After reloading the service, we can connect again and test if the changes were successful.

#services #configure-services #linux #course4-module2 