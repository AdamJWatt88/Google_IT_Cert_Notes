-   **Authoritative name servers** are responsible for a specific **DNS zone**
-   **DNS zones** are hierarchical and don't overlap
-   **Root name servers** are responsible for the **root zone**, while each TLD name server is responsible for its specific TLD zone
-   Authoritative name servers are responsible for even finer grained zones underneath that
-   The purpose of **DNS zones** is to allow for easier control over multiple levels of a domain
-   Network administrators can split up configurations into multiple zones to ease management
-   Zones are configured through zone files that declare all resource records for a particular zone
-   Zone files contain an **SOA record** that declares the zone and the name server that is authoritative for it, along with **NS records** that indicate other name servers responsible for the zone
-   Multiple physical servers with their own **FQDN**s and IP addresses are often involved in serving DNS traffic
-   Besides **SOA** and **NS records**, zone files contain other resource record types like **A**, **Quad A**, and **CNAME records**, along with configurations such as default **TTL value**s
-   Zones can be configured to go many layers deep, but it's rare to see zones deeper than a few levels
-   Reverse lookup zone files let DNS resolvers ask for an IP and get the associated FQDN returned, and contain mostly pointer resource record declarations (PTR records) that resolve an IP to a name.

#authoritative-name-servers #dns-zone #root-name-servers #soa-record #ns-record #FQDN #course2-module4 