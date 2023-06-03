-   Before DNS, language-based system needed to refer to network devices.
-   Humans remember descriptive words better than numbers, but computers communicate using numbers.
-   **Numbered network addresses** were correlated with words through **hosts files**.
-   **Hosts files** are **flat files** that contain network address and corresponding host name.
-   Hosts files are evaluated by the networking stack of the operating system itself.
-   Presence of an entry in hosts file translates to anywhere a networking address is referred to.
-   Hosts files contain a special IP address called **loopback address**.
-   **Loopback address always points to itself** and is a way of sending network traffic to yourself.
-   Loopback IP for IPv4 is **127.0.0.1** and it's configured on every modern OS through an entry in a host file.
-   Almost every host file contains a line that reads **127.0.0.1 localhost**, most likely followed by **::1 localhost for IPv6**.
-   Host files still exist on modern operating systems and are important to know about, though not used much anymore due to DNS.
-   Some software may require specific entries in the host file to operate properly.
-   Host files can be helpful for troubleshooting purposes in IT support.
-   Host files are examined before DNS resolution attempt occurs on just about every major operating system.
-   Host files can be used to force a computer to think a certain domain name always points at a specific IP.

#numbered-network-addresses #host-file #loopback-address #localhost #course2-module6 