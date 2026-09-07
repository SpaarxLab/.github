# SpaarxLab GitHub defaults

This public repository provides the SpaarxLab organization profile and
public-safe contribution, support, security, issue, and pull-request defaults.

Repository-specific instructions override these defaults. Internal company
state, customer material, credentials, and protected partner source do not
belong here.

## Edit these defaults

This is a Markdown and GitHub-template repository. Install Git; no runtime,
package installation, database, Docker, or environment file is required.

```bash
git clone https://github.com/SpaarxLab/.github.git
cd .github
git switch -c docs/improve-contribution-guide
```

Edit `profile/README.md` for the public organization profile, the root guides
for contribution/support/security defaults, or `.github/` for issue and PR
templates. Preview Markdown on GitHub, check links and YAML syntax when editing
templates, and run `git diff --check`. Submit a PR as described in
[CONTRIBUTING.md](CONTRIBUTING.md). Profile visibility must be checked on GitHub
after merge; a local Markdown preview does not prove organization display.

Everything in this repository is public. Keep internal onboarding details in
the team's private documentation. There are no required secrets or seed data.
