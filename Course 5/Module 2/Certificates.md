-   X.509 Standard:
    
    -   The X.509 standard defines the format of digital certificates and includes a certificate revocation list (CRL) for distributing information about invalidated certificates.
    -   First issued in 1988, the modern version is Version 3.

-   Fields in an X.509 Certificate:
    
    1.  **Version**: Indicates the X.509 standard version followed by the certificate.
    2.  **Serial Number**: Uniquely identifies the certificate and assists the Certificate Authority (CA) in managing and identifying individual certificates.
    3.  **Certificate Signature Algorithm**: Specifies the public key algorithm used for the certificate's public key and the hashing algorithm used to sign the certificate.
    4.  **Issuer Name**: Contains information about the authority that signed the certificate.
    5.  **Validity**: Comprises two subfields - Not Before and Not After - defining the dates when the certificate is valid.
    6.  **Subject**: Contains identifying information about the entity to which the certificate was issued.
    7.  **Subject Public Key Info**: Two subfields defining the algorithm and public key of the certificate's subject.
    8.  **Certificate Signature Algorithm (again**): Matches the subject public key algorithm and field.
    9.  **Certificate Signature Value**: Represents the digital signature data itself.
    
    -   Additionally, certificate fingerprints are computed by clients during validation or inspection, serving as hash digests of the entire certificate.

-   Web of Trust:
    
    -   An alternative to the centralized PKI model is the concept of a web of trust.
    -   In a web of trust, individuals sign other individuals' public keys rather than relying solely on certificate authorities.
    -   Before signing a key, an individual verifies the person's identity through an agreed-upon mechanism, such as checking identification documents.
    -   By signing the public key, the individual vouches for the association between the key and the person's identity, establishing trust.
    -   This process is reciprocal, with both parties signing each other's keys.
    -   Key signing parties are organized to facilitate the establishment of web of trust, where participants verify identities and sign keys.
    -   At the end of the party, each participant's public keys should be signed by every other participant, creating a web of trust.
    -   Over time, when a participant from the initial key signing party establishes trust with a new member, the web of trust expands to include the new member and individuals trusted by that member.
    -   This allows separate webs of trust to be interconnected, enabling the network of trust to grow.

Note: These detailed notes provide an in-depth exploration of certificates, covering the X.509 standard, its fields, and the concept of a web of trust as an alternative to the centralized PKI model.

# Supplemental Reading for the X.509 Standard

## For more information about this topic from this Video Lecture check out the following link. The [X.509 standard](https://www.ietf.org/rfc/rfc5280.txt) is what defines the format of digital certificates.

#certificates #X509 #web-of-trust #course5-module2 