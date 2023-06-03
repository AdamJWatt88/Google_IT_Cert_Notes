-   Introduction of improvements in addition to increasing address size.
-   **IPv6 header** is simpler than IPv4 header.
-   IPv6 header contains the **following fields**:
    1.  **Version field**: 4-bit field that defines the IP version in use.
    2.  **Traffic class field**: 8-bit field that defines the type of traffic and allows for different priorities.
    3.  **Flow label field**: 20-bit field used in conjunction with the traffic class field for QoS decisions.
    4.  **Payload length field**: 16-bit field that defines the length of the data payload.
    5.  **Next header field**: unique to IPv6, defines the type of header immediately following this one.
    6.  **Hop limit field**: 8-bit field identical to TTL field in IPv4 header.
    7.  **Source and destination address fields**: each 128 bits.
![[IPv6-header.png]]
-   Optional headers are abstracted from the IPv6 header to reduce the overall size.
-   Optional headers contain a next header field and allow for a chain of headers to be formed.
-   If the next header field specifies another header, it follows after the current header. If not, a **data payload** of the same length as specified in the payload length field follows.

#ipv6 #ipv6-header #course2-module6 