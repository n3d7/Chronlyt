# Security Policy

## Supported versions

While Chronlyt is pre-stable, only the latest `0.x` release receives security fixes.

## Reporting a vulnerability

If you believe you have found a security vulnerability in Chronlyt, please use GitHub's private vulnerability reporting feature:

**Security → Report a vulnerability**

Do not open a public issue containing:

- vulnerability details that could enable exploitation;
- credentials, tokens or API keys;
- personal or behavioural data;
- private logs or database contents.

Security reports will be reviewed as soon as reasonably possible.

## Security model

Chronlyt is designed around a local-first security model.

- Personal behavioural data is stored locally by default.
- Chronlyt does not include developer telemetry or analytics SDKs.
- Sensitive credentials such as AI API keys and account session tokens are stored using operating-system credential facilities.
- Optional AI requests require explicit user configuration and consent.
- Backups and exports do not intentionally include authentication secrets or API keys.
- Application updates use cryptographic verification before installation.
- Diagnostics are designed to exclude user content and credentials.

Because backups and exports may contain personal behavioural information, users should protect them appropriately and use encrypted storage where necessary.

## Closed-source application

The public `n3d7/Chronlyt` repository contains product documentation, release information and public project resources.

The application source code is maintained separately and is not published in this repository.