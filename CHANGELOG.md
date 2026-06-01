# Changelog

All notable changes to this project are documented here automatically by the
agent when a FID reaches **Closed** status. Entries are added in reverse
chronological order (newest first).

Format: Each entry includes the version, date, and changes.

**Version source of truth:** `VERSION` file at project root. All other files
(protocol.config.yaml, ECHO.md, README.md, STARTER-PROMPT.md) should match.
When bumping, update `VERSION` first, then propagate.

**Version history note:** This project was forked from Savant's internal ECHO
Protocol (formerly v4.0.0). The version was reset to v0.0.1 for the public
boilerplate release to reflect independent versioning.

---

## v0.0.3 — 2026-06-01

### Fixed (HIGH)

- README.md clarifies ECHO.md as the single source of truth (protocol spec vs landing page)
- Go, Java, C# starter prompts added to STARTER-PROMPT.md
- Law 3 vs Emergency Procedure contradiction resolved — emergency procedures are escape hatches requiring FID + documentation

### Fixed (MEDIUM)

- "Final Certification" mapped to COMPLETE state in termination criteria
- `strict_mode: false` behavior documented (Core enforced, Extended advisory, circuit breakers still apply)
- Quality override precedence: language override wins over config defaults
- Law 6 and Anti-Patterns now include language-specific type safety shortcuts for all 6 languages
- Circuit Breaker #2 (500-char sample) fully specified: random selection, exact match, revert on unintended changes
- Savant vs ECHO naming relationship explained in README footer

### Fixed (LOW)

- Version source of truth documented in CHANGELOG header (`VERSION` file is canonical)
- Version reset from Savant v4.0.0 acknowledged in CHANGELOG
- Law 8 "log intent" destination specified (session summary)
- Universal starter prompt aligned to 8 boot steps (matches language variants)
- LEARNINGS.md date format corrected to YYYY-MM-DD-HHMM (consistent with SESSION-SUMMARY)
- FID filename convention added to template (`FID-YYYY-MMDD-NNN-[short-description].md`)
- Quickstart notes dev/ directories are gitignored and auto-created at runtime

## v0.0.2 — 2026-06-01

- Tiered activation: Core (Laws 1-4 always active) + Extended (Laws 5-15, configurable via `strict_mode`)
- Quality overrides per-language in coding-standards (TS: 400 lines, Python: 400/120, Go: 350/120, Java: 350/40/120, C#: 350/120)
- Honest Assessment nuance: verified claims need proof, design decisions need reasoning
- Language standards: Go, Java, C# coding standards with naming conventions and patterns
- CHANGE_ME boot check: agent halts if language is not configured
- README quickstart hook: 30-second value prop above the fold
- MIGRATION.md: retrofit guide for existing projects with checklist
- Go, Java, C# badges in README

## v0.0.1 — 2026-06-01

Initial boilerplate release.

- ECHO Protocol — universal agent bootstrap (15 Laws, Five Questions, Perfection Loop FSM)
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
