# Contributing to CRISP-lang Foundation

Thank you for your interest in contributing to CRISP! We welcome contributions of all sizes from people with all levels of experience. This document explains how to get started, what we expect from contributors, and how we review and accept changes.

Quick links
- Repository: https://github.com/CRISP-lang-foundation/CRISP-lang
- Org-wide community files: https://github.com/CRISP-lang-foundation/.github

1. Code of conduct
Please follow our Code of Conduct (CODE_OF_CONDUCT.md) in all interactions. Be respectful, patient, and helpful.

2. Get the code
1. Fork the repo you want to work on (for example, CRISP-lang) and clone your fork:

```bash
# fork -> then
git clone https://github.com/<your-username>/CRISP-lang.git
cd CRISP-lang
```

2. Add the upstream remote and keep your fork up to date:

```bash
git remote add upstream https://github.com/CRISP-lang-foundation/CRISP-lang.git
git fetch upstream
git checkout main
git merge upstream/main
```

3. Set up your dev environment
- We try to keep the dev setup simple. See each repository's README or docs/dev-setup.md for repo-specific instructions.
- Typical steps:
  - Install Rust (https://www.rust-lang.org/tools/install) and the toolchain from rustup
  - Install the required system packages for your OS (see repo README)

4. Build and run tests
- Build the project:

```bash
# example for Rust-based CRISP-lang
cargo build
```

- Run tests:

```bash
cargo test
```

If tests fail locally, include failing output in your PR and explain what you tried.

5. Branching and commits
- Create a feature branch for each logical change:

```bash
git checkout -b feature/short-description
```

- Keep commits focused and atomic. Use clear commit messages. Follow this template for commit messages:

```
Short summary (50 chars or less)

More detailed description (wrap at ~72 chars). Explain why the change was made.

Fixes: #<issue-number>   # when applicable
```

6. Issues
- Search existing issues before opening a new one. If the issue is new, create a clear issue with:
  - Problem description
  - Steps to reproduce (if applicable)
  - Expected vs actual behavior
  - Environment (OS, Rust version, platform)

- Use these labels (if available): `good-first-issue`, `help wanted`, `bug`, `enhancement`, `documentation`.

7. Pull requests
- Push your branch to your fork and open a Pull Request (PR) against the target repo's default branch (usually `main`).
- In your PR description include:
  - What the change does and why
  - How to test the change
  - Any relevant screenshots or logs
  - Link to related issues (e.g., `Fixes #123`)

PR checklist (add to PR description):
- [ ] I have run the tests locally
- [ ] I followed the coding style and added/updated docs
- [ ] My commit messages are clear
- [ ] This change is covered by tests where applicable

8. Code style and review
- Respect existing coding style in each repository.
- For Rust code, format with `cargo fmt` and check with `cargo clippy` when possible.
- Maintain backwards-compatibility where reasonable and document breaking changes.

9. Documentation
- Keep documentation close to the code. Update README or docs/ when behavior changes.
- For the CRISP book or larger docs, follow the repo's style and build instructions.

10. Asking for help
- Use GitHub Discussions (when enabled) for general questions and design conversations.
- Use Issues for bug reports and feature requests.
- If you need real-time help, include a note in the issue or discussion and a maintainer may offer a short pairing session.

11. Security issues
- Do NOT open public issues for security vulnerabilities. Instead, contact the maintainers privately (see org members or the security policy if available).

12. Maintainers and review process
- We aim to respond to issues and PRs within a few business days. Response times may vary — maintainers are volunteers.
- PRs will be reviewed by one or more maintainers. You may be asked to make changes; please push additional commits to the same branch.

13. New contributor tips
- Look for issues labeled `good-first-issue` or `help wanted`.
- Start small: fix a typo, improve docs, or add a test.
- Ask for help on the issue if you get stuck — we prefer small, incremental changes.

14. Licensing and copyright
- By contributing, you agree that your contributions will be distributed under the repository's existing license.

Thanks again for contributing — we appreciate your time and help in growing CRISP!
