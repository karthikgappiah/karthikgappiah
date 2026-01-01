# Contributing

This document gives the rules for changes to this repository. Obey all of the rules.

## Repository contents

This repository is a GitHub profile repository. GitHub shows `README.md` on the profile page of the owner.

| File | Purpose |
| --- | --- |
| `README.md` | The public profile page. |
| `CONTRIBUTING.md` | The rules for contributors. |
| `AGENTS.md` | The instructions for AI agents. |
| `CLAUDE.md` | A symbolic link to `AGENTS.md`. |

The repository has no code, no build, and no tests.

## Workflow

1. Make a branch from the default branch.
2. Make one change.
3. Commit the change.
4. Push the branch.
5. Open a pull request.

## Atomic changes

Each issue, commit, and pull request must have one purpose only. Do not combine unrelated changes. If you have two unrelated changes, make two commits and two pull requests.

## Branch names

Use this format for all branch names:

```text
type/short-description
```

- Use a Conventional Commits type for `type`. Examples: `feat`, `fix`, `docs`, `chore`.
- Use lowercase words with hyphens for `short-description`.

Examples:

```text
feat/add-project-section
fix/correct-case-study-link
docs/update-contributor-guide
```

## Conventional Commits

Use the multiline [Conventional Commits](https://www.conventionalcommits.org/) format for all:

- Issue titles and descriptions.
- Commit messages.
- Pull request titles and descriptions.

The format has three parts:

1. A header: `type(optional-scope): description`.
2. A blank line.
3. A short body. The body tells what changed and why.

For an issue or a pull request, the title is the header. The description is the body.

Example:

```text
fix(readme): correct the Taggato case study link

The link went to the wrong case study page. Change the link to the
correct page.
```

## Signed commits

Sign every commit. Unsigned commits are not permitted.

To sign all commits automatically, set this configuration:

```sh
git config commit.gpgsign true
```

To sign one commit, use the `-S` option:

```sh
git commit -S
```

GitHub must show the commit as "Verified". Add your signing key to your GitHub account.

## Authored-By trailer

Add one `Authored-By` trailer to every commit. Use the values of your Git `user.name` and `user.email`. Do not add other attribution trailers. For example, do not add `Co-Authored-By` or `Signed-off-by`.

Example:

```text
Authored-By: Jane Doe <jane@example.com>
```

To add the trailer from your Git configuration, use this command:

```sh
git commit -S --trailer "Authored-By: $(git config user.name) <$(git config user.email)>"
```

## Documentation

Update the documentation in the same pull request when you change:

- The behavior of the project.
- The setup instructions.
- The contributor workflow.

Make sure that the documentation agrees with the current repository.

## Language

Write in [ASD-STE100 Simplified Technical English](https://www.asd-ste100.org/). This rule applies to:

- All technical documentation, for example `CONTRIBUTING.md` and `AGENTS.md`.
- All issue, commit, and pull request text.

Follow these guidelines:

- Write short sentences. Use a maximum of 20 words in an instruction.
- Use common words. Use one word for one meaning.
- Use the active voice.
- Write instructions as commands. Start with the verb.
- Write one instruction in each sentence.
