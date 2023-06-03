-   Network connectivity issues are common problems in troubleshooting network issues.
-   The inability to establish a connection to a server or website is a typical symptom of network problems.
-   **ICMP (Internet Control Message Protocol)** is a protocol used by routers and remote hosts to communicate issues that occur during transmission back to the origin of the transmission.
-   ICMP packets have a **header** with fields such as **type**, **code**, and **checksum**, followed by a **data section** used to determine which transmission caused the error
	-   **Type field** - The type filed is eight bits long, and specifies what type of message is being delivered. Some examples are destination unreachable or time exceeded
	-   **Code field** - Indicates a more specific reason for the message than just the type. For example, of the destination unreachable type, there are individual codes for things like destination network unreachable, and destination port unreachable.
	-   **Checksum** - 16-bits and works like every other checksum field (REAL helpful)
	-   **Rest of Header** - 32-bit field optionally used by some of the specific types and codes to send more data.
	-  **Data payload for an ICMP packet** - The payload for an ICMP packet exists entirely so that the recipient of the message knows which of their transmissions caused the error being reported. It contains the entire IP header and the first eight bytes of the data payload section of the offending packet.
 ![[icmp-packet.png]]
-   The ping tool allows users to send **ICMP echo requests** to check if a destination is up and running on the network and can communicate.
-   **Ping** is a simple program that exists on most operating systems and allows users to send an **ICMP echo request** to a **destination IP** or **fully qualified domain name**.
	Example to ping Google.com
	`ping google.com`
-   The output of the ping command generally displays the **address sending the ICMP echo reply,** the **round-trip communication time**, **TTL remaining**, and the **size of the ICMP message in bytes**.![[ping-results.png]]
-   Ping also supports various command-line flags that allow users to change its behavior, such as the number of echo requests sent, their size, and the speed at which they are sent.
-   In Linux and macOS, the ping command runs until it is interrupted by the end-user by pressing **Control + C** keys simultaneously, while in Windows, it defaults to sending only four echo requests.

#ping #icmp #icmp-echo-reply #course2-module6