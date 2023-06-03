-   Cryptographic hash functions are crucial for authentication, where passwords are securely stored as hash digests instead of plain text.
-   Storing passwords in plain text is insecure, as it exposes sensitive information in the event of a system compromise.
-   When a user enters their password, it is run through a hash function, and the resulting hash digest is compared with the stored hash for authentication.
-   Brute force attacks involve trying all possible input values until a matching hash is found, allowing the attacker to determine the corresponding password.
-   Brute force attacks can be computationally intensive, and the goal is to make them infeasible within a useful time frame.
-   One method to raise the computational bar is to run the password through the hash function multiple times (thousands of iterations).
-   **Rainbow tables** are precomputed tables of password values and their corresponding hashes, used to speed up password recovery from stolen password hashes.
-   **Rainbow table** attacks trade computational power for disk space by storing precomputed hashes.
-   **Salts** are additional randomized data added to the password before hashing, making rainbow table attacks more difficult.
-   Salts ensure that each password has a unique hash, and an attacker would need to compute a rainbow table for each possible salt value.
-   Using a large salt value increases the computational and storage requirements for generating useful rainbow tables.
-   Modern systems use long salt values (e.g., 128-bit) that make rainbow table attacks infeasible within a realistic timeframe.
-  **Salting passwords significantly enhances their security** and raises the bar against rainbow table attacks.

#hashing #salts #rainbow-table #course5-module2 