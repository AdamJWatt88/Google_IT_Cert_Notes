-   **DHCP** is an **application layer protocol** that helps configure the **network layer**.
-   **DHCP** relies on the **transport**, **network**, **data link**, and **physical layers** to operate.
-   **DHCP** discovery is the process by which a client attempts to get network configuration information.
-   The **DHCP** discovery process has four steps: **server discovery**, **DHCP offer**, **DHCP request**, and **DHCP acknowledgement**.
-   DHCP listens on **UDP port 67**
-   **DHCP discovery messages** are always sent from **UDP port 68**
-   The client sends a DHCP discover message as a broadcast message to every node on the local area network.
-   The DHCP server examines its own configuration and decides what IP address to offer to the client.
-   The response is sent as a DHCP offer message to the client.
-   The client machine processes the DHCP offer to see what IP is being offered to it.
-   The client responds to the DHCP offer message with a DHCP request message.
-   The DHCP server receives the DHCP request message and responds with a DHCP acknowledgement message.
-   The networking stack on the client computer uses the configuration information presented by the DHCP server to set up its own network layer configuration.
-   The configuration information is known as **DHCP lease** and includes an expiration time.
-   A client can release its lease to the DHCP server when it disconnects from the network.
-   Once a lease has expired, the DHCP client needs to negotiate a new lease by performing the entire **DHCP discovery process** again.

#dhcp #server-discovery #dhcp-offer #dhcp-request #dhcp-acknowledgement #dhcp-discovery-messages #course2-module4 