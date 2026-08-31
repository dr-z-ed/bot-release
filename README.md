# Dr. Zed public release repository

This repository is the public binary distribution boundary for Dr. Zed. Source code, provider
credentials, customer data, signing private keys, and development-only reference files do not belong
here.

Production releases are built and signed only by the protected release workflow in
`faraz-shamim/drzed-rust`. That workflow creates a draft here, attaches the Windows ZIP, SHA-256
file, and source-identity manifest, verifies the complete draft, and then publishes it. This public
repository never receives source code or signing credentials. Its verification workflow checks the
published files again without holding a secret.

Production artifacts must be attached to immutable tagged GitHub Releases such as `v1.2.0`. Never
serve production binaries from a raw branch.
