**OAuth**:

- OAuth is an open standard that enables users to grant third-party websites and applications access to their information without sharing their account credentials.
- It allows for access delegation, where the user delegates access to their account to the third party.
- The user is prompted to confirm and authorize the specific information or access being requested by the third party.
- Upon authorization, the identity provider issues a token to the third party, granting them access to the user's information.
- OAuth is commonly used by large internet companies like Google, Microsoft, and Facebook to grant access to their APIs for third-party applications.

**Phishing Attacks and OAuth:**

- OAuth permissions can be exploited in phishing attacks, where attackers send fraudulent OAuth authorization requests to trick users into granting access to their accounts.
- This can lead to unauthorized access to accounts through the obtained OAuth authorization token.
- In 2017, an OAuth-based worm attack used phishing emails that appeared to be from a trusted source, requesting access to Google Docs. Victims unknowingly granted access, allowing the attacker to perpetuate the attack.

**OAuth and OpenID:**

- OAuth is an authorization system, while OpenID is an authentication system, although they are often used together.
- OpenID Connect is an authentication layer built on top of OAuth, enhancing the integration of authentication and authorization.

**TACACS+ and Authorization**:

- TACACS+ (Terminal Access Controller Access-Control System Plus) is a full AAA (Authentication, Authorization, and Accounting) system that handles both authentication and authorization.
- After a user is authenticated, TACACS+ determines access permissions, allowing or disallowing certain commands or device access for the user account.
- TACACS+ provides flexibility in granting admin access to certain users (e.g., networking teams) while limiting access for other users (e.g., support team with read-only access).
- More advanced AAA systems, like TACACS+, can further refine authorization at the command level, allowing precise control over access permissions.

**RADIUS and Authorization:**

- RADIUS (Remote Authentication Dial-In User Service) also allows for authorization of network access.
- Upon successful authentication to the RADIUS server, the server returns configuration information to the network access server.
- This information includes authorizations, specifying the network services the user is permitted to access (e.g., WiFi and VPN).

Overall, both OAuth and AAA systems like TACACS+ and RADIUS play crucial roles in managing access permissions, ensuring secure and controlled access to resources and services.

#OAuth #phishing #RADIUS #TACACS #course5-module3 