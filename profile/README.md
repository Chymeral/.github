<p align="center">
  <img src="https://raw.githubusercontent.com/Chymeral/chymeral/main/branding/chymeral_logo.svg" alt="Chymeral logo" width="360">
</p>

# Chymeral

> Pronounced **Kímeral**.

Chymeral is a minimalist terminal emulator with a reusable local 2D graphics
runtime for applications compatible with the **Chymeral Link Protocol (CLP)**.

It preserves the conventional terminal model: programs remain ordinary
binaries or launchers with `stdin`, `stdout`, `stderr`, arguments, and exit
codes. A CLP-aware program may additionally render a local scene and receive
runtime events from the Chymeral window that launched it.

## Ecosystem

| Project | Purpose | Current stable line |
| --- | --- | --- |
| [Chymeral](https://github.com/Chymeral/chymeral) | Terminal application, local graphics runtime, and CLP host. | `1.0.0` |
| [Chymeral Rust SDK](https://github.com/Chymeral/chymeral-rust-sdk) | Reference Rust client library for the language-neutral CLP contract. | `1.0.0` |

The Rust SDK is available on [crates.io](https://crates.io/crates/chymeral-rust-sdk)
with generated API documentation on
[docs.rs](https://docs.rs/chymeral-rust-sdk/1.0.0/chymeral_rust_sdk/).

## Downloads

The [latest Chymeral release](https://github.com/Chymeral/chymeral/releases/latest)
provides portable Linux x86_64 and Windows x86_64 editions. Extract the matching
archive and launch `Launch Chymeral.sh` on Linux or `Launch Chymeral.cmd` on
Windows; no installation is required. The Linux launcher explicitly selects X11,
so a Wayland desktop needs Xwayland and `DISPLAY` available.

## Design

- One window, two complementary surfaces: a PTY-backed ANSI/VT terminal grid
  and an opt-in retained 2D scene.
- CLP is local, private to each Chymeral window, and neutral between programming
  languages.
- SDKs are client libraries, not host-loaded plugins. Rust has no privileged
  path; future language bindings share the same protocol contract.
- The runtime targets Linux and Windows. macOS is intentionally outside the
  current scope.
- Chymeral is not a widget toolkit, mod system, global graphics service, or a
  replacement for application logic, physics, or input policy.

## Start Here

- Read the [Chymeral README](https://github.com/Chymeral/chymeral#readme) and
  [Main Manual](https://github.com/Chymeral/chymeral/blob/main/Main_Manual.md)
  to build, configure, and run the terminal.
- Read the [Rust SDK README](https://github.com/Chymeral/chymeral-rust-sdk#readme)
  to build a CLP client in Rust.
- Read the [CLP concepts in the Main Manual](https://github.com/Chymeral/chymeral/blob/main/Main_Manual.md)
  before implementing a client in another language.

## Contributing and Support

Please use the issue tracker of the repository that owns the problem or
proposal. Read the relevant repository's contributing guide before opening a
pull request. Security issues must never be reported through public issues;
follow the applicable [security policy](https://github.com/Chymeral/chymeral/blob/main/SECURITY.md).

Chymeral is available under the [MIT License](https://github.com/Chymeral/chymeral/blob/main/LICENSE).
