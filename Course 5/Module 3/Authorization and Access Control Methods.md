- Authorization is a component of the AAA (Authentication, Authorization, and Accounting) security framework, closely related to authentication.
- While authentication verifies the identity of a user, authorization determines what resources or actions the user account is allowed or denied access to.
- Authentication and authorization are separate components with distinct purposes in ensuring secure access to systems and services.
- Successful authentication alone does not guarantee access to a system or resource; authorization is required to determine if the authenticated user has the necessary privileges.
- In the context of Kerberos, after successful authentication and receiving a ticket granting ticket, authorization comes into play when requesting access to a specific service.
- The ticket granting service verifies if the authenticated user is authorized to access the requested service. If not authorized, access is denied by the ticket granting service.
- If the user is authorized, the ticket granting service issues a ticket that grants access to the requested service.
- **OAuth** is a widely used open standard for authorization and access delegation, employed by companies like Google, Facebook, and Microsoft.
- **OAuth** enables users to grant limited access to their resources (such as personal information) to third-party applications or services without disclosing their credentials.
- It allows users to authorize applications to access specific resources on their behalf without sharing their username and password.
- OAuth uses access tokens to represent the authorized access and provides a secure mechanism for authorization and delegation of access rights.
- By implementing OAuth, companies can provide their users with seamless access to various services and applications while maintaining control over the access privileges granted.
- OAuth is widely adopted in scenarios where users want to utilize their existing accounts with trusted identity providers to access multiple services without creating separate accounts for each service

# Supplemental Reading for Authorization

## This was used in an [OAuth-based worm-like attack](https://www.theverge.com/2017/5/3/15534768/google-docs-phishing-attack-share-this-document-with-you-spam) in early 2017, with a rash of phishing emails that appeared to be from a friend or colleague who wants to share a Google Document.

#authentication #authorization #OAuth #course5-module3 