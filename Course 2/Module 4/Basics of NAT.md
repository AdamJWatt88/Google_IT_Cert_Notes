-   **Network Address Translation (NAT)** is a technique that translates one IP address into another and is used for security and conserving available IPV4 space.
-   Unlike protocols like **DNS** and **DHCP**, **NAT** is a technique and not a defined standard, which means that it is implemented differently by different operating systems and network hardware vendors.
-   **NAT** is accomplished by allowing a gateway, usually a router or firewall, to rewrite the source IP of an outgoing IP datagram while retaining the original IP to rewrite it into the response.
-   **NAT** provides additional security measures to a network by hiding the IP of a computer from the outside world through IP masquerading.
-   In **IP masquerading**, the router translates the IP addresses of all the computers on a network to its own IP address, making the entire address space of that network protected and invisible to the outside world.
-   **One-to-many NAT** is a common type of NAT used on LANs today, where a single public IP address is used to represent multiple private IP addresses.

#NAT #ip-masquerading #one-to-many-NAT #course2-module4 