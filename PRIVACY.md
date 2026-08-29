# Chronlyt Privacy

Chronlyt is designed around local-first, privacy-conscious operation. It is also becoming a modular platform, so privacy must be understood at two levels: the Chronlyt base application and the plugins added to it.

## Scope

This document describes the privacy direction and currently documented behavior of the Chronlyt base application. It does not make blanket promises for every plugin.

Plugins can introduce their own data, storage, account, integration, or network requirements. Review the documentation and provenance of a plugin before using it. When plugin-specific information is available, it takes precedence for that plugin's behavior.

## Base application principles

Chronlyt's core is designed to work locally and without turning personal application data into a developer dataset.

The base application does not include developer analytics, third-party analytics SDKs, or automatic crash-report uploads. It does not automatically upload local user data as a general synchronization service.

Current releases store structured application data locally. Sensitive credentials used by supported core features are designed to remain in operating-system credential facilities rather than ordinary application data, logs, exports, or backups.

## Network activity

Some Chronlyt operations can require network access, including update checks, account operations, configured integrations, or other functionality explicitly used by the user. Plugins may add different network behavior.

The destination service processes information according to its own terms and privacy policy. Before enabling networked functionality, review what it sends, where it sends it, and whether that behavior is appropriate for you.

## Releases and updates

Chronlyt releases are distributed through [GitHub Releases](https://github.com/n3d7/Chronlyt/releases). Release packages may include signatures, checksums, and update metadata. Follow the verification guidance supplied with the release you install.

## Your responsibility when adding plugins

Adding a plugin changes what Chronlyt can do and may change what information it handles. Do not assume that a plugin inherits every privacy property of the base application unless its documentation says so.

Use plugins only when you trust their source or publisher and understand their requested data and network behavior.

## Source code and repositories

Chronlyt is a closed-source application. The public [n3d7/Chronlyt](https://github.com/n3d7/Chronlyt) repository contains documentation, release information, issue tracking, and other public project resources.

Plugin development is organized separately in [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins). The Chronlyt application source code is maintained separately and is not published in this repository.
