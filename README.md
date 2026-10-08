# TrustOps AI

This repository contains the **repository base** for the TrustOps AI project, including the planned directories, contribution guidance, and secret scanning. The approved repository architecture document defines the planned files, ownership, and dependency rules. `.gitkeep` files allow Git to retain empty directories.

No application source, application tests, infrastructure configuration, datasets, or scenarios have been implemented yet. Add each file together with its feature when work begins. See [ARCHITECTURE.md](ARCHITECTURE.md) for the planned module boundaries.

The Security workflow scans Git history for secrets on pull requests and pushes to `main` and `dev`. Dependabot proposes weekly GitHub Actions updates to `main`. Application CI will be added with the code it validates. See [SECURITY.md](SECURITY.md) for scanner maintenance.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the task-branch and pull-request workflow.
