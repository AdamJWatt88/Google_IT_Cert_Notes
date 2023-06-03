-   **Ethernet frames** are data packets at the **Ethernet level**
-   Ethernet frames are highly structured collections of information presented in a specific order, with almost all sections being mandatory.![[ethernet-frame.png]]
-   The first part of an Ethernet frame is the preamble, which is eight bytes or 64 bits long.
-   The preamble contains a series of alternating ones and zeros that act partially as a buffer between frames and can also be used to synchronize internal clocks.
-   The **start frame delimiter** (SFD) signals to a receiving device that the preamble is over and that the actual frame contents will now follow.
-   Immediately following the SFD is the destination MAC address, which is the hardware address of the intended recipient.
-   Following the destination MAC address is the source MAC address or where the frame originated from.
-   The **Ether-type field**, which is 16 bits long, is used to describe the protocol of the contents of the frame.
-   Instead of the Ether-type field, you can also find a **VLAN header,** which indicates that the frame itself is a **VLAN frame**.
-   The data payload of a traditional Ethernet frame can be anywhere from 46-1500 bytes long and contains all of the data from higher layers, such as the IP, transport, and application layers that are actually being transmitted.
-   Following the data payload is the frame check sequence, which is a four-byte or 32-bit number that represents a checksum value for the entire frame.
-   The frame check sequence is calculated by performing a **cyclical redundancy check**against the frame, which is an important concept for data integrity.
-   The receiving network interface uses the checksum value to infer if it received uncorrupted data.
-   If the checksum computed by the receiving end doesn't match the checksum in the frame check sequence field, the data is thrown out.
-   Ethernet itself only reports on data integrity, it doesn't perform data recovery.

#ethernet-frame #course2-module1 