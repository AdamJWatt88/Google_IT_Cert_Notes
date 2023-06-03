-   **Asymmetric encryption** allows secure communication over untrusted channels **without** the need to share a shared secret or key.
-   **Asymmetric encryption** is **more complex** and computationally expensive compared to symmetric encryption.
-   **Symmetric encryption** algorithms are **faster** and more **efficient** for encrypting **large amounts of data**.
-   **Many secure communication schemes** combine **both** asymmetric and symmetric encryption for different purposes.
-   Asymmetric encryption is used as a key exchange mechanism in which the shared secret or symmetric encryption key is securely transmitted using asymmetric encryption.
-   Once the shared secret is received, data can be sent quickly and efficiently using symmetric encryption.
-   **MACs (Message Authentication Codes)** are related to asymmetric encryption and provide message authentication and data integrity.
-   MACs are **different from digital signatures** as they use the same secret key for generation and verification.
-   MACs **require** the secret key to be agreed upon or shared securely among all parties involved.
-   **HMAC (Hash-based Message Authentication Code**) is a popular type of MAC that uses a cryptographic hash function and a secret key to generate the MAC.
-   The strength of the MAC depends on the security of the underlying cryptographic hash function.
-   The MAC is sent alongside the message and is verified by performing the same operation on the received message and comparing the computed MAC with the received one.
-   **CMACs (Cipher-based Message Authentication Codes)** are MACs based on symmetric encryption ciphers like DES or AES.
-   CMACs use a shared key and encrypt the message to produce the MAC.
-   **CBC-MAC (Cipher Block Chaining Message Authentication Code)** is a specific type of CMAC that uses block ciphers in CBC mode.
-   CBC mode incorporates previously encrypted blocks into the next blocks of plaintext, creating a chain of interdependent encrypted blocks.
-   Any modification to the plaintext will result in a different output at the end of the chain, ensuring message integrity.

#asymmetric-encryption #symmetric-encryption #MAC #message-authentication-codes #HMAC #hash-based-message-authentication-code #CMAC #cipher-based-message-authentication-code #CBC-MAC #cipher-block-chaining-message-authentication-code #course5-module2 