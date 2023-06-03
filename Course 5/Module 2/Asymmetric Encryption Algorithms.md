-   **RSA (Rivest-Shamir-Adleman)** is a practical asymmetric cryptography system.
-   RSA was patented in 1983 and released to the public domain in 2000 by RSA Security.
-   **RSA specifies key generation, distribution, encryption, and decryption operations**.
-   Key generation in RSA involves choosing two unique, random, and large prime numbers.
-   **DSA (Digital Signature Algorithm)** is another asymmetric encryption system used for signing and verifying data.
-   DSA was patented in 1991 and is part of the US government's federal information processing standard.
-   DSA's security depends on a random seed value used in the signing process.
-   In 2010, Sony's PlayStation 3 Game Console was compromised due to a flaw in DSA's randomization process.
-   Asymmetric systems are commonly used as key exchange mechanisms to establish a shared secret for symmetric ciphers.
-   **Diffie-Hellman (DH**) is a popular key exchange algorithm.
-   DH involves two parties agreeing on a starting number and choosing secret numbers to combine with the shared number.
-   DH allows the parties to derive a shared secret without revealing enough information to eavesdroppers.
-   DH was designed for key exchange but has been adapted for encryption purposes and used in **PKI systems**.
-   **Elliptic Curve Cryptography (ECC)** is a public-key encryption system that uses the algebraic structure of elliptic curves over finite fields.
-   ECC generates secure keys using the properties of elliptic curves.
-   **Elliptic curves** have properties like horizontal symmetry and limited intersections with non-vertical lines.
-   ECC provides security comparable to traditional public key systems but with smaller key sizes.
-   **ECDH (Elliptic Curve Diffie-Hellman)** and **ECDSA (Elliptic Curve Digital Signature Algorithm)** are elliptic curve variants of Diffie-Hellman and DSA.
-   The US NIST recommends EC encryption, and the NSA allows its use to protect top-secret data with 384-bit EC keys.
-   The NSA has expressed concerns about the potential vulnerability of EC encryption to quantum computing attacks.

# Supplemental Reading for Asymmetric Encryption Attack

- An asymmetric encryption attack happened in 2010 to [Sony with their Playstation 3](https://nakedsecurity.sophos.com/2012/10/25/sony-ps3-hacked-for-good-master-keys-revealed/) game console. It turns out they weren’t ensuring the randomized seed value was changed for every signature. This resulted in a hacker group called 'fail0verflow' being able to recover the private key that Sony used to sign software for the platform. This allowed modders to write and sign custom software that was allowed to run on the otherwise very locked down console platform. This [resulted in game piracy](https://www.theguardian.com/technology/gamesblog/2011/jan/07/playstation-3-hack-ps3) becoming a problem for Sony, as this facilitated the illicit copying and distribution of games, causing a significant loss in sales.

#RSA #rivest-shamir-adleman #DSA #digital-signature-algorithm #Diffie-Hellman #PKI-systems #elliptic-curve-cryptography #ECC #ECDH #elliptic-curve-diffie-hellman #ECDSA #elliptic-curve-digital-signature-algorithm #course5-module2 