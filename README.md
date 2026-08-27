# Dr. Zed public release repository

This repository is the public binary distribution boundary for Dr. Zed. Source code, provider
credentials, customer data, signing private keys, and development-only oracle files do not belong
here.

Phase 0 accepts and validates a signed-tag release request from
`faraz-shamim/drzed-rust`. It deliberately does not build or publish an application yet. The
production packaging, Windows signing, checksums, signed update metadata, and GitHub Release
publication workflow arrive in the dedicated release phase.

Production artifacts must be attached to immutable tagged GitHub Releases such as `v1.2.0`. Never
serve production binaries from a raw branch.
