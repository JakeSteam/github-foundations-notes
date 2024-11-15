https://learn.microsoft.com/en-us/training/modules/maintain-secure-repository-github/

## Secure development strategy

Many aspects to consider, but three in particular (quoted verbatim):

> - **There's a general knowledge problem**: Many developers and other staff members assume they understand security, but they don't. Cybersecurity is a constantly evolving discipline. A program of ongoing education and training is essential.
>
> - **Code must be created correctly and securely**: We need to be sure that the code is created correctly and securely implements the required features. We also need to make sure that the features were designed with security in mind.
>
> - **Applications must comply with rules and regulations**: We need to make sure that the code complies with required rules and regulations. We have to test for compliance while building the code and then retest periodically, even after deployment.

## Security tab features

- `SECURITY.md`: Like `CONTRIBUTING.md`, defines how to report a security vuln. [More info](https://docs.github.com/code-security/getting-started/adding-a-security-policy-to-your-repository).
- Dependabot alerts when the repo is using vulnerable dependencies or malware.
- Security advisories with alerts about general security vulns in the repo.
- Code scanning to find, triage, fix, vulns & errors in code.

## Other security features

- `.gitignore` can exclude sensitive info (like configs).
- It _correctly_ points out any file pushed to a public repo should be assumed compromised, and keys should be rotated etc.
- Branch protection rules can prevent main branch force pushes, require PRs, etc. [More info](https://docs.github.com/repositories/configuring-branches-and-merges-in-your-repository/managing-protected-branches/managing-a-branch-protection-rule).
- `CODEOWNERS` can set up people required to review certain areas / filetypes. [More info](https://docs.github.com/github/creating-cloning-and-archiving-repositories/creating-a-repository-on-github/about-code-owners#codeowners-syntax).
- Secret scanning automatically looks for common credential patterns (e.g. API keys) then performs an action depending on the service provider. Might revoke, issue a new secret, or let the provider reach out to user.

## Exercise

https://github.com/skills/secure-repository-supply-chain
