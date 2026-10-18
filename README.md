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

The local checkout is intentionally named `chymeral-github` so it is easy to
find in a file browser. Its GitHub remote must be named exactly `.github`:

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

## Publishing

1. Create a **public** repository named `.github` under the `Chymeral`
   organization without adding GitHub-generated starter files.
2. Add that repository as the remote of this checkout.
3. Push its `main` branch.
4. In the organization settings, pin `chymeral` and `chymeral-rust-sdk` as
   featured repositories.

Repository-specific documentation and policies take precedence over these
defaults. Do not place application releases, SDK packages, source code, or
duplicated manuals here.
