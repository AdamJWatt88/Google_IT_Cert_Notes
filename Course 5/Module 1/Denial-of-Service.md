**Denial-of-Service (DoS) attack:**

-   Aims to prevent legitimate users from accessing a service by overwhelming the network or server.
-   Takes up resources, leaving no room for legitimate users.
-   Example: Website with limited capacity of serving ten users.
    -   Attacker occupies all ten spots, denying service to legitimate users.
-  **Ping of Death (PoD**):
    -   Sends a malformed ping to a computer.
    -   Ping larger than what the internet protocol can handle.
    -   Results in buffer overflow, system crash, and potential execution of malicious code.
-  **Ping flood**:
    -   Sends numerous ping packets (ICMP echo requests) to a system.
    -   Overwhelms the system, causing it to be taken down.
-   **SYN flood**:
    -   Targets TCP connections.
    -   Sends SYN packets to the server but doesn't send ACK messages.
    -   Connection stays open, consuming server resources.
    -   Also known as half-open attacks.
-  **Distributed Denial-of-Service (DDoS) attack:**
    -   Utilizes multiple machines to carry out the attack.
    -   Requires a large volume of systems and often involves botnets.
-   **Example: DDoS attack on DYN (DNS service provider) in October 2016.**
    -   Fake DNS lookup requests and SYN floods overwhelmed DYN's system.
    -   DYN handled DNS for major websites (Reddit, GitHub, Twitter).
    -   Services became inaccessible due to DYN's downtime.

#denial-of-service #DoS-attack #ping-of-death #ping-flood #SYN-flood #distributed-denial-of-service #DDoS-attack #course5-module1 

