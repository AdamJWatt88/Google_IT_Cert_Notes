- **Multi-factor authentication (MFA)** involves using multiple pieces of information or objects to authenticate users.
- **MFA factors** can be categorized into **three types**: something you know, something you have, and something you are.
- **Something you know** refers to information like passwords or PINs.
- **Something you have** involves physical tokens, such as ATM or bank cards.
- **Something you are** relates to biometric data, like fingerprints or iris scans.
- The purpose of MFA is to make it difficult for attackers to steal or clone multiple authentication factors.
- Using multiple passwords alone does not significantly enhance security, as passwords are vulnerable to phishing and keylogging attacks.
- Combining a password with a physical token significantly improves security. Even if the password is compromised, the attacker would still need the physical token to access the account.
- **Physical tokens** can take various forms, including USB devices, standalone token generators, or traditional keys.
- A common type of physical token is a **time-based token (TOTP)**, which displays a rotating one-time password (OTP). The **RSA SecureID token** is an example of such a token.
- Time-based tokens require synchronization between the token and the authentication server, often achieved using **Network Time Protocol (NTP)**.
- An attacker would need to steal the physical token or clone it by obtaining the secret seed value.
- Counter-based tokens increment a secret counter value each time an OTP is generated. The counter value is also incremented on the server upon successful authentication, providing additional security.
- Token generators can be physical devices or smartphone apps that perform the same functionality.
- SMS delivery of one-time password tokens is another common method but has security concerns. SMS is not encrypted, and interception by attackers is possible.
- There have been cases of attackers stealing SMS-based multi-factor codes by impersonating the owner and redirecting calls and messages to their own device.
- The convenience trade-off of physical tokens is the need to carry an additional device for authentication. Loss, damage, battery issues, and synchronization problems may occur.
- Using an app on a smartphone mitigates some issues but still requires additional support and can be inconvenient.
- Generated one-time passwords are susceptible to phishing attacks, where users are tricked into entering their credentials and OTPs on fake authentication pages.
- Phishing emails claiming compromised accounts are a common tactic used by attackers to deceive users and gain access to their accounts.

Note: These notes provide a detailed summary of the content, capturing the key points and concepts discussed in the module.

#multifactor-authentication #MFA #physical-tokens #time-based-tokens #RSA-SecureID #course5-module3 