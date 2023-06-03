-   Routing tables are used by routers to determine the next hop for incoming data packets.
-   The earliest routers were just regular computers with two network interfaces and a manually updated routing table.
-   All major operating systems today still have a routing table that they consult before transmitting data.
-   The most basic routing table will have four columns: **Destination network**, **Next hop**, **Total hops**, and **Interface**.![[basic-routing-table.png]]
-   The **Destination network** column contains the definition of the **remote network**, including the **network ID** and the **net mask**.
-   The **Next hop** column contains the IP address of the next router that should receive data intended for the **destination network**.
-   The **Total hops** column keeps track of how far away the destination network currently is and helps routers pick the shortest possible path to ensure timely delivery of data.
-   The **Interface** column tells the router which of its interfaces it should forward traffic matching the destination network out of.
-   Routing tables can vary depending on the make and class of the router, but they all share these basic elements.
-   **Core Internet routers** may have millions of rows in their routing tables, which must be consulted for every single packet that flows through the router on its way to its final destination.

#routers #routing #routing-table #course2-module2 