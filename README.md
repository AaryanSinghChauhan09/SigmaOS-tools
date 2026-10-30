# SigmaOS tools

System tools and utilities for the SigmaOS project. The crate manifest and
`src/tools/` tree define the current component API and implementation. The
component contract also assigns this repository responsibility for installer,
ISO generation, updates, rollback, packaging, and reproducible CI tooling; those
areas remain subject to integration evidence and are not implied complete here.

## Development

Use the Rust toolchain declared by `Cargo.toml`. Run `cargo check` and the
available crate tests before proposing implementation changes. Keep upstream
behavior and system-level risks explicit in changes, and include a rollback
path when a change affects installation or system state.

## Component status

This repository contains implementation code. Its integration and release
readiness must be evaluated against the owning SigmaOS repository's checks;
the presence of code alone does not establish production readiness.
