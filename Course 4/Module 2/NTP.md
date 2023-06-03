-   **Network time protocol (NTP)** is one of the oldest internet protocols used today to **keep clocks synchronized** on machines connected to a network.
-   **NTP is important** because machines need to have **accurate time** across the network for **security services like Kerberos** and **network authentication protocols** to work.
-   An NTP server can be set up using a **local** or **public server**.
-   To **set up a local** NTP server, **NTP server software** can be installed on a **managed server** and **NTP clients** can be installed on machines, which **sync their time** to the NTP server.
-   To use a **public NTP server**, client machines connect to other organizations' servers to get synchronized time.
-   It is a **good practice to run your own NTP server** and have it **point to a public NTP server** instead of connecting all your clients to a public NTP server.
-   NTP is an important network service to integrate into a fleet, whether by running your own NTP server or using a public one.

#network-time-protocol #NTP #course4-module2 