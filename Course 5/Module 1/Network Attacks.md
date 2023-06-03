-   **DNS cache poisoning attack**:
    
    -   Simple concept but can cause significant damage.
    -   Tricking DNS server into accepting a fake DNS record.
    -   Fake record points to a compromised DNS server.
    -   Fake DNS addresses served when accessing legitimate websites.
    -   Can spread to other networks if their DNS servers are compromised.
    -   Example: Large-scale DNS cache poisoning attack in Brazil.
        -   Attackers poisoned DNS cache of local ISPs.
        -   Inserted fake DNS records for popular websites (Google, Gmail, Hotmail).
        -   Users redirected to attacker-controlled server hosting a malicious banking trojan.
        -   Trojan designed to steal banking credentials.

-  **Man-in-the-middle attack (MITM)**:
    
    -   Attack where the attacker positions themselves between two communicating hosts.
    -   Monitors and potentially modifies information in transit.
    -   Session hijacking is a common MITM attack.
        -   Stealing authentication token to impersonate the user.
    -   Ensuring data integrity is crucial for protection against MITM attacks.
    -   Rogue access point attack:
        -   Unauthorized access point installed on the network without admin knowledge.
        -   Plugging a router into a corporate network to create a wireless network.
        -   Allows unauthorized access to secure network from outside the building.

-  **Evil Twin attack**:
        -   Similar to rogue AP, but creates an identical network to the target network.
        -   Attacker controls the identical network (Evil Twin).
        -   Monitoring and capturing traffic when users connect to it.

# Supplemental Reading for Network Attacks

- If you're interested in reading a news story about a network attack, check out the following link [here](https://threatpost.com/major-dns-cache-poisoning-attack-hits-brazilian-isps-110711/75859/).

#network-attacks #DNS-cache-poisoning-attack #man-in-the-middle-attack #evil-twin-attack #course5-module1 