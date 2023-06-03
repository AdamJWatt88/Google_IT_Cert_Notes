
## Resources
- Many **network protocols** are implemented based on specifications published by the [Internet Engineering Task Force (IETF)](https://www.ietf.org/).
- The most common **distance vector protocols**
	 - [RIP, or Routing Information Protocol](https://en.wikipedia.org/wiki/Routing_Information_Protocol) 
	 - [IETF RFC2453](https://tools.ietf.org/html/rfc2453)
	 - [EIGRP, or Enhanced Interior Gateway Routing Protocol](https://en.wikipedia.org/wiki/Enhanced_Interior_Gateway_Routing_Protocol) 
	 - [Cisco documentation](https://www.cisco.com/c/en/us/support/docs/ip/enhanced-interior-gateway-routing-protocol-eigrp/16406-eigrp-toc.html)
* In terms of **exterior gateway protocols**, there is only one in use today. The entire Internet needs to agree on how to exchange this sort of information, so a single standard has emerged. This standard is known as [BGP, or Border Gateway Protocol](https://en.wikipedia.org/wiki/Border_Gateway_Protocol) ([IETF RFC4271](https://tools.ietf.org/html/rfc4271))**.

## Notes 
- **Exterior gateway protocols (EGPs)** allow routers from different organizations to exchange data
-   EGPs are essential to the functioning of the Internet
-   The Internet is composed of many autonomous systems, and core Internet routers need to know about these systems in order to properly forward traffic
-   The **Internet Assigned Numbers Authority (IANA)** is responsible for managing IP address allocation and **Autonomous System Number (ASN)** allocation
-   ASNs are 32-bit numbers assigned to individual autonomous systems
-   ASNs never need to change in order to represent more networks or hosts, but the core Internet routing tables need to be updated to reflect the change
-   ASNs are looked at by humans far less often than IP addresses, and they represent entire autonomous systems
-   Understanding the basics of autonomous systems, ASNs, and how core Internet routers route traffic between them is important to understand some of the basic building blocks of the Internet

#exterior-gateway-protocols #Internet-assigned-numbers-authority #autonomous-system-number #course2-module2 #IEFT