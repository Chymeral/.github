# Chymeral Organization Metadata

This repository provides the public organization profile and the shared GitHub
community defaults for [Chymeral](https://github.com/Chymeral).

It contains no Chymeral runtime code and no SDK implementation. Product code,
release artifacts, protocol documentation, and technical validation remain in
their respective repositories.

## Purpose

GitHub renders `profile/README.md` from a public repository named `.github` as
the organization profile. The files at this repository root provide sensible
defaults for future Chymeral repositories when they do not define a more
specific policy themselves.

The local checkout name is not significant. The GitHub repository name must be
exactly `.github`:

```text
https://github.com/Chymeral/.github
```

## Contents

| Path | Role |
| --- | --- |
| `profile/README.md` | Public landing page shown on the Chymeral organization profile. |
| `ISSUE_TEMPLATE/` | Default bug-report and feature-request forms. |
| `CONTRIBUTING.md` | Cross-repository contribution baseline. |
| `PULL_REQUEST_TEMPLATE.md` | Review checklist for repositories that do not define their own template. |
| `CODE_OF_CONDUCT.md` | Expected public-community behavior and reporting guidance. |
| `SECURITY.md` | Default security-reporting policy for future repositories. |
| `SUPPORT.md` | Routes for support, bug reports, and feature proposals. |

## Maintenance

This repository is public at <https://github.com/Chymeral/.github>. Keep its
profile and shared defaults aligned with the released Chymeral ecosystem.

1. Keep `profile/README.md` focused on the organization, ecosystem map, stable
   versions, and canonical entry points.
2. Keep repository-specific technical guidance in the repository that owns it.
3. In the organization settings, pin `chymeral` and `chymeral-rust-sdk` as
   featured repositories.

Repository-specific documentation and policies take precedence over these
defaults. Do not place application releases, SDK packages, source code, or
duplicated manuals here.
