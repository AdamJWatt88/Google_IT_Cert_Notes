-   **NAT** at the network layer is straightforward, but at the **transport layer**, several additional techniques come into play.
-   **One-to-many NAT** allows many computers to have their outbound traffic translated via NAT to a single IP, but return traffic can be more complicated.
-   **Port preservation** is a technique where the source port chosen by a client is the same port used by the router to direct traffic back to the right computer.
-   The router stores the source port in a table and uses it to forward traffic back to the correct computer.
-   **Port forwarding** is a technique where specific destination ports can be configured to always be delivered to specific nodes, allowing for complete IP masquerading while still having services that can respond to incoming traffic.
-   Traffic for different services can be aimed at the same external IP and DNS name but delivered to different internal servers due to their different destination ports.

#port-preservation #port-forwarding #one-to-many-NAT #NAT #Transport-layer #course2-module4  