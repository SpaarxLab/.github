# Contributing to SpaarxLab repositories

Thank you for helping improve SpaarxLab work.

## Before starting

1. Read the target repository's README and current-state file.
2. Confirm that the issue or requested outcome is still current.
3. Use a focused branch and keep the change bounded to one outcome.
4. Never add credentials, customer data, employee data, private company
   material, or source from a repository you do not have permission to use.

## Pull requests

A useful pull request explains:

- the outcome it changes;
- the authority or issue behind the change;
- what was verified and how;
- privacy, security, data, migration, deployment, or compatibility impact;
- what remains unverified;
- the rollback or recovery path when the change is consequential.

Passing tests do not by themselves prove deployment, customer use, safety, or
commercial value. Keep claims at the level the evidence supports.

Repository-specific contribution instructions and approval requirements always
take precedence over this default.

## Clone, fork, and branch

Clone the target repo when you have write access, or use GitHub's Fork button
when permitted. In a fork, `origin` should be your fork and `upstream` the
original repository:

```bash
# Replace OWNER and REPO with the repository you are contributing to.
git clone https://github.com/OWNER/REPO.git
cd REPO
# Fork contributors only: replace UPSTREAM_OWNER with the original owner.
git remote add upstream https://github.com/UPSTREAM_OWNER/REPO.git
git fetch upstream
git remote show upstream
```

For a shared clone, use `origin` instead of `upstream` in fetch/show commands
and do not add a second remote. Check `HEAD branch` in the output; branch
names vary. Create a feature branch from that remote's default branch, make
your change, run the target repo's documented checks, inspect `git diff`, and
commit only intended files. Push the feature branch to `origin` and open a PR
against the original repository's default branch. Do not change repository
visibility to work around a private-fork restriction.

When setup fails, include the OS, runtime version, repo commit, command, and
redacted error. Never attach an entire environment file. Improvements to setup
should update the target README and its safe configuration example together.
