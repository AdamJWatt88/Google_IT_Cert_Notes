Lesson Topic: Wireless Security Protocols - WPA and WPS

1. **Introduction to WPA (Wi-Fi Protected Access)**

- WPA was introduced as a replacement for WEP by the Wi-Fi Alliance.
- Designed as a short-term solution compatible with older WEP-enabled hardware through a firmware update, eliminating the need for new Wi-Fi hardware.
- WPA aimed to address the security shortcomings of WEP.

2.**WPA Security Features and TKIP (Temporal Key Integrity Protocol)**

- **TKIP** was the security protocol implemented by WPA to enhance security.
- **TKIP introduced three key features**: 
	- **Secure key derivation**: Improved method of incorporating the IV into the per-packet encryption key. 
	- **Sequence counter**: Prevented replay attacks by rejecting out-of-order packets. 
	- **64-bit MIC (Message Integrity Check)**: Prevented packet forging, tampering, or corruption.
- TKIP used the **RC4 cipher** but addressed the weaknesses of WEP's key generation.![[TKIP.png]]
- Key mixing function was used to generate unique encryption keys per packet.
- **WPA utilized 256-bit long encryption keys**.

3. **Pre-Shared Key (PSK) and Key Derivation**

- Under WPA, the pre-shared key (Wi-Fi password) is used as a factor to derive the encryption key.
- **PSK** is fed into the **PBKDF2 (Password-Based Key Derivation Function 2)** along with the network's SSID as a salt.
- PBKDF2 is run through the HMAC-SHA1 function 4,096 times to generate a unique encryption key.
- **The SSID salt defends against rainbow table attacks**.
- PSK can be entered as a **64-character hexadecimal value** or as an **ASCII passphrase (8-63 characters) for PBKDF2**.

4. **WPS (Wi-Fi Protected Setup)**

- WPS was introduced by the Wi-Fi Alliance in 2006.
- It simplifies the secure joining of wireless clients to a network without directly entering the pre-shared key.
- **WPS** supports various methods for exchanging network details:
	- **PIN entry authentication**: Client or AP generates a PIN for authentication. 
	- **NFC or USB**: Out-of-band exchange of network details. 
	- **Push button authentication:** Button press required on both AP and client for authentication.

5. **Vulnerabilities and Security Implications of WPS**

- The PIN authentication method in WPS has vulnerabilities.
- The PIN consists of eight digits, with the last digit serving as a checksum.
- The PIN authentication occurs in halves, making it easier to guess the correct PIN.
- The first half of the PIN has around 10,000 possibilities, while the second half has only 1,000 possibilities.
- Without rate limiting, an attacker could recover the PIN and pre-shared key in less than four hours.
- The Wi-Fi Alliance introduced a one-minute lockout period after three incorrect PIN attempts.
- If an attacker compromises the network using the PIN attack, they can reuse the PIN to obtain the new password, even if it has been changed.

Note: As an IT support specialist, it is important to be aware of the vulnerabilities associated with WPS and recommend using more secure methods of network authentication, such as WPA2-PSK or WPA3-PSK, to prevent potential security breaches.

#WPA #TKIP #temporal-key-integrity-protocol #pre-shared-key #PSK #WPS #wi-fi-protected-setup #course5-module4 