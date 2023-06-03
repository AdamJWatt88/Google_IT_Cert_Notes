-   **IPv4** uses a **32-bit number** to represent the address for a node on a network, which is not enough for the number of Internet-connected devices in the world.
-   IPv6 was developed as a new Internet Protocol because of the issue of running out of IPv4 address space.
-  **IPv6 addresses** are **128 bits** in size, which is a huge number range called an undecillion.
-   IPv6 addresses are usually written out as **eight groups of 16 bits each**, each group made up of **four hexadecimal numbers**.
-  **IPv6** has a notation method to **shorten the address**, which is by removing any leading zeros from a group and replacing consecutive sections containing just zeros with two colons. ![[zero-notation-IPv6.png]]
-   IPv6 has several reserved address ranges besides the one reserved for documentation purposes or the **loopback address**, such as **multi-cast** and **link-local unicast**.
	- **::1** for loopback
	- **FF00::** is used for multi-cast, which is a way of addressing groups of hosts all at once
	- **FE80::** are used for link-local unicast. Link-local unicast addresses allow for local network segment communications and are configured based upon a host's MAC address. The link-local address are used by an IPv6 host to receive their network configuration, which is a lot like how DHCP works
-   The IPv6 address space is so huge that there was never any need to think about splitting it up into address classes like IPv4. The **first 64 bits** of any IPv6 address is the **network ID**, and the **second 64 bits** of any IPv6 address is the **host ID**.![[network-id-host-id-IPv6.png]]

#ipv6 #loopback-address #multicast #link-local-unicast #course2-module6 


