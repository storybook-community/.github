# Inviting new contributors

This is an outline of the workflow for inviting new contributors to maintain a new addon fork.

## General procedure

1. Meet contributor and explain how the community works ([team structure](https://github.com/storybook-community/.github/blob/main/profile/CONTRIBUTE.md))
2. Make sure contributor is aware of, and will abide by
   * [Code of conduct](https://github.com/storybook-community/.github/blob/main/profile/CODE_OF_CONDUCT.md)
   * [Safety procedures](https://github.com/storybook-community/.github/blob/main/profile/SAFETY.md)
3. Invite contributor
   * Go to https://github.com/orgs/storybook-community/people
   * Give the [Community contributors](https://github.com/orgs/storybook-community/teams/community-contributors) role to externals, and [Trusted contributors](https://github.com/orgs/storybook-community/teams/trusted-contributors) role to folks already vetted by Storybook
   * Tell contributor to ensure they have a GPG key set up for commit signing, and 2FA enabled
4. Fork contributor's addon repo
   * Fork `main` branch
   * Completely block pushes to `main` for now (make PRs mandatory and PR approval mandatory, forbid self approval)
   * Ensure tags have been pushed
5. Give contributor individual access to that specific repo as a maintainer
6. Start a `setup` branch, ask contributor to:
   * Add CI/CD workflows from e.g. https://github.com/storybook-community/storybook-source-link/tree/main/.github
   * Align script names in `package.json` to match CI/CD workflows and other repos
   * Review addon metadata (help them if needed)
   * Prefix package name with `@storybook-community/` (unless package ownership was transferred on NPM)
   * Make sure the version in package.json matches the current release
   * Edit README to include thank you note for original addon author
   * Open PR
7. Review contributor PR, and once all good, give contributor full maintain rights on their repo
8. Merge PR and verify first version published successfully
9. Start communication campaign on the addon
10. Encourage contributor to modernise addon in a follow-up issue
    * Tooling updates
    * Realign code structure and tsup config on https://github.com/storybookjs/addon-kit
 
## Ownership transfers

When a package's ownership is transferred to us, we don't rename it in `package.json`.
