### Introduction to PKI:

-   **PKI** stands for **Public Key Infrastructure**, which is a critical component of securing communications on the Internet.
-   Public key cryptography allows secure data transmission over untrusted channels and verifies the sender's identity using **digital signatures**.
-   PKI is a system that encompasses the **creation**, **storage**, and **distribution of digital certificates**.
-   A **digital certificate** is a file that proves an entity's ownership of a specific public key.
-   The **certificate contains information** about the **public key, the entity it belongs to, and a digital signature** from another party that has verified this information.
-   **If the signature is valid** and the signing entity is trusted, the public key can be trusted for secure communication with the owning entity.

### Components of PKI:

-   **Certificate Authority (CA)**: Responsible for **storing**, **issuing**, and **signing certificates**. It is a **crucial component** of a PKI system.
-  **Registration Authority (RA)**: Verifies the identities of entities requesting certificates to be signed and stored with the CA. This role is often combined with the CA.
-   **Central Repository**: A secure storage and indexing system for keys and certificates.
-   **Certificate Management System**: Facilitates the management of access to certificate storage and issuance of certificates.

### Types of Certificates:

-   **SSL/TLS Server Certificate**: Presented by a web server during the initial setup of an SSL/TLS connection. The client verifies the certificate's subject matches the server's hostname and that it is signed by a trusted CA.
-   **Wildcard Certificate**: Valid for multiple hostnames within a domain, denoted by an asterisk (`*`) replacing the hostname.
-   **Self-Signed Certificate**: Signed by the same entity that issued it. Not trusted unless the key is already trusted.
-  **SSL/TLS Client Certificate**: Optional component used to authenticate clients to servers in SSL/TLS connections. These certificates are not issued by public CAs but by internal CAs managed by the service operator.
-   **Code Signing Certificate**: Used to sign executable programs, allowing users to verify the application's integrity, origin, and authenticity.

### Building Trust in PKI:

-   PKI relies on trust relationships and the establishment of a network or **chain of trust**.
-   The chain of trust starts with the **root certificate authority**, which issues **self-signed certificates** because there is **no higher authority to sign on their behalf**.
-   The **root CA** can use its self-signed certificate and associated private key to sign other public keys and issue certificates, creating a tree structure with the root private key at the top.
-   **If the root CA signs a certificate with the "CA" field set to true**, it designates an intermediate or subordinate CA. This means **the entity can sign other certificates** and carries the same level of trust as the root CA.
-   An **intermediate CA** can further delegate authority by assigning other intermediate CAs, thus extending the chain of trust.
-   **Certificates without authority** as a CA are called end-entity or leaf certificates, **representing the end of the trust chain**.

### Establishing Trust in Root CAs:

-   Trust in root CAs is essential for bootstrapping the chain of trust.
-   Root CA certificates are distributed through alternative channels.
-   **Major operating system vendors include trusted root CA certificates with their OS** and provide programs for their distribution.
-   **Most browsers utilize the OS-provided store of root certificates**.

Note: The lesson provides an overview of PKI, including its components, certificate types, and the establishment of trust relationships. It highlights the importance of root CAs, their self-signed certificates, and the distribution of trust through alternative channels.

#public-key-infrastructure #certificates #course5-module2 