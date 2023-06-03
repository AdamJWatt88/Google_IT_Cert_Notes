1. **Introduction to WPA2 (Wi-Fi Protected Access 2)**

- WPA2 improves upon WPA's security measures.
- It implements **CCMP (Counter Mode CBC-MAC Protocol)** based on the **AES cipher**, replacing the insecure **RC4 cipher**.
- Key derivation process remains the same as WPA, and pre-shared key requirements are unchanged.

2. **Counter Mode CBC-MAC Protocol (CCMP)**

- **CCMP** is a mode of operation for block ciphers used in WPA2.
- **It provides authenticated encryption, ensuring both confidentiality and authentication of data**.
- CCMP uses an "**authenticate then encrypt**" mechanism.
- The **CBC MAC Digest** is computed first, and the resulting authentication code is encrypted with the message using AES in counter mode.
- AES in counter mode converts a block cipher into a stream cipher by using a random seed value and an incremental counter to create a key stream for data encryption.![[CCMP.png]]

3. **Four-Way Handshake Process in WPA2**

- The four-way handshake authenticates clients and generates a temporary encryption key (PTK) for data encryption.
- **AP** confirms the client's correct pairwise master key (PMK) or pre-shared key in a WPA-PSK setup without disclosing the PMK.
- **PTK** is derived from the **PMK**, **AP nonce, client nonce, AP MAC address, and client MAC address.**
- AP and client nonces are random bits of data generated and exchanged.
- PTK generation ensures confidentiality between clients, as it is unique for each client.
- **PTK consists of five individual keys**: two for encryption and confirmation, two for message integrity codes, and one for encrypting data.
- AP transmits the **GroupWise Transient Key (GTK)**, used to encrypt multicast or broadcast traffic, encrypted with the EAPoL encryption key from the PTK.
- GTK is shared among all clients connected to the AP and updated periodically.![[4_way_handshake.png]]

4. **WPA2-Enterprise and WPA2-Personal**

- **WPA2-Enterprise** refers to the implementation of 802.1X authentication in Wi-Fi networks.
- **WPA2-Personal** or **WPA2-PSK** uses a pre-shared key for client authentication.
- AP acts as the authenticator in WPA2-Personal, while the authentication server (backend RADIUS) remains the same.
- PMK is generated using components of the chosen EAP method.

5. **WPS Vulnerabilities**

- **WPS (Wi-Fi Protected Setup**) is a convenience feature for joining a **WPA-PSK-protected network**.
- The four-way authentication handshake in WPA2 is susceptible to offline brute-force attacks.
- An attacker capturing the four-way handshake can guess the pre-shared key or PMK.
- Nonces and MAC addresses from the handshake packets are used to compute PTKs.
- Successful validation of a message authentication code (MIC) within a PTK confirms the correct PMK guess.
- Brute-force or dictionary-based attacks depend on the quality of password guesses and require significant computational power.
- Pre-computed PMKs (rainbow tables) exist for common SSID and password combinations, reducing computational requirements for deriving the PTK.

Note: Despite WPA2 being a robust security protocol, it is important to be aware of the vulnerabilities associated with offline brute-force attacks on the four-way handshake. Employing strong, unique passwords and regularly updating network security measures are crucial to mitigating such risks.

#WPA2 #Wi-Fi-Protected-Access-2 #CCMP #Counter-Mode-CBC-MAC-Protocol #Counter-Mode-CBC-MAC-Protocol #CCMP #Four-Way-Handshake-Process #GroupWise-Transient-Key #GTK #course5-module4 