# Architecture — Elyne Refactor

[Français](architecture.md) · [Overview](../README.en.md)

## Simplified flow

Authorized repository → static analysis and context → model proposals → comparison and checks → report for human review.

## Components and boundaries

- The advertised pipeline combines a work sandbox, deterministic analysis, document retrieval, and comparison of proposals from several local models.
- Outputs may include patches and structured reports. Signing an artifact can attest its provenance; it does not by itself prove that a patch is correct.
- Local deployment and network isolation are architectural goals. CLI, API, IDE, and CI integrations depend on the installed version and profile.

This textual flow describes the product architecture. It does not replace verification on a specific build, hardware profile, and configuration. The [evidence summary](evidence.en.md) states what is actually documented.
