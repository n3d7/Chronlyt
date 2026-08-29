# Security Policy

## Supported versions

While Chronlyt is pre-stable, only the latest `0.x` release receives security fixes.

## Reporting a vulnerability

If you believe you have found a security vulnerability in Chronlyt, use GitHub's private vulnerability reporting feature:

**Security → Report a vulnerability**

Do not open a public issue containing:

- details that could enable exploitation;
- credentials, tokens, or API keys;
- personal data;
- private logs, databases, exports, or configuration files.

If you are unsure whether a problem belongs to the Chronlyt core or a plugin, report it privately and identify the plugin and version involved when possible.

## Platform and plugin scope

Chronlyt is becoming a modular desktop platform. The base application and installed plugins can have different trust boundaries, data access, and network behavior.

The documented core security model includes local-first storage, operating-system credential facilities for supported sensitive credentials, and cryptographic verification for application updates. The base application does not include developer telemetry or third-party analytics SDKs.

These statements do not automatically apply to every plugin. Review a plugin's documentation, provenance, dependencies, data handling, and network behavior before using it. No undocumented plugin sandbox, permission model, API guarantee, or compatibility boundary is implied here.

## Closed-source application

The public [n3d7/Chronlyt](https://github.com/n3d7/Chronlyt) repository contains documentation, release information, issue tracking, and public project resources for the base application.

The Chronlyt application source code is maintained separately and is not published in this repository. Plugin development is organized in [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins).
