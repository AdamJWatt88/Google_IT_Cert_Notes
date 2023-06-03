- **Host-based firewalls** are important for creating multiple layers of security.
- They protect individual hosts from compromise in untrusted and potentially malicious environments.
- Host-based firewalls also protect hosts from potentially compromised peers within trusted networks.
- **Network-based firewalls** filter traffic in and out of the internal network, while host-based firewalls protect individual machines.
- Starting with an **implicit deny rule** in both network-based and host-based firewalls provides a secure default configuration.
- **Selective enabling** of specific services and ports allows only known and trusted traffic.
- Host-based firewall configurations may differ from network firewall configurations, tailored to the specific needs of individual hosts.
- Minimizing **attack surfaces** and exposure is crucial for securing systems, and host-based firewalls play a significant role in this aspect.
- Host-based firewalls provide flexibility by permitting connections to selective services on a given host from specific networks or IP ranges.
- This capability is commonly used to implement a highly secure **host-to-network connection**.
- **Bastion hosts** or networks are specifically hardened and minimized to reduce what is permitted to run on them.![[bastion_host.png]]
- Bastion hosts can be exposed to the Internet and used as gateways or access portals to more sensitive services like authentication servers or domain controllers.
- **Monitoring and logging** can be prioritized for bastion hosts, and they typically have limited network connectivity.
- Applications installed on bastion hosts are restricted to those that are strictly necessary given their specific purpose.
- Host-based firewall rules may include access rules that allow connections from **VPN subnets**.
- It is good practice to keep the network to which VPN clients connect separate using subnetting and VLANs.
- Separating the VPN network allows for more granular security enforcement and additional layers of defense.
- VPN hosts should be protected using other means as they operate in a potentially malicious environment and represent a vector of attack.
![[monitor_traffic-on_vpn.png]]
- **Monitoring traffic** to and from VPN hosts is important for detecting and preventing compromise.
- For client systems like laptops, **users with administrative rights have the ability to change firewall rules and configurations**.
- Logging should be implemented to monitor any changes made by users with administrative privileges.
- If possible, **prevent the disabling** of host-based firewalls, especially for client systems.
- Management tools like **Active Directory** can help prevent the disabling of host-based firewalls, particularly with Microsoft Windows machines.

  
#Host-based-firewalls #Multiple-layers-of-security #Compromise #Untrusted-environments #Potentially-malicious-environments #Trusted-networks #Network-based-firewalls #Individual-machines #Implicit-deny-rule #Secure-default-configuration #Selective-enabling #Specific-services #Specific-ports #Known-traffic #Trusted-traffic #Network-firewall-configurations #Attack-surfaces #Flexibility #Host-to-network-connection #Bastion-hosts #Minimized #Internet-exposure #Gateways #Access-portals #Sensitive-services #Authentication-servers #Domain-controllers #Monitoring #Logging #Limited-network-connectivity #VPN-subnets #Subnetting #VLANs #Granular-security-enforcement #Additional-layers-of-defense #VPN-hosts #Potentially-malicious-environment #Vector-of-attack #Administrative-rights #Firewall-rules #Configurations #Disabling #Client-systems #Management-tools #Active-Directory #Microsoft-Windows-machines #course5-module5 