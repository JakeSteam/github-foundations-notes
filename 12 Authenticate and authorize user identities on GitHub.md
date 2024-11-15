https://learn.microsoft.com/en-us/training/modules/authenticate-authorize-user-identities-github/

## SAML SSO

> - Before enabling SAML SSO with your GitHub Enterprise, an Administrator needs to connect the GitHub organization to a supported IdP.
> - Next, when a member accesses resources within an organization that uses SAML SSO, GitHub redirects the member to the IdP to authenticate.
> - After successful authentication, the IdP redirects the member back to GitHub, where the member can access the organization's resources. The result means that even after configuring SAML SSO, the GitHub organization's members will continue to be prompted to log into their user accounts on GitHub.

## Types of 2FA

- Physical security key: Most secure, but usually also requires one of the following.
- Time-based OTP: E.g. Authy.
- SMS: Not supported in all regions (also SMS is less secure).

## Usage limits

> - Maximum number of members in a GitHub team: 5,000
> - Maximum number of members in a GitHub organization: 10,000
> - Maximum number of teams in a GitHub organization: 1,500

## Misc

- "SCIM" can be used to synchronise between GitHub and SSO provider.
