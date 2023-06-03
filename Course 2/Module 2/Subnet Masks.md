-   **Subnet ids** are used to further divide an IP address to identify individual **subnetworks**.
-   **Subnet ids** are calculated via a **subnet mask**, which is a binary number consisting of two sections.![[subnet-masks-binary.png]]
-   The subnet mask's first section is a string of ones that tells us what part of the IP address is the subnet ID.
-   The subnet mask's second section is a string of zeros that tells us what part of the IP address is the host ID.
-   The size of a subnet is entirely defined by its subnet mask, which specifies the number of available host IDs.
-   A subnet can usually only contain two less than the total number of host IDs available.
-   The subnet mask 255.255.255.0 is commonly used and reserves the last octet for host IDs, which can contain the numbers 1-254. The number 0 is not used, and 255 is reserved for broadcast.
-   A subnet mask can be written in a shorthand way using the number of ones in the mask, such as /27 for a mask with 27 ones.![[subnet-mask-27-shorthand.png]]

#subnet-masks #subnet-id #subnetworks #subnetting #/27 #course2-module2 