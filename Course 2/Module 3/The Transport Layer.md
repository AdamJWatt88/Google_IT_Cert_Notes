-   **Transport layer** responsible for important functions in computer networking, including:
    
    -   **Multiplexing** and **demultiplexing** traffic
    -   Establishing long-running connections
    -   Ensuring data integrity through error checking and verification
    
-   **Multiplexing** and **demultiplexing** are key functions of the transport layer, which allow nodes on a network to direct traffic toward many different receiving services.![[multiplexing-vs-demultiplexing.png]]
    
    -   Multiplexing directs traffic to specific services running on a networked computer.
    -   Demultiplexing delivers traffic that's all aimed at the same node to the proper receiving service.
    -   **Ports** are used to handle multiplexing and demultiplexing in the transport layer.
    -   A port is a 16-bit number used to direct traffic to specific services running on a networked computer.
-   **Servers** and **clients**:
    
    -   A server or service is a program running on a computer waiting to be asked for data.
    -   A client is another program that is requesting this data.
-   **Ports**:
    
    -   Different network services listen on specific ports for incoming requests.
    -   The same device might be running multiple services that listen on different ports.
    -   Ports are normally denoted with a colon after the IP address.
    -   **Socket address** or **socket number** refers to the *combination* of **IP address** *and* **port number.**
    -   Example: requesting a web page from a web server running on a computer listening on IP 10.1.1.100, the traffic would be directed to port 80 on that computer. The full IP and port would be 10.1.1.100:80.
-   **TCP** vs. **UDP**:
    
    -   **TCP (Transmission Control Protocol)** is a reliable protocol that ensures data integrity through error checking and verification.
    -   **UDP (User Datagram Protocol)** is a faster protocol that does not include these error checking features.
    -   TCP uses a three-way handshake to establish connections between devices.
    -   TCP flags are used in the three-way handshake process to establish connections.
-   **Firewalls**:
    
    -   Firewalls are used to keep networks safe.
    -   They can be hardware or software-based.
    -   Firewalls monitor incoming and outgoing traffic and filter out potentially harmful traffic.

#Transport-layer #Multiplexing #demultiplexing #socket-address #socket-number #tcp #udp #firewalls #course2-module3 