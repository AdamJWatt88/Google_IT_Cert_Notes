- The **most secure option for protecting wireless networks is 802.1X with EAP-TLS**, as it offers the best security, assuming proper handling of the **Public Key Infrastructure (PKI)** aspects.
- However, **implementing EAP-TLS requires additional complexity and overhead**, including the use of a **RADIUS** server and an authentication back-end. PKI components and certificate management are also necessary.
- Companies often find the **overhead of implementing EAP-TLS to be too high**, considering the trade-off between security and convenience.
- An **alternative to EAP-TLS is WPA2 with AES/CCMP mode**, which provides good security against brute force or rainbow table attacks.
- To further enhance security with **WPA2**, it is recommended to use a long and complex passphrase that is not found in dictionaries.
- Changing the **SSID** to a unique and uncommon value also reduces the likelihood of rainbow table attacks, as attackers would need to perform computations themselves.
- Although a long and complex Wi-Fi password might tempt users to use **WPS (Wi-Fi Protected Setup)** for convenience, it is **generally not recommended for security reasons**.
- WPS is more commonly used in consumer-oriented environments and should be disabled in enterprise environments that prioritize security over convenience.
- It is **important to verify that WPS is disabled on access points (APs)**, as some router manufacturers may not allow the feature to be disabled through the management console.
- Tools like **Wash** can be used to scan and enumerate APs that have WPS enabled, providing independent verification of the feature's status.

#8021X #EAP-TLS #PKI #RADIUS #WPA2 #AES #CCMP #bruteforce #rainbowtable #SSID #WPS #Wi-FiProtectedSetup #dictionaries #security #convenience #enterprise #verification #accesspoints #routermanufacturers #managementconsole #tools #Wash #course5-module4 