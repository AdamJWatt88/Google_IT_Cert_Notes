-   IP addresses consist of a **network ID** and a **host ID**![[ip-network-id-host-id.png]]
-   IBM owns all IP addresses with a 9 as the value of the first octet in the IP address
-   The address class system divides the global IP address space into three primary types: **Class A**, **Class B**, and **Class C**
-   **Class A** addresses have a first octet for the **network ID** and the last three for the **host ID**; **Class B** addresses have the first two octets for the network ID and the second two for the host ID; **Class C** addresses have the first three octets for the network ID and the last for the host ID
-   Each address class represents a network of vastly different size
-   The first bit of an IP address determines its address class: 0 for Class A, 10 for Class B, and 110 for Class C![[ipv4-address-classes.png]]
-   The possible values for the first octet of an IP address are 0-127 for Class A, 128-191 for Class B, and 192-223 for Class C
-   **Class D** addresses begin with the bits 1110 and are used for multicasting, with decimal values between 224 and 239
-   **Class E** addresses are unassigned and only used for testing purposes
-   The address class system has been largely replaced by **CIDR**, but it's still important to understand.

#ipv4-address-classes #classA #classB #classC #classD #classE  #network-id #host-id #course2-module2 