-   **TCP protocol** establishes connections for sending long chains of segments of data
-   Contrasts with IP and Ethernet protocols which send individual packets of data
-   Understanding TCP is important for troubleshooting network traffic issues
-   TCP uses **six control flags**, which appear in a specific order in the **TCP header**
-   The six TCP control flags are: **URG**, **ACK**, **PSH**, **RST**, **SYN**, **FIN**
-   The **URG flag** is for **urgent data**. A value of one here indicates that the segment is considered urgent and that the urgent pointer field has more data about this. This feature of TCP has never really had widespread adoption and isn't normally seen.
-   The **ACK flag** indicates that the **acknowledgement number field** should be examined if there is a value of one in this field
-   The **PSH flag** is used to **push currently-buffered data** to the application on the receiving end as soon as possible
-   The **RST flag** is used to **reset** a TCP connection when one side can't recover from missing or malformed segments
-   The **SYN flag** is used to **synchronize** the sequence number field when first establishing a TCP connection
-   The **FIN flag** is used to indicate that the transmitting computer has no more data to send and the connection can be closed
-   TCP connection establishment uses a **three-way handshake** involving SYN, SYN/ACK, and ACK flags![[three-way-handshake.png]]
-   The three-way handshake ensures that both devices are speaking the same protocol and can understand each other
-   Once the handshake is complete, the TCP connection is established in **full duplex mode**
-   **Full duplex mode** allows both sides to send and receive data simultaneously
-   TCP connection closure uses a **four-way handshake** involving FIN and ACK flags![[four-way-handshake.png]]
-   Both sides typically send FIN flags to close the connection

	#six-control-flags #URG #ACK #PSH #RST #SYN #FIN #three-way-handshake #four-way-handshake #full-duplex #course2-module3 