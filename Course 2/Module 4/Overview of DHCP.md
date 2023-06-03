-   Managing hosts on a network requires specific configurations: **IP address**, **subnet mask**, **primary gateway**, and **name server**
-   Out of these four things, three are likely the same on just about every node on the network, the subnet mask, the primary gateway, and DNS server but the last item, an **IP address needs to be different on every single node on the network**.
-   **DHCP** or **Dynamic Host Configuration Protocol** automates the configuration process of hosts on a network, reducing administrative overhead.
-   **DHCP** is an **application layer protocol** that enables a machine to query a DHCP server and receive all networking configurations in one go.
-   DHCP assigns a range of IP addresses to client devices, ensuring that they obtain an IP address when needed.
-   There are three standard ways that DHCP can operate: **dynamic allocation**, **automatic allocation**, and **fixed allocation**.
	-   **Dynamic allocation** is the most common. With dynamic allocation a range of IP addresses is set aside for client devices and one of these IPs is issued to these devices when they request one
	-  **Automatic allocation** is very similar to dynamic allocation in that a range of IP addresses is set aside for assignment purposes. The main difference here is that the DHCP server is asked to keep track of which IPs it's assigned to certain devices in the past.
	- **Fixed allocation** requires a manually specified list of MAC address and their corresponding IPs
-   DHCP discovery can also configure other things beyond IP address, such as **NTP servers**.

#dhcp #dynamic-allocation #automatic-allocation #fixed-allocation #course2-module4 