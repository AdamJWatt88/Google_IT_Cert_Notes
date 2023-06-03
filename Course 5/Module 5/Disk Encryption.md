- **Full disk encryption (FDE)** is an important component of a defense-in-depth security model.
- FDE protects against physical forms of attack and prevents data theft from stolen or lost hard drives.
- FDE is recommended for **mobile devices** like laptops, cell phones, and tablets, as well as desktops and servers.
- FDE provides **confidentiality and integrity**, preventing unauthorized tampering with system files and malware installation.
- Critical boot files are stored in an **unencrypted partition** on the disk for the system to boot with FDE.
- These boot files, such as the kernel and bootloader, can be vulnerable to replacement by an attacker with physical access.
- **Secure boot protocol**, using public key cryptography, protects against tampering with the unencrypted boot partition.
- Microsoft's **BitLocker** and Apple's **FileVault 2** are first-party FDE solutions, while there are also third-party and open-source options like **DM crypt, PGP, TrueCrypt, and FileCrypt**.
- FDE relies on a **secret key** for encryption and decryption, often **password-protected**, with the encryption key used to derive a user key.
- **Key escrow functionality** allows authorized parties to securely store and retrieve the encryption key or recovery passphrase if the user forgets the password.
- **File-based encryption**, such as home directory encryption, only encrypts specific files or folders, offering confidentiality and integrity for those files but leaving system files unencrypted.
- File-based encryption is less protected against physical attacks and compromises between security and usability.
- Understanding **threats** and their associated **risks** is crucial for designing a security architecture and selecting appropriate defenses.

# Supplemental Reading for Disk Encryption

There are first-party full-disk encryption (FDE) solutions from Microsoft and Apple, called [BitLocker](https://docs.microsoft.com/en-us/windows/security/information-protection/bitlocker/bitlocker-overview) and [FileVault 2](https://support.apple.com/en-us/HT204837), respectively.

There are also a bunch of third-party and open-source solutions. On Linux, the [dm-crypt package](https://wiki.archlinux.org/index.php/dm-crypt) is very popular.

There are also offerings from [PGP](https://www.symantec.com/products/encryption), [VeraCrypt](https://www.veracrypt.fr/en/Home.html) and a host of others.

#Full-disk-encryption #FDE #Defense-in-depth-security-model #Physical-forms-of-attack #Data-theft #Stolen-or-lost-hard-drives #Mobile-devices #Confidentiality #Integrity #Unauthorized-tampering #System-files #Malware-installation #Critical-boot-files #Unencrypted-partition #Kernel #Bootloader #Replacement-by-attacker #Physical-access #Secure-boot-protocol #Public-key-cryptography #Unencrypted-boot-partition #Microsoft-BitLocker #Apple-FileVault-2 #Third-party-and-open-source-options #DM-crypt #PGP #TrueCrypt #FileCrypt #Secret-key #Encryption-and-decryption #Password-protected #User-key #Key-escrow-functionality #Authorized-parties #Recovery-passphrase #Forgotten-password #File-based-encryption #Home-directory-encryption #Specific-files-or-folders #Confidentiality-and-integrity #System-files-unencrypted #Physical-attacks #Compromises #Security-architecture #Appropriate-defenses #Threats #Risks #course5-module5 