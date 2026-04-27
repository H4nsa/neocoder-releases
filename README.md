# NeoCoder Releases

Binary-only public distribution repository for NeoCoder.

The NeoCoder source repository is private. This repository is used only for GitHub Releases assets such as installer scripts, platform bundles, `SHA256SUMS`, and optional signatures. It must not contain Rust source code, Cargo manifests, private CI logs, internal URLs, credentials, or source archives.

NeoCoder is not affiliated with, endorsed by, or sponsored by OpenAI. Public release archives must not contain top-level `codex` or `codex-*` executables. Internal Cargo binaries are staged under NeoCoder names before publishing.

Default public binaries:

- `neocoder`
- `neocoder-runtime`
- `neocoder-app-server`
- `neocoder-auth-token`
- `neocoder-mcp-server`
- `neocoder-neoflow-proxy`

Installers and self-update default to this repository:

```bash
curl -fsSL https://github.com/H4nsa/neocoder-releases/releases/download/neocoder-v0.1.0/install.sh | sh
```

Every release must include `SHA256SUMS`. Installers and `neocoder self-update` fail closed when checksums are missing or mismatched.
