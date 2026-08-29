# Changelog

All notable Chronlyt changes are documented here. The project follows [Semantic Versioning](https://semver.org/).

This file is a historical release record. Older entries describe the earlier fixed-feature productivity application and are not the current product definition. See the [README](README.md) for Chronlyt's plugin-based platform direction.

## [Unreleased]

### Added

### Changed

- Repositioned the public project and documentation around Chronlyt as a modular desktop platform whose functionality comes from plugins.
- Retired the old static website, screenshots and fixed-feature user guides.

### Fixed

### Security

## [0.2.1] - 2026-08-23

### Added

- Optional accounts with email/password, Google and Apple sign-in, email verification, password recovery and restart-safe sessions.
- Self-hosted PostgreSQL auth service with Argon2id, rotating opaque tokens, SMTP flows, persisted rate limits and OIDC verification.
- Settings → Account, optional account choice during onboarding and privacy-safe account network activity entries.

### Changed

### Fixed

### Security

- Account session secrets are kept in the operating-system credential store and excluded from React, SQLite, localStorage, logs, exports and backups.
- Desktop OAuth uses the system browser, PKCE S256, state/nonce verification and strict Tauri deep-link callbacks.

## [0.2.0] - 2026-08-23

### Added

- Official Tauri 2 signed updater with optional startup checks, manual checks, release notes and progress.
- Optional OpenAI-compatible AI Analysis with OS credential storage, exact payload preview and one-time consent.
- Independent offline Markdown and versioned JSON Data Export for arbitrary periods.
- About, What's New, privacy-safe diagnostics and a local Network Activity journal.
- Windows NSIS and Linux DEB, RPM and AppImage release targets with SHA-256 checksums.
- Product README, user documentation, issue forms and a static privacy-first landing page.
- Configurable Statistics workspace with global periods, equivalent-period comparisons, persisted drag/resize layout, metric definitions, details, charts and a focus heatmap.
- Indexed Rust/SQLite Statistics aggregation for Focus Sessions, Activities, Tasks, Goals, learning, health, content, finance, XP, streaks and recorded Rule Violations.
- Consent-based Background Mode and operating-system autostart choices in onboarding and Settings.
- Lightweight native tray controls and scheduling for Focus timers, enabled Activity Check-ins and notifications while the window is hidden.
- One-time Background/Autostart migration prompt for users who completed the earlier onboarding.

### Changed

- Renamed the product from Actumetry to Chronlyt throughout the application and data paths.
- Reorganized Settings into user-oriented categories and improved first-run onboarding.
- Synchronized application, Rust workspace and analytics sidecar versions.
- Dashboard and Statistics now share the reusable widget workspace while retaining independent persisted layouts.
- Manual launches open the main window; autostart launches may start hidden when the user enables Start Minimized.

### Fixed

- Update failures no longer expose raw technical errors as the primary user message.
- AI Analysis and Data Export no longer share workflows or imply network access for exports.
- Focus elapsed time and timer counts remain timestamp-backed and do not depend on renderer visibility, pause/resume cycles or recovery.
- Finance Statistics keep currencies separate and exclude opening balances from net change.

### Security

- API keys are stored in the operating-system credential store and excluded from SQLite, exports and backups.
- Update artifacts are verified using the public key embedded in Chronlyt; the private key remains outside Git.
- Background Mode and autostart do not enable additional tracking, AI, analytics or network access.
