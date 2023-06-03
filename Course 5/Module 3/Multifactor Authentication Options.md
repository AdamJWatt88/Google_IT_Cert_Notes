- **Biometric authentication** uses unique physiological characteristics of individuals to verify their identity.
- Popular biometric features include **fingerprints, iris scans, facial recognition, gate detection, and voice**.
- Biometric authentication has gained popularity, especially in mobile devices, such as fingerprint scanners used to unlock phones.
- **Biometric data should never be stored directly**, just like passwords. Instead, it should be run through a **hashing algorithm**, and the resulting hash is stored.
- Biometric data has privacy implications, as it is inherently part of an individual's identity. Stolen or leaked biometric data is difficult to change, unlike passwords.
- Biometric authentication is more reliable for identifying individuals since biometric features are typically not shareable.
- Some biometric systems, like fingerprint-based attendance recording in schools, can be tricked by creating fake fingerprints using substances like glue.
- Other biometric systems include iris scans, facial recognition (e.g., Windows Hello for Windows 10), and voice recognition.
- **Universal Second Factor (U2F)** is an evolution of physical tokens and a standard developed by Google, Yubico, and NXP Semiconductors.
- **U2F tokens**, known as security keys, are small embedded crypto processors with secure storage of asymmetric keys and additional slots for embedded code.
- Security keys provide a more secure and convenient second factor authentication solution compared to one-time passwords (OTP).
- During registration, the security key generates a private-public key pair unique to the site and submits the public key for registration.
- Security keys generate unique key pairs for each site to prevent cross-referencing and maintain privacy.
- During authentication, the user enters their username and password, followed by physically tapping the security key to ensure user presence.
- The security key unlocks the private keys stored within it for authentication.
- The authentication process involves challenge-response, where the site sends a randomized challenge to the client.
- The client signs the challenge using the private key and sends the signed data back to the site.
- The site verifies the signature using the registered public key. If the signature is valid, the user is authenticated.
- Security keys provide protection against phishing attacks due to the interactive nature of the process.
- Security keys are resistant to cloning or forgery because of their unique embedded secrets and tamper protection.
- From a convenience perspective, security keys offer a user-friendly authentication flow compared to OTPs, as users only need to tap the security key.
- As an IT support specialist, understanding multi-factor authentication setups, including biometrics and U2F, is essential for providing support and implementing such systems.

Note: These notes provide a detailed summary of the content, capturing the key points and concepts discussed in the module.

#multifactor-authentication #biometric-authentication #U2F-tokens #course5-module3 