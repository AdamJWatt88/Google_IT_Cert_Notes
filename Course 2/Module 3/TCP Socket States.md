-   A **socket** is an endpoint in a potential TCP connection that requires actual programs to **instantiate** them
-  An **instantiation** is the actual implementation of something defined elsewhere.
-   Contrast to ports which are more of a virtual descriptive thing.
-   **TCP sockets** can exist in various states, and understanding them can help troubleshoot network connectivity issues.
-   Common TCP socket states are:
    -   **LISTEN**: TCP socket is ready and listening for incoming connections **(seen on server-side only)**.
    -   **SYN_SENT**: synchronization request has been sent, but the connection hasn't been established yet **(seen on client-side only)**.
    -   **SYN_RECEIVED**: socket previously in a LISTEN state has received a synchronization request and sent a SYN/ACK back but hasn't received the final ACK from the client yet **(seen on server-side only)**.
    -   **ESTABLISHED**: TCP connection is in working order and both sides are free to send each other data **(seen on both client and server-side)**.
    -   **FIN_WAIT**: FIN has been sent, but the corresponding ACK from the other end hasn't been received yet **(seen on both client and server-side)**.
    -   **CLOSE_WAIT**: connection has been closed at the TCP layer, but the application that opened the socket hasn't released its hold on the socket yet **(seen on both client and server-side).
    -   **CLOSED**: connection has been fully terminated, and no further communication is possible **(seen on both client and server-side)**.
-   There are other TCP socket states that exist, and the names can vary from operating system to operating system.
-   TCP, as a protocol, is universal in how it's used, but socket state descriptions at the operating system level aren't as universal.
-   When troubleshooting issues at the TCP layer, it's essential to check out the exact socket state definitions for the systems you're working with.

#tcp #tcp-socket #LISTEN #SYN-SENT #SYN-RECIEVED #ESTABLISHED #FIN_WAIT #CLOSE_WAIT #CLOSED #course2-module3 