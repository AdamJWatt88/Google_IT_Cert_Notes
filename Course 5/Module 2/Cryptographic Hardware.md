-   **Trusted Platform Module (TPM)**:
    
    -   Hardware device integrated into computer hardware as a dedicated crypto processor.
    -   Functions: secure key generation, random number generation, remote attestation, data binding and sealing.
    -   Contains unique secret RSA key burned during manufacturing for hardware authentication.
    -   Remote attestation: System authenticates software and hardware configuration to a remote system.
    -   TPM generates a secure hash of system configuration using its unique RSA key for integrity verification.
    -   Data binding and sealing: Secret key is used to derive a unique key for data encryption.
    -   Encrypted data is bound to the TPM and can only be decrypted using the TPM's key.
    -   Data sealing requires the TPM to be in a specified state for decryption.

-   **TPM Implementations**:
    
    -   Standard with several revisions: discrete hardware chip, integrated chip, firmware/software, or virtualized in a hypervisor.
    -   Discrete chip is most secure with physical tamper resistance to prevent physical attacks.
    -   Mobile devices have a similar concept called a secure element embedded in microprocessors or mainboards.
    -   Secure element provides tamper-resistant storage of cryptographic keys and a secure environment for applications.
    -   Trusted Execution Environment (TEE): Isolated execution environment alongside the main OS.
    -   TEE provides isolation of applications from the main OS and other applications, ensuring secure processes.

-   **Criticisms and Attacks on TPM**:
    
    -   Trusting the manufacturer: The manufacturer has access to the secret key burned into the hardware.
    -   Possibility of key duplication by the manufacturer, compromising TPM security.
    -   One reported attack using an electron microscope and micron precision equipment to view and access TPM contents.
    -   Attack proved physical tampering with the TPM is possible despite tamper protections.

-   **Full Disk Encryption (FDE)**:
    
    -   Encryption of the entire drive, protecting all contents from data theft or tampering.
    -   Implementations: PGP, Bitlocker (integrated with TPM), Filevault 2, dm-crypt.
    -   FDE configuration includes an encrypted partition (root volume) and a small unencrypted boot partition.
    -   Unencrypted partition contains elements like kernel, bootloader, and NRD for booting.
    -   User must enter a passphrase to unlock the encrypted disk during boot process.
    -   TPM can be utilized for disk encryption keys and platform integrity to prevent unlocking if system configuration changes.

-   **Importance of Randomness**:
    
    -   Random number selection is crucial in encryption.
    -   Pseudorandom numbers have patterns that can be discovered through observation and analysis.
    -   Operating systems maintain an entropy pool as a source of random data to seed random number generators.
    -   Dedicated random number generators and pseudorandom number generators are used for generating cryptographic keys.

-   **Conclusion**:
    
    -   Covered various cryptography concepts and applications.
    -   TPM provides secure key generation, attestation, and data binding/sealing.
    -   TPM implementations range from discrete chips to secure elements and trusted execution environments.
    -   Criticisms include trusting the manufacturer, but attacks require specialized equipment.
    -   Full disk encryption protects all contents and can utilize TPM for keys and platform integrity.
    -   Randomness is essential in encryption to avoid patterns; entropy pools and dedicated generators ensure randomness.

# Supplemental Reading for TPM Attacks

## There’s been one report of a [physical attack on a TPM](https://arstechnica.com/gadgets/2021/08/how-to-go-from-stolen-pc-to-network-intrusion-in-30-minutes/) which allowed a security researcher to view and access the entire contents of a TPM.

#trusted-platform-module #TPM #full-disk-encryption #FDE #cryptographic-hardware