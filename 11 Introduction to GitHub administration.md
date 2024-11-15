https://learn.microsoft.com/en-us/training/modules/github-introduction-administration/

## Admin at different levels

Team / org / enterprise: https://learn.microsoft.com/en-us/training/modules/github-introduction-administration/2-what-is-github-administration

## GitHub auth options

- Username & password: Default, but no longer recommended as passwords can be reused etc.
- Personal access tokens: Alternative to passwords, and can have limited permissions. Token is tied to a repo / org, so much safer.
- SSH keys: Used instead of username & password / PAT, can be used to automatically authenticate without needing manual auth for every interaction.
- Deploy keys: Type of SSH key that grants user access to a specific repo. Haven't used these personally.

## Additional auth options

- 2FA
- SAML SSO (e.g. Okta)
- LDAP: "Lightweight directory access protocol (LDAP) is a popular application protocol for accessing and maintaining directory information services." (e.g. Active Directory).

## Org permission levels

| **Permission level**     | **Description**                                                                                                                                                                                                           |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Owner**                | Organization owners can do everything that organization members can do, and they can add or remove other users to and from the organization. This role should be limited to no less than two people in your organization. |
| **Member**               | Organization members can create and manage organization repositories and teams.                                                                                                                                           |
| **Moderator**            | Organization moderators can block and unblock nonmember contributors, set interaction limits, and hide comments in public repositories that the organization owns.                                                        |
| **Billing manager**      | Organization billing managers can view and edit billing information.                                                                                                                                                      |
| **Security managers**    | Organization security managers can manage security alerts and settings across your organization. They can also read permissions for all repositories in the organization.                                                 |
| **Outside collaborator** | Outside collaborators, such as a consultant or temporary employee, can access one or more organization repositories. They aren't explicit members of the organization.                                                    |

## Protection rules

Rules that can be applied:

> - Require a pull request before merging.
> - Require status checks to pass before merging.
> - Require conversation resolution before merging.
> - Require signed commits.
> - Require linear history.
> - Require merge queue.
> - Require deployments to succeed before merging.
> - Lock the branch by making it read-only.
> - Restrict who can push to matching branches.
