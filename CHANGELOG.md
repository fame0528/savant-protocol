# Changelog

All notable changes to this project are documented here automatically by the
agent when a FID reaches **Closed** status. Entries are added in reverse
chronological order (newest first).

Format: Each entry includes the FID ID, severity, a brief description, and the
resolution summary.

---

## v0.0.1 — 2026-06-01

Initial boilerplate release.

### Added

- Tiered activation: Core (Laws 1-4 always active) + Extended (Laws 5-15, configurable via `strict_mode`)
- Quality overrides per-language in coding-standards (TS: 400 lines, Python: 400/120, Go: 350/120, Java: 350/40/120, C#: 350/120)
- Honest Assessment nuance: verified claims need proof, design decisions need reasoning
- Language stubs: Go, Java, C# coding standards with naming conventions and patterns
- CHANGE_ME boot check: agent halts if language is not configured
- README quickstart hook: 30-second value prop above the fold
- MIGRATION.md: retrofit guide for existing projects with checklist
- Go, Java, C# badges in README
- ECHO Protocol v0.0.1 — universal agent bootstrap (15 Laws, Five Questions, Perfection Loop FSM)
- Language-agnostic configuration via `protocol.config.yaml`
- Coding standards for Rust, TypeScript, and Python
- FID (Feature Implementation Document) lifecycle with auto-archive to `dev/fids/archive/`
- Auto-changelog updates on FID closure
- Session lifecycle management with auto-generated summaries
- Circuit breaker rules (Levenshtein change control, oscillation detection, hard stop)
- Anti-patterns and emergency procedures
- Autonomy levels (Guided, Supervised, Autonomous)
- Starter prompts for universal and language-specific agent activation
- VERSION file for protocol version tracking
- CHANGELOG.md for automated change documentation

<!-- Agent entries are added below this line -->
