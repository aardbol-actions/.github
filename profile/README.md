# aardbol-actions

The purpose of the **aardbol-actions** organization is to provide a collection of reusable GitHub Actions with recent dependencies and hardened security. The main focus is on forking and improving existing actions that have been abondened upstream or hardly maintained.

## Repositories

- **[common](https://github.com/aardbol-actions/common)** — Shared Actions and config files: `action-io-generator`, `bundle-verifier`, `commit-data`, eslint/ts/webpack configs
- **[buildah-build](https://github.com/aardbol-actions/buildah-build)** — Buildah-based container image build action

## Security

This organization applies the following measures across all repositories:

- **Security policy** — `SECURITY.md` directs reporters to GitHub's Private vulnerability reporting tool.
- **Code scanning (CodeQL)** — Analyzes JavaScript/TypeScript code on every push/PR to `main` and weekly.
- **Dependabot alerts** — Monitors npm and GitHub Actions dependencies daily; grouped PRs.
- **Secret scanning** — Enabled org-wide with push protection.
- **Branch protection** — `main` requires passing status checks and pull request review.
- **Action pinning** — All GitHub Actions pinned by commit SHA with version comments.
- **Container scanning (Trivy)** — Filesystem vulnerability scan on every push/PR and weekly.
- **OpenSSF Scorecards** — Weekly supply-chain security evaluation.