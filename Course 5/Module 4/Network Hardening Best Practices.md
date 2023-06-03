- Network hardening is the process of securing a network by reducing vulnerabilities through configuration changes and specific steps.
- Disabling unnecessary services or restricting access to them is a general security principle that should be applied to network security.
- Implicit deny is a network security concept where anything not explicitly permitted should be denied.
- **Implicit deny** can be configured on a firewall through **Access Control List (ACL)** configurations, making it easier to build secure firewall rules.
- Network security monitoring and analysis are crucial components of network security.
- Monitoring allows establishing a baseline of normal network traffic to identify unusual or potential attack traffic.
- Network traffic monitoring and log analysis help in understanding network behavior and detecting potential intrusions, malware infections, or atypical behavior.
- Logs from different network and client devices, such as firewall logs, authentication server logs, and application logs, are valuable sources of information for analysis.
- IT support specialists should pay close attention to external-facing devices or services that are more susceptible to malicious traffic.
- Logs analysis systems are configured using user-defined rules to identify interesting or atypical log entries and generate alerts for further investigation.
- Normalizing log data is necessary to convert logs from different devices and systems into a common format for easier analysis and correlation.
- Correlation analysis involves matching events across different systems to identify connections and potential threats.
- Detailed logging and log analysis are critical in investigating and reconstructing events after a breach to prevent further attacks and determine the extent of the compromise.
- **Splunk** is a popular and powerful log analysis system that aggregates and searches logs from various systems and formats, generating alerts and visualizations.
- **Flood guards** protect against Denial of Service (DoS) attacks and ensure availability of network resources.
- Flood guards identify common flood attack types and trigger alerts or block attack traffic based on configurable thresholds.
- **Fail2Ban** is an open-source flood guard protection tool that blocks further attempts from a suspected attack address.
- Network separation or segmentation is a security principle that involves creating virtual networks (VLANs) for different device classes to enhance management and security.
- Network separation allows for more control and monitoring of traffic flow between networks, reducing the risk of unauthorized access.
- Routing and network ACLs are used to provide appropriate access between different networks, such as enabling employee access to printers on a separate network.

Note: These detailed notes cover the main points and concepts mentioned in the given text.

# Supplemental Reading for Network Hardening Best Practices

## For more information on this Video Lecture check out the following links:

[Cisco IOS firewall rules](https://www.cisco.com/en/US/docs/routers/access/800/850/software/configuration/guide/firewall.html "Cisco IOS firewall rules")

[Juniper firewall rules](https://www.juniper.net/documentation/en_US/junos/topics/usage-guidelines/services-configuring-stateful-firewall-rules.html)

[Iptables firewall rules](https://www.digitalocean.com/community/tutorials/iptables-essentials-common-firewall-rules-and-commands)

[UFW firewall rules](https://www.digitalocean.com/community/tutorials/ufw-essentials-common-firewall-rules-and-commands)

[Configuring Mac OS X firewall](https://support.apple.com/en-us/HT201642)

[Microsoft firewall rules](https://technet.microsoft.com/en-us/library/cc754274(v=ws.11).aspx)

#network-hardening #Fail2Ban #flood-guards #Splunk #course5-module4 