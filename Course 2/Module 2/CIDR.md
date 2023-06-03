-   **Address classes** were the first attempt at organizing the global Internet IP space
-   **Subnetting** was introduced to improve organization, but traditional subnetting couldn't keep up with the growing Internet
-   With traditional subnetting and the address classes, the network ID is always either eight bit for class A networks, 16 bit for Class B networks, or 24 bits for class C networks. This means that there might only be 254 class C networks in existence.
-   Classful addressing limits the number of available networks and hosts, which results in a large routing table and network sizing issues
-   **CIDR (classless inter-domain routing)** is a flexible approach to describing blocks of IP addresses that expands on the concept of subnetting by using subnet masks to **demarcate** networks
-   **Demarcation point** describes where one network or system ends and another one begins
-   CIDR abandons the concept of address classes entirely and allows an address to be defined by only two individual IDs, which simplifies routing and allows for more arbitrary network sizes
-   CIDR allows networks themselves to be of different sizes, which reduces the number of entries in a routing table and provides additional available host IDs
-   CIDR uses slash notation (CIDR notation) to indicate the network mask, such as /24 or /23
-   A single slash 23 network has 512-2, or 510 hosts, while two slash 24 networks have a total of 254+254, or 508 hosts.

#CIDR #subnetting #subnetworks #subnet-masks #course2-module2 