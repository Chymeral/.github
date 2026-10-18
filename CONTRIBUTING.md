# Contributing to Chymeral

Thank you for helping improve the Chymeral ecosystem. This repository defines
organization-wide defaults. The contributing guide in the repository you are
changing always takes precedence, especially for build commands, supported
platforms, protocol compatibility, and release processes.

## Choose the right repository

- Report terminal, renderer, CLP-host, or desktop-integration issues in
  [`chymeral`](https://github.com/Chymeral/chymeral).
- Report Rust client-library and Rust conformance issues in
  [`chymeral-rust-sdk`](https://github.com/Chymeral/chymeral-rust-sdk).
- Propose language-neutral CLP contract changes in the core repository before
  implementing them in any SDK.

## Before opening an issue

- Search existing issues and documentation first.
- Use a concise, reproducible report with version, platform, and expected and
  actual behavior.
- Keep security concerns out of public issues; use the repository's security
  policy instead.
- Make clear whether the issue affects Linux, Windows, or both.

## Before opening a pull request

- Keep the change focused on one problem.
- Follow the target repository's formatting, test, documentation, and manual
  validation requirements.
- Explain public API, protocol, compatibility, and platform implications.
- Do not add language-specific behavior to CLP unless it can be represented by
  every conforming client.
- Do not commit generated binaries, local configuration, credentials, or
  unrelated formatting changes.

## Working language

English is the working language for public documentation, source code, issue
reports, and review discussion so that the ecosystem remains accessible to
contributors across platforms and languages.

## Community expectations

All participation is subject to the [Code of Conduct](CODE_OF_CONDUCT.md).
