
## Resources
-   RFCs belong to IETF [Internet Engineering Task Force](https://www.ietf.org/), an open community charged with developing and maintaining the standards required for the Internet to continue to operate.
-   large collections of RFCs [here](https://www.ietf.org/standards/rfcs/).

## Notes
-   In 1996, it became clear that the IPv4 standard with 32-bit numbers cannot accommodate the growing number of devices and people on the internet.
-   **RFC 1918** was published to define non-routable address space, which cannot be routed to by core routers, and can only be used for communication within a network.
-   Non-routable address space allows for nodes on a network to communicate with each other, but no gateway router will attempt to forward traffic to this type of network.
-   **NAT (network address translation)** technology allows computers on non-routable address space to communicate with other devices on the internet.
-   RFC 1918 defined three ranges of non-routable address space: **10.0.0.0/8**, **172.16.0.0/12**, and **192.168.0.0/16**.
-   These ranges are free for anyone to use for their internal networks, but interior gateway protocols will route these address spaces, whereas exterior gateway protocols will not.

#RFC-1918 #nat #network-address-translation #course2-module2 