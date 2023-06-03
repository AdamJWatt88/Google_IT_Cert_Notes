-   `dnsmasq` can be used as a **DHCP server**.
-   **DHCP server** is usually set up on a machine with a **static IP address** connected to a **physical network with multiple machines**.
-   In this example, simulation is done on one machine with two interfaces, `eth_srv` and `eth_cli`.
-   `eth_srv` is configured to be the **DHCP server's interface with the IP address 192.168.1.1/24**.
-   `eth_cli` is the **client interface** without any IP address configured yet.
-   To use dnsmasq as DHCP server, additional configuration is needed in the **dhcp.config file**, including the **interface, domain, DHCP options, and DHCP range**.
-  **DHCP range is the range of IP addresses that the DHCP server can handle**.
-   Lease time specifies how long the assigned IP address is reserved for the client.
![[configure-dhcp-with-dnsmasq.png]]
-   Start `dnsmasq` with the configuration file using the command `sudo dnsmasq -d -q -c dhcp.config`.
-   Use DHCP client on the eth_cli interface to acquire an IP address.
-   Verify the eth_cli interface has acquired an IP address using the `IP address show eth_cli` command.
-   `dnsmasq` will show the **hostname** of the machine with the assigned IP address.
-   `dnsmasq` also has **DNS capabilities** and can act as a **DNS server**.
-   Test setup on a separate network from the production network to avoid affecting the production network.

#dnsmasq #dns #dns-servers #dhcp-server #course4-module2 