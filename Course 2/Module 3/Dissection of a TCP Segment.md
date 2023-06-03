-   To troubleshoot network traffic that isn't behaving as expected, you might need to analyze it closely.
-   Just like how an **Ethernet frame** encapsulates an **IP datagram**, an **IP datagram** encapsulates a **TCP segment**.
-   A **TCP segment** is made up of a **TCP header** and a **data section**.
-   The **TCP header** contains many fields with lots of information.![[tcp-header.png]]
-   The source port and the destination port fields are used to direct traffic to the correct service and keep outgoing connections separate.
-   The **destination port** is the port of the service the traffic is intended for
-   A **source port** is a high numbered port chosen from a special section of ports known as ephemeral ports. A **source port** is required to keep lots of outgoing connections separate
-   A source port is needed so that when the web server replies, the computer making the original request can send this data to the program that was actually requesting it. It is in this way that when a web server responds to your request to view a web page, that this response gets received by your web browser and not your word processor.
-   The **sequence number** is a 32-bit number that keeps track of where in a sequence of TCP segments this one is expected to be.
-   The **acknowledgment number** is the number of the next expected segment.
-   The **data offset field** is a four-bit number that communicates how long the TCP header for this segment is.
-   Six bits are reserved for the six **TCP control flags**.
-   The **TCP window** specifies the range of sequence numbers that might be sent before an acknowledgment is required. his is done in order to make sure that all expected data is actually being received, and that the sending device doesn't waste time sending data that isn't being received.
-   The 16-bit checksum is calculated across the entire segment to make sure that no data was lost or corrupted along the way.
-   The urgent pointer field is used in conjunction with one of the TCP control flags to point out particular segments that might be more important than others.
-   The options field is rarely used in the real world but is sometimes used for more complicated flow control protocols.
-   Padding is a sequence of zeros to ensure that the data payload section begins at the expected location.

#ethernet-frame #ip-datagram #tcp-segment #tcp-header #sequence-number #acknowledgment-number #data-offset-field #tcp-control-flags #tcp-window
#course2-module3  