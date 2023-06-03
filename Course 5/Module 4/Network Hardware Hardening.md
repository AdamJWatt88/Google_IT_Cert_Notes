Video Topic: Ways to Implement Network Hardware Hardening for IT Support Specialists

1. **DHCP (Dynamic Host Configuration Protocol)**

- **DHCP** is a protocol used for assigning critical configuration information to devices on a network.
- Attackers target DHCP due to its important role in network communication.
- **Rogue DHCP server attack**: Attackers deploy a malicious DHCP server to distribute DHCP leases with manipulated information.
- Enterprise switches protect against rogue DHCP attacks using DHCP snooping.
- **DHCP snooping** monitors DHCP traffic, tracks IP assignments, and maps them to switch ports.
- DHCP snooping builds a map of assigned IP addresses to physical switch ports, protecting against attacks like IP spoofing and ARP poisoning.
- It also allows designating trusted DHCP servers or trusted uplinked ports for legitimate DHCP responses.

2. **Dynamic ARP Inspection (DAI)**

- **ARP (Address Resolution Protocol)** enables Layer 2 man-in-the-middle attacks due to its unauthenticated nature.
- Attackers can forge **ARP responses (gratuitous ARP responses)** and redirect network traffic.
- **DAI** is a feature on enterprise switches that prevents ARP-based attacks.
- It relies on DHCP snooping to establish a trusted binding of IP addresses to switch ports.
- **DAI** detects forged ARP packets and drops them based on the authoritative IP address assignments stored in the DHCP snooping table.
- DAI enforces rate-limiting of ARP packets per port to prevent ARP scanning.![[dynamic-ARP-inspection.png]]

3. **IP Source Guard (IPSG)**

- **IPSG**, used **in conjunction with DHCP snooping**, prevents IP spoofing attacks.
- IPSG dynamically creates rules for each switch port based on the DHCP snooping table.
- It drops packets that don't match the IP address assigned to the port.

4. **802.1X and EAPoL (Extensible Authentication Protocol over LAN)**

- 802.1X is the IEEE standard for encapsulating EAP traffic over **802 networks.**
- **EAPoL**, also known as **EAP over LAN**, provides authentication for Ethernet, Wi-Fi, and fiber networks.
- EAP supports numerous authentication types (around 100), with **EAP-TLS** being one of the common and secure methods.
- EAP-TLS utilizes **TLS (Transport Layer Security)** for mutual authentication of clients and authenticating servers.
- **EAP-TLS requires client-side certificates**, which can be used in combination with other factors such as usernames, passwords, or one-time passwords.
- The authentication process involves the supplicant (client device), authenticator (switch or access point), and authentication server (RADIUS server).
- The authenticator forwards authentication requests to the authentication server for verification.![[EAPOL.png]]

5. **EAP-TLS Security and PKI (Public Key Infrastructure)**

- **EAP-TLS** leverages the security provided by **TLS** and **PKI**.
- Client certificates are used for authentication, signed by the authenticating CA.
- Proper management of PKI elements is crucial for security, including safeguarding private keys and distributing CA certificates to client devices.
- Binding client-side certificates to client platforms using TPMs (Trusted Platform Modules) enhances security.
- **Combining TPMs with full disk encryption (FDE)** prevents compromise even if a computer is stolen.![[EAPTLS.png]]

6. **Importance for IT Support Specialists**

- IT support specialists benefit from understanding these processes for troubleshooting and evaluating infrastructure security.
- While not required to know every step-by-step detail, awareness of these processes aids in identifying and addressing security issues.

Note: It is recommended to watch the video multiple times for better comprehension and retention of the material.

#DHCP #dynamic-ARP-inspection #DAI #rogue-DHCP-server-attack #network-hardening-hardware #ARP-responses #DHCP-snooping #IP-source-guard #IPSG #course5-module4 