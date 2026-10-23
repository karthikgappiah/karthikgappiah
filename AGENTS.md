Use Conventional Commits for every commit:

- Subject: a type, optional scope in parentheses, colon, and brief summary.
- Body: explain what changed and why.
- Trailer: `Authored-By: Name <email>`
- Separate the subject, body, and trailer with blank lines.

Example:
```text
docs: add empty README

Create an empty README.md to initialize the profile repository.

Authored-By: Karthik G. Appiah <122487930+karthikgappiah@users.noreply.github.com>
```

Each issue, commit, and pull request must address **one coherent purpose**. Never group unrelated changes together, regardless of size.

- **Scope:** Include only changes strictly required for the stated purpose, plus directly related tests and documentation.
- **Separation:** Put unrelated fixes, refactors, formatting, and cleanups into separate issues, commits, and PRs. 
- **PR Scope:** Splitting unrelated changes into separate commits within the same pull request is not sufficient. Each PR must have a single purpose.
- **Scope Creep:** If work reveals an unrelated problem, create a new tracking issue rather than expanding the current scope.
- **Rationale:** This ensures clean git history, easy code reviews, safe rollbacks, and precise automated changelogs.
