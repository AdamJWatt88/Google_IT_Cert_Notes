-   Sometimes you won't be able to resolve or get the IP address of a website name in IT support.
-   **First**, check that your network connection is actually working by **pinging** a website like [www.google.com](http://www.google.com/).
-   If **DNS is an issue**, use `nslookup` to **verify** that the hostname points to a name server.
	`nslookup www.google.com`
 -   `nslookup` gives us the **name server** of a host or **domain name**.
![[nslookup.png]]
-   **Copy** the **IP address** or results and **paste** it into a **web browser** to see if DNS is working.
-   If **DNS settings** aren't working correctly, **check the host file** for incorrect entries.
-   Remove incorrect entries and save the configuration file, then restart the browser.
-   Troubleshoot DNS problems by isolating the problem down until you can get to a root cause.

#dns #host-file #nslookup #course4-module2 