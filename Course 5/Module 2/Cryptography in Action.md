Section: HTTPS and TLS

-   **HTTPS** is the secure version of HTTP (Hypertext Transfer Protocol).
-   **HTTPS** encapsulates **HTTP** traffic over an encrypted secured channel using **SSL** or **TLS**.
-   **SSL 3.0** was deprecated in 2015, and TLS is now the commonly used protocol.
-   **TLS** is a **generic protocol** for secure communications and authentication over a network.
-   **TLS secures web browsing, VoIP calls, email, instant messaging, and Wi-Fi network security**.
-   TLS provides secure communication, authentication of parties, and integrity of communications.
-   TLS handshake is the process of establishing a secure channel.
-   The handshake begins with the client sending a ClientHello message with TLS version, cipher suites, and options.
-   The server responds with a **ServerHello** message, selecting the highest protocol version and cipher suite.
-   The server sends its digital certificate, and the client validates it.
-   The client sends a **ClientKeyExchange** message to establish a shared secret.
-   The client switches to secure communications with a **ChangeCipherSpec** message.
-   An encrypted **Finished** message verifies the handshake's success.
-   The server also sends a **ChangeCipherSpec** and encrypted **Finished** message.
-   Once the handshake is complete, application data can flow securely.

**Section: Forward Secrecy**

-   **Session key** is the shared symmetric encryption key used in TLS sessions.
-   If the private key is compromised, all previously transmitted messages using the derived keys can be decoded.
-   Forward secrecy ensures that even if the private key is compromised, session keys remain secure.

**Section: SSH (Secure Shell)**

-   **SSH** is a secure network protocol for accessing network services over unsecured networks.
-   It is commonly used for remote login to command line-based systems.
-   **SSH** uses encryption to protect user names, passwords, keystrokes, and terminal output.
-   Public key cryptography is used to authenticate the remote machine and allow user authentication.
-   SSH supports various key exchange mechanisms and symmetric encryption ciphers.

**Section: PGP (Pretty Good Privacy)**

-   **PGP** is an encryption application for authentication and privacy.
-   It relies on asymmetric encryption and is commonly used for encrypted email communication.
-   PGP can also encrypt files, documents, and folders, and provide full disk encryption.
-   PGP was developed by Phil Zimmermann in 1991 to facilitate secure communications.
-   PGP faced US export restrictions due to encryption technology regulations.
-   Zimmermann published the source code in a book to challenge restrictions under the First Amendment.
-   PGP is highly secure and has no known cryptographic or computational weaknesses.
-   Law enforcement may resort to legal measures to obtain passwords or keys for encrypted PGP data.

Note: The notes cover the real-world applications of encryption concepts, focusing on HTTPS and TLS, SSH, and PGP. The content explains how these protocols and technologies provide security, authentication, and privacy in various communication scenarios.

# Supplemental Reading for PGP

## PGP was [developed by Phil Zimmermann in 1991](http://www.philzimmermann.com/EN/essays/WhyIWrotePGP.html) and was freely available for anyone to use.

#https #http #TLS #SSL #cryptography #PGP #encryption #course5-module2 