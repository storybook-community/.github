# Contributing

This page covers how to join the organization, how we operate and what is expected on every repository of the organization and from every member.

## Joining the community

### Team structure

The organization is divided in two teams:
* [Trusted Contributors](https://github.com/orgs/Storybook-Community/teams/trusted-contributors) are Storybook maintainers and long-term contributors who are trusted to manage the NPM and GitHub spaces
* [Community Contributors](https://github.com/orgs/Storybook-Community/teams/community-contributors) manage an individual repository that they have forked and maintained after it was abandonned

New members are added to the community contributors team and given full access to the repositories they create or transfer. They do not have full write access to other repositories.

To be included in the trusted contributors team, organization members must first be invited to the Storybook organization as contributors or maintainers. This distinction is made to keep our end users safe and limit the security exposure associated with an open community publishing NPM packages.

### Joining

This community works by invitation only. Community admins will get in touch with you to offer you to join the community. We typically invite people who commit to maintaining someone else's addon after a major update of Storybook.

## Community standards

### Code of Conduct

Please read the [Code of Conduct](https://github.com/storybook-community/.github/profile/CODE_OF_CONDUCT.md) first. All contributors must adhere to this code of conduct.

### Developer Certificate of Origin

To ensure that contributors are legally allowed to share the content they contribute under the license terms of this project, contributors must adhere to the [Developer Certificate of Origin](https://developercertificate.org/) (DCO). All contributions made must be signed to satisfy the DCO. This is handled by a Pull Request check.

> By signing your commits, you attest to the following:
>
> 1. The contribution was created in whole or in part by you and you have the right to submit it under the open source license indicated in the file; or
> 2. The contribution is based upon previous work that, to the best of your knowledge, is covered under an appropriate open source license and you have the right under that license to submit that work with modifications, whether created in whole or in part by you, under the same open source license (unless you are permitted to submit under a different license), as indicated in the file; or
> 3. The contribution was provided directly to you by some other person who certified 1., 2. or 3. and you have not modified it.
> 4. You understand and agree that this project and the contribution are public and that a record of the contribution (including all personal information you submit with it, including your sign-off) is maintained indefinitely and may be redistributed consistent with this project or the open source license(s) involved.

## Repository conventions

Repositories in the organization must follow the below principles:

* The `main` branch must be protected from force pushes and direct commits
* Releases must be made on `main` only (via `auto`, `semantic-release` or `changesets` based on preferences)
* Canary releases should be made on PR branches (through an `auto` canary release workflow)
* Fork packages must be named `@storybook-community/<original-name>` so they are published in the correct NPM namespace
* The following checks must be enabled in the CI/CD pipeline for pushes to the `main` branch: `build`, `test`, `CodeQL`, `dco`

We encourage contributors to keep their package compatible with the https://github.com/storybookjs/addon-kit overall CI/CD structure and script names. It's acceptable to replace package managers (we favour `pnpm`) and to add extra tooling (e.g. ESLint, lint-staged and commitlint).

## Community discussion

If you are a member of this community, pass along your Discord ID to be invited to our dedicated room on the [Storybook Discord server](https://discord.gg/invite/storybook).
