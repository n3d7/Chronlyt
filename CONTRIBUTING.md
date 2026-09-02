# Contributing to Chronlyt

Chronlyt's application core is proprietary and closed-source. The core source is maintained separately and is not published in this repository, so outside pull requests to the application core cannot be accepted here.

There are still several useful ways to contribute.

## Report a bug

Use the [bug-report form](https://github.com/n3d7/Chronlyt/issues/new?template=bug_report.yml) for reproducible application problems. Include the Chronlyt version, operating system, installation format, and clear reproduction steps.

Do not attach credentials, personal data, databases, private exports, or unreviewed logs. Security vulnerabilities must be [reported privately](SECURITY.md).

## Suggest an improvement

Use the [feature-request form](https://github.com/n3d7/Chronlyt/issues/new?template=feature_request.yml) to describe the user problem and desired behaviour. Plugin ideas and plugin-system proposals may belong in [Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins); check its current contribution guidance first.

## Improve public documentation

Documentation fixes and focused improvements are welcome in this repository. Keep claims consistent with released behaviour, avoid promises about unfinished features, and link to release notes when availability varies by version.

Start with the [user documentation](docs/user/README.md), [Privacy document](PRIVACY.md), and [Security Policy](SECURITY.md). Keep documentation pull requests small enough to review and explain what user-facing confusion they resolve.

## Report platform and packaging problems

Reports about Windows or Linux packaging, installation, startup, updates, and desktop integration are useful. Use the bug form and include your platform version and package format. Never include private signing material or sensitive machine data.

## Build a plugin

Plugin authors normally keep plugin source in their own repositories. The public [Chronlyt-Plugins repository](https://github.com/n3d7/Chronlyt-Plugins) provides the canonical contracts, validation tooling, compatibility material, and registry foundation.

Community registry intake is still evolving and is not yet fully open. Do not assume a plugin can be submitted or listed until that repository publishes an active intake process. You can still study the contracts and build compatible plugin work in your own repository.

## Report a security issue

Do not open a public issue for a vulnerability. Follow [SECURITY.md](SECURITY.md) and use GitHub's private vulnerability reporting flow.

## Repository boundaries

- `n3d7/Chronlyt` is the public home for documentation, releases, issue tracking, and project information.
- The proprietary Chronlyt core is maintained separately and is not open to external source pull requests.
- [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins) contains the public plugin contracts, validator, compatibility material, and registry work.

Contributing here does not grant access to the private application source. Please keep reports and pull requests within the public repository boundary.
