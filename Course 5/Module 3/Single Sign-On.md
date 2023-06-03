- **Single sign-on (SSO**) is an authentication concept that enables users to authenticate once and gain access to multiple services and applications without the need for repeated authentication.
- With **SSO**, users do not require separate sets of usernames and passwords for each application or service, as they authenticate to a central authentication server, such as an **LDAP server**.
- After successful authentication, the central authentication server provides a cookie or token that can be used to access applications configured to use SSO.
- Kerberos is an example of an SSO authentication service. Users authenticate against the Kerberos service once, **receiving a ticket-granting ticket** that can be presented to the ticket-granting service instead of traditional credentials.
- **SSO offers convenience by allowing users to use a single set of credentials** to access multiple services, reducing the likelihood of insecure password storage or writing down passwords.
- SSO also **reduces the burden of password assistance support** and eliminates the need for frequent re-authentication during the workday.
- However, a downside of SSO is that if an attacker compromises an account, they gain access to all applications and services associated with that account.
- **Implementing multi-factor authentication alongside SSO** is highly recommended to enhance security.
- SSO introduces a **new attack vector: theft of SSO session cookies or tokens**. Attackers may attempt to steal these tokens to gain wide access, potentially bypassing multi-factor authentication protections until the token expires.
- An example of an SSO system is **OpenID**, a decentralized authentication system based on an open standard.
- **OpenID** allows participating sites (relying parties) to authenticate users through a third-party authentication service (identity provider), eliminating the need for individual site-specific authentication infrastructure.
- Users can access sites without creating new accounts, simplifying access management across multiple sites by leveraging an existing account with an identity provider.
- In the OpenID authentication process, the relying party looks up the OpenID provider, establishes a shared secret for validating provider messages, and redirects the user to the identity provider's login flow.
- Once authenticated, the user confirms trust with the relying party, and credentials are relayed to the relying party in the form of a token, indicating successful authentication to the service.

#SSO #single-sign-on #OpenID #authentication #course5-module3 