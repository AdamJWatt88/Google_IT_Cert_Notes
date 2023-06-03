1. Introduction to Network Software Hardening

- Network software hardening complements network hardware hardening in securing networks and their traffic.
- Software solutions like **firewalls**, **proxies**, and **VPNs** play a crucial role in network security.

2. **Firewalls**

- Firewalls regulate traffic flow for an entire network and can be deployed as dedicated network infrastructure devices.
- **Host-based firewalls** run on client systems and provide protection for individual hosts.
- **Both network-based and host-based firewalls are recommended for comprehensive network security**.
- Host-based firewalls are essential for protecting mobile devices and preventing compromise from within the internal network.

3. **VPNs (Virtual Private Networks)**

- VPNs provide secure access to internal resources for mobile or roaming users.
- They are commonly used for secure remote access and linking two networks together.
- **Site-to-site VPNs** connect multiple offices, allowing seamless access to devices and services in either location.
- VPN tunnels encrypt traffic between the offices, ensuring secure communication.
- Remote access VPN services enable individuals to access internal resources while outside the office.

4. **Proxies**

- Proxies protect client devices and their traffic and offer secure remote access without using a VPN.
- Web proxies can be configured to route web traffic through a controlled proxy server for various purposes.
- Web requests can be logged for traffic analysis, forensic investigation, and compliance purposes.
- Proxy servers can block malicious or policy-violating content.![[proxy-server.png]]
- **Reverse proxies** enable secure remote access to web-based services without a VPN.![[reverse-proxy.png]]
- They intercept connection requests from outside the network and relay them to internal services.
- Reverse proxies can enforce additional security measures such as client TLS certificates, username and password authentication, and access control lists (ACLs).
- **Popular proxy solutions** supporting reverse proxy configurations include **HAProxy**, **Nginx**, and **Apache web server**.

Note: As an IT support specialist, you may need to configure and maintain firewalls, VPNs, and proxies to ensure network security and facilitate secure remote access to internal resources.

# Supplementary reading on HAProxy, nginx and Apache HTTP server

We've included the main documentation for each product we mention, as well as a direct link the the documentation that covers reverse proxying specifically.

[HAProxy main documentation](http://www.haproxy.org/#docs "HAProxy main documentation")

[HAProxy reverse proxy documentation](http://cbonte.github.io/haproxy-dconv/1.8/intro.html#3.3.1 "HAProxy reverse proxy documentation")

[nginx main documentation](http://nginx.org/en/docs/ "nginx main documentation")

[nginx reverse proxy documentation](http://nginx.org/en/docs/beginners_guide.html#proxy "nginx reverse proxy documentation")

[Apache HTTP server main documentation](http://httpd.apache.org/docs/ "Apache HTTP server main documentation")

[Apache HTTP server reverse proxy documentation](https://httpd.apache.org/docs/2.4/howto/reverse_proxy.html "Apache HTTP server reverse proxy documentation")

#VPN #proxy #reverse-proxy #firewalls #course5-module4 