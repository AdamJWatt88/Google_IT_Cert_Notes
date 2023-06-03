-   **Routing tables** are constructed based on the quickest path to destination networks.
-   **Routing protocols** are used by routers to share information with each other.
-   Routing protocols fall into two categories: **interior gateway protocols (IGP)** and **exterior gateway protocols (EGP)**.
-   **IGP** is further split into two categories: **link state routing protocols** and **distance vector protocols**.
-   **IGP** is used by routers to share information within a single **autonomous system**.
-   **Autonomous system** is a collection of networks that fall under the control of a single network operator.
-   **Distance vector protocols** are older and routers using them share a list of distances to networks.
-   With distance vector protocols, routers don't know much about the total state of an autonomous system.
-   **Link state protocols** advertise the state of each router's interfaces and share this information with every other router in the system.
-   Link state protocols require more memory and processing power but provide more accurate and up-to-date information than distance vector protocols.
-   Link state protocols have mostly made distance vector protocols outdated over the years.

#routing-table #routing #interior-gateway-protocols #exterior-gateway-protocols #distance-vector-protocols #link-state-protocols #course2-module2 