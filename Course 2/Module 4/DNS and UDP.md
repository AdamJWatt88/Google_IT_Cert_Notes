-   **DNS** uses **UDP** instead of **TCP** for transport layer due to several reasons.
-   **UDP** is **connectionless**, so there is no set up or tear down of a connection, which means less traffic needs to be transmitted overall.
-   A single **DNS** request and its response can usually fit inside of a single **UDP datagram**, making it an ideal candidate for a connectionless protocol.
-   DNS can generate a lot of traffic, so using **UDP** reduces overhead.
-   **Port 53** is the port that DNS listens on.
-   **TCP** requires more packets than **UDP** for a **DNS** lookup to take place, which adds up fast.
-   **TCP** is more robust than **UDP**, but for something as simple as **DNS**, **UDP** is sufficient.
-   **DNS** provides error recovery functionality at the application layer by simply repeating a lookup if it doesn't succeed.
-   **DNS** over **TCP** does exist and is used when responses are too large to fit in a single **UDP datagram.**

#tcp #dns #udp #udp-datagram