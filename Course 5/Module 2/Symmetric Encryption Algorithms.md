 -   **Symmetric encryption algorithms** are more **complex** and secure than substitution ciphers.
-   **DES (Data Encryption Standard)** was one of the earliest encryption standards, with a **64-bit key size (56 bits without parity bits)**.
-   **Key size** determines the maximum potential strength of an encryption system.
-   Brute force attacks involve guessing the key to decrypt the message.
-   DES proved to have a small key size vulnerability, leading to the development of replacement algorithms.
-   **AES (Advanced Encryption Standard)** replaced DES and uses a **128-bit block size** and **supports key lengths of 128, 192, or 256 bits**.
-   **AES** is **approved for top-secret information** by the US NSA and has theoretical resistance to brute-force attacks.
-   Encryption algorithms need to be implemented in software or hardware for practical use.
-  **Speed and ease of implementation are important considerations for encryption algorithms.**
-   Hardware acceleration, such as AES instructions in modern CPUs, can improve computational speed and efficiency.
-  **RC4 (Rivest Cipher 4**) was a popular but weak symmetric stream cipher.
-   RC4 has **inherent weaknesses and vulnerabilities**, leading to its discouragement and abandonment in many protocols.
-   Major web browsers dropped support for RC4 and SSL/TLS versions due to vulnerabilities.
-   Preferred secure configurations include **TLS 1.2** with **AES GCM (Galois/Counter Mode),** which combines AES block cipher with a stream cipher-like operation.

# Supplemental Reading for Symmetric Encryptions

- For more information about symmetric encryptions, check out the following link [here](http://www.rc4nomore.com/).

#symmetric-encryption-algorithm #DES #data-encryption-standard #AES #advanced-encryption-standard #RC4 #rivest-cipher-4 #course5-module2 