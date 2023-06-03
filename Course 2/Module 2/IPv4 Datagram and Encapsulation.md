-   **IP datagram** is the name of packets at the network layer under the IP protocol
-   IP datagram consists of two sections: **header** and **payload**
-   IP datagram header contains more data than an ethernet frame header![[ip-datagram-header.png]]
-   The header starts with a 4-bit version field indicating the version of IP being used
-   **IPv4** is the most common version of IP, followed by **IPv6**
-   Header length field is a 4-bit field that declares how long the entire header is (usually 20 bytes)
-   **Service type field** (8 bits) is used to specify details about **quality of service (QoS)** technologies. The important takeaway about **QoS** is that there are services that allow routers to make decisions about which IP datagram maybe more important than others
-   **Total length field** (16 bits) indicates the total length of the IP datagram
-   **Identification field** (16 bits) is used to group messages together and indicate the size of an individual datagram
-   **Flag field** and **fragmentation offset** field are closely related and are used to indicate if a datagram can be fragmented or has already been fragmented
-   Fragmentation is the process of taking a single IP datagram and splitting it up into several smaller datagrams.
-   **Time to live (TTL) field** (8 bits) indicates how many router hops a datagram can traverse before it's thrown away. The recommended standard for a TTL field value is **64**. Every time a datagram reaches a new router, that router deck remains the TTL field by one. Once this value reaches zero, a router knows it doesn't have to forward the datagram any further. The main purpose of this field is to make sure that when there's a miss configuration in routing that causes an endless loop.
-   **Protocol field** (8 bits) contains data about what transport layer protocol is being used (TCP or UDP)
-   **Header checksum field** is a checksum of the contents of the entire IP datagram header
-   **Source** and **destination IP address fields** are each 32 bits long
-   **IP options field** is an optional field used to set special characteristics for datagrams, followed by a padding field
-   **IP datagram** is the payload section of an ethernet frame, and the payload of an IP datagram is the entirety of a TCP or UDP packet
-   The layering of networking is important because each layer is needed for the one above it

#datagram #course2-module2 