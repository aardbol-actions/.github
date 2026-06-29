# aardbol-actions

The **aardbol-actions** organization hosts shared GitHub Actions and npm packages
for container image and CI/CD development.

## Repositories

- **[common](https://github.com/aardbol-actions/common)** — Shared Actions and config files:
  `action-io-generator`, `bundle-verifier`, `commit-data`, plus shared ESLint, TypeScript,
  and Webpack configs.

## Security

This organization applies the following measures across all repositories:

- **Security policy** — `SECURITY.md` directs reporters to GitHub's Private vulnerability
  reporting tool; acknowledgment within 72 hours.
- **Code scanning (CodeQL)** — Analyzes JavaScript/TypeScript code on every push/PR
  to `main` and weekly.
- **Vulnerability scanning (Trivy)** — Filesystem scan for npm dependency CVEs on
  every push/PR and weekly.
- **Dependabot alerts** — Monitors npm and GitHub Actions dependencies daily;
  grouped PRs for `@actions/*`, `@types/*`, and ESLint packages.
- **Secret scanning** — Enabled org-wide with push protection.
- **Branch protection** — `main` requires passing status checks (lint, test, bundle
  verification, CodeQL, Trivy) and pull request review before merge.
- **Action pinning** — All GitHub Actions pinned by commit SHA with a human-readable
  version comment.
- **OpenSSF Scorecards** — Weekly supply-chain security evaluation.
- **Link checking** — Lychee validates all markdown links on every push/PR.
