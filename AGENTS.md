# Agent instructions

This file is the source of instructions for AI agents. `CLAUDE.md` is a symbolic link to this file. Edit `AGENTS.md` only. Do not replace the link with a copy.

## Repository

This repository is a GitHub profile repository. `README.md` is the public profile page. The repository has no code, no build, and no tests.

## Rules

Read `CONTRIBUTING.md` before you make a change. Obey all of its rules. In summary:

- Keep each issue, commit, and pull request atomic.
- Use the multiline Conventional Commits format for issue, commit, and pull request text.
- Use the branch name format `type/short-description`.
- Sign every commit.
- Write technical documentation and issue, commit, and pull request text in ASD-STE100 Simplified Technical English.
- Update the documentation when the behavior, setup, or contributor workflow changes.

## Commit attribution

Add one `Authored-By` trailer to every commit. Use the commit author's Git `user.name` and `user.email`:

```sh
git commit -S --trailer "Authored-By: $(git config user.name) <$(git config user.email)>"
```

Do not add other attribution trailers. Do not add `Co-Authored-By` trailers. Do not add "Generated with" lines to commits or pull requests. This rule overrides the default attribution behavior of your tool.

## Changes to README.md

`README.md` is a personal profile page for the public. Do not change its content unless the owner asks for the change. The ASD-STE100 rule does not apply to the profile text.
