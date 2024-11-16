https://learn.microsoft.com/en-us/training/modules/manage-innersource-program-github/

## Overview

> **InnerSource** is the practice of applying open-source patterns to projects with a limited audience. For example, a company might establish an InnerSource program that mirrors the structure of a typical open-source project, except that it's only accessible to the employees of that company. In effect, it's an open-source program behind your company's firewall.

Essentially, open source within your company. Pretty standard at the smaller orgs I've been at.

## Benefits

- **Encourages transparency**: See how others solve problems, find code & assets to reuse, helps understand other project's ideas.
- **Reduces friction**: Can directly raise PRs / issues against the codebase, and can even fork to meet needs (although this only applies at a massive company!).
- **Standardise practices**: Easier to communicate ways of working, coding practices etc when they're visible.

## How to set up

- Repositories can be public, **internal**, or private.
- Permissions can then be configured with 5 permission levels (quoted verbatim):
  - Read level is recommended for non-code contributors who want to view or discuss the project.
  - Triage level is recommended for contributors who need to proactively manage issues and pull requests without write access.
  - Write level is recommended for contributors who actively push to the project.
  - Maintain level is recommended for project managers who need to manage the repository without access to sensitive or destructive actions.
  - Admin level is recommended for people who need full access to the project, including sensitive and destructive actions like managing security or deleting a repository.

## Best practices

- Use descriptive repo name
- Have a concise description (sentence or two)
- License repo
- Include a `README.md`

## Readme contents

Quoted verbatim:

> - Articulate the purpose and vision of the project so potential consumers understand whether it fits their needs.
> - Offer visual aids, such as screenshots or code samples, to illustrate the project in action.
> - Include links to a production or demo version of the app for review.
> - Set expectations for prerequisites and deployment procedures.
> - Include references to the projects on which you depend. These references are a good way to promote the work of others.
> - Use Markdown to guide readers through properly formatted content.

## Special files

Some files can be in root (typical), `/docs`, or `/.github`:

- `CONTRIBUTING.md`: Explain contribution police, appears when people create issues / PRs.
- `README.md`: Information about the project.

Other files need to be in `/.github`:

- `ISSUE_TEMPLATE.md`: A template for issues.
- `PULL_REQUEST_TEMPLATE.md`: A template for PRs.

## Measuring success

Guidance on InnerSource success metrics, quoted directly:

> - Measure process, not output
>   - Code review turnaround time
>   - Pull request size
>   - Work in progress
>   - Time to open
> - Measure against targets and not absolutes
> - Measure teams and not individuals
>   - Number of unique contributors to a project
>   - Number of projects reusing code
>   - Number of cross-team @mentions

Absurdly detailed process guide: https://githubtraining.github.io/innersource-theory/#/measuring_success
