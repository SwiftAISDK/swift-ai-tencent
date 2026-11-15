# Changelog

## 1.0.0

- Add Tencent TokenHub chat/streaming and Kling video, plus TC3-signed Tencent Cloud VOD start/status operations with independent lazy credentials. Preserve current media options, billing/error metadata, cancellation and per-file MOV/MP4/WebM media types. Translate all portable 3.0.3 matching-release scenarios and published TC3 signature vectors. Validation passed: node Scripts/test-packages.mjs (55 owning packages, 2451 owning tests and 1736 compatibility tests), generation checks, 27 tooling tests, isolation/version checks, deterministic exports and minimum-dependency consumers. Documentation check/build passed (104 pages). Publication is gated by exact-source Swift 6.3.3 CI; subsequent public refs and clients are recorded in Docs/ReleaseVerification20261115.json. Paid/live-service checks were not run; this delta does not claim full-package parity.
  Compatibility: Initial independent SwiftPM package 1.0.0. Requires swift-ai-core 1.5.0, swift-ai-openai-compatible 1.2.1. Existing package selectors remain unchanged. JavaScript workflow/lifecycle-only exclusions and native representation differences are documented.
