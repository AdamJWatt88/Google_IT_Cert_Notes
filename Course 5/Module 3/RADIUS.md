- **RADIUS** is a protocol that provides **AAA (Authentication, Authorization, and Accounting)** services for users on a network.
- It is commonly used to manage access to **internal networks**, **WiFi networks**, **email services**, and **VPN services**.
- Originally designed for remote dial-up users, RADIUS has evolved to support various standard authentication protocols such as **EAP (Extensible Authentication Protocol)**.
- As an IT support specialist, you may not be responsible for configuring the RADIUS server directly, but you may encounter clients that authenticate against a RADIUS backend server.
- Understanding the role of the RADIUS server in the authentication scenario will help you troubleshoot any issues that arise.
- Clients do not interact directly with the RADIUS server. When a client wants to access a protected resource, they present their authentication credentials to a **NAS (Network Access Server)**.
- The **NAS** then relays the credentials to the **RADIUS server for verification.**
- The RADIUS server verifies the credentials using a configured authentication scheme.
- RADIUS servers can store user authentication information in a flat file or connect to external sources such as **SQL databases**, **LDAP, Kerberos**, or **Active Directory**.
- After evaluating the user authentication request, the RADIUS server responds with one of **three messages**:
    - **Access**: The user is granted access to the requested resource.
    - **Reject**: The user's authentication credentials are rejected, denying access to the resource.
    - **Access-Challenge**: The RADIUS server requires additional information or authentication steps from the client before granting access.
    - **Access-Accept**: The user is granted access, but additional authorization checks may be required.
- The RADIUS protocol also supports accounting features to track and record user activity, but it is primarily focused on authentication and authorization.

#RADIUS #network-access-server #NAS #course5-module3 