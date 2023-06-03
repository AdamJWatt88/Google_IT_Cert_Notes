-   **MD5 (Message Digest Algorithm 5)** is a popular cryptographic hash function designed in the early 1990s.
-   It operates on **512-bit blocks** and generates a **128-bit hash digest.**
-   MD5 had a design flaw discovered in 1996, but it continued to be widely used despite the recommendation to use the more secure **SHA1 hash**.
-   In 2004, MD5 was found to be susceptible to hash collisions, allowing malicious actors to create different files with the same MD5 hash.
-   The vulnerabilities in MD5 were further exploited in 2008 when security researchers demonstrated the creation of a fake SSL certificate using an MD5 hash collision.
-   Due to these serious vulnerabilities, it was recommended to stop using MD5 for cryptographic applications by 2010.
-   **SHA1 (Secure Hash Algorithm 1)** is another widely used cryptographic hash function published in 1995.
-   It operates on **512-bit blocks** and generates a **160-bit hash digest**.
-   **SHA1 is used in protocols like TLS/SSL, PGP/SSH, and IPSec**, as well as version control systems like Git.
-   SHA1 has also been found to have weaknesses and vulnerabilities, leading to recommendations for replacement with SHA2 or SHA3.
-   Security researchers have demonstrated partial collisions and theoretical attacks against SHA1, with full collisions requiring significant computing power.
-   In early 2017, the first full collision of SHA1 was published, highlighting the increasing feasibility of attacks against the hash function.
-   **Message Integrity Check (MIC)** is a concept related to hash functions, providing a checksum for a message to ensure it wasn't modified in transit.
-   MICs do not use secret keys and do not authenticate the message, making them vulnerable to tampering or malicious actions.
-   MICs primarily protect against accidental corruption or loss of the message


# Supplemental Reading for SHA1 Attacks

## During the 2000s, a bunch of [theoretical attacks](https://eprint.iacr.org/2005/010) against SHA1 were [formulated](https://www.schneier.com/blog/archives/2005/02/sha1_broken.html) and some [partial collisions](https://eprint.iacr.org/2007/474) were demonstrated. In early 2017, the first [full collision of SHA1](https://shattered.io/) was published.

#MD5 #message-digest-algorithm-5 #SHA1 #secure-hash-algorithm-1 #message-integrity-check #MIC #course5-module2 