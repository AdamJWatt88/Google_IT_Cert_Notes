-   Wireless networking is becoming increasingly popular with the rise of portable computing devices like laptops, tablets, and smartphones.
-   **IEEE 802.11** standards define the most common specifications for wireless communication, which is known as Wi-Fi.
-   Wireless networking devices communicate through radio waves and operate at different frequency bands, such as **2.4GHz** and **5GHz**.
-   There are several **802.11 specifications**, including **802.11b**, **802.11a**, **802.11g**, **802.11n**, and **802.11ac**, each with some improvements over the previous version.
-   The **802.11 protocol** defines how wireless networking operates at both the **physical and data link layers**.
-   An **802.11 frame** contains **several fields**, including a **frame control field, duration field, four address fields, sequence control field, data payload section, and frame check sequence field.**![[802.11-frame.png]]
	-   **Frame control field** - This field is 16 bits long and contains a number of sub-fields that are used to describe how the frame itself should be processed. This includes things like what version of the 802.11 was used.
	-   **Duration field** - It specifies how long the total frame is. The receiver knows how long it should expect to have to listen to the transmission.
	-   **Four access fields** - Are used to indicate which wireless access point should process the frame, and they include the source address, intended destination address, receiver address, and transmitter address. 
	-  **Sequence control field** - The sequence control field is 16 bits long and mainly contains a sequence number used to keep track of ordering the frames after this is the data payload section, which has all of the data of the protocols further up the stack
	-  **Data payload** - Has all of the data of the protocols further up the stack
	-   **Frame check sequence (FCS)** - This field contains a checksum used for a cyclical redundancy check, just like how Ethernet does it.

-   The **four address fields** are used to indicate which wireless access point should process the frame, and they include the **source address, intended destination address, receiver address, and transmitter address.**![[802.11-frame-addresses.png]]
-   The wireless access point is a device that bridges the wireless and wired portions of a network, and multiple access points can be used to cover a large area.
-   The association between the wireless device and access point is important for transmitting and receiving data on the wireless network.

#IEEE #course2-module5 