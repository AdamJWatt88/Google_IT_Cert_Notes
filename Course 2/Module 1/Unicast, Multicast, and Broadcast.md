-   **Unicast** is a type of transmission that is intended for just one receiving address.
-   Ethernet uses a special bit in the destination MAC address to identify unicast frames.
-   If the least significant bit in the first octet of a destination address is set to zero, it means that ethernet frame is intended for only the destination address.
-   If the least significant bit in the first octet of a destination address is set to one, it means you're dealing with a multicast frame.
-   **Multicast** is a type of transmission where the frame is sent to all devices on the local network segment, but it will be accepted or discarded by each device depending on criteria aside from their own hardware MAC address.
-   Network interfaces can be configured to accept lists of configured multicast addresses for these sorts of communications.
-   **Broadcast** is a type of ethernet transmission that is sent to every single device on a **LAN**.
-   Broadcast is accomplished by using a special destination known as a broadcast address, which is all F's.
-   Ethernet broadcasts are used so that devices can learn more about each other.

#unicast #multicast #broadcast #course2-module1 