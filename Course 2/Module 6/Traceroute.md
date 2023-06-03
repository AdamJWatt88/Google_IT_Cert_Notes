-   **Ping** can help determine if a computer can be reached from another and the quality of the connection
-   However, when communicating across networks, problems may arise from intermediary nodes
-   **Traceroute** can help identify where in the long chain of router hops the problem actually is
-   **Tracerout**e discovers the paths between two nodes and provides information about each hop along the way
	-   Traceroute works by manipulating the **TTL Field** at the **IP Level**; TTL Field is decremented by one by every router that forwards the packet and when it reaches zero, the packet is discarded and an **ICMP time-exceeded message** is sent back to the originating host
-   Traceroute uses the **TTL Field** by setting it to 1 for the first packet, 2 for the second, 3 for the third and so on, ensuring that the first packet sent will be discarded by the first router hop, resulting in an **ICMP time-exceeded message**; the second packet will make it to the second router, the third to the third and so on until the packet reaches its destination
-   For each hop, Traceroute sends three identical packets, and the output of a Traceroute command shows the number of the hop, the round trip time for all three packets, the IP of the device at each hop, and a host name if Traceroute can resolve one
-   Traceroute sends **UDP packets** to very high port numbers on Linux and Mac OS, while on Windows, the command is **tracert** and defaults to using ICMP echo requests; Traceroute has more options than can be specified using command line flags on all platforms
-   Two other tools similar to Traceroute are **mtr** on Linux and Mac OS, which works in real time and continually updates its output with all the current aggregate data about the Traceroute, and **pathping** on Windows, which runs for 50 seconds and then displays the final aggregate data all at once.

#traceroute #ttl-field #icmp-time-exceeded-message #tracert #mtr #pathping 