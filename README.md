# Chronlyt

**A private, local-first desktop workspace that becomes the tool you want it to be.**

Chronlyt starts with a focused base application. Add optional plugins for the tools and workflows that matter to you, and leave out the ones that do not.

**Start with Chronlyt. Make it yours.**

[Download](https://github.com/n3d7/Chronlyt/releases) · [Plugins](docs/user/plugins.md) · [Documentation](docs/user/README.md) · [Privacy](PRIVACY.md) · [Security](SECURITY.md) · [Contributing](CONTRIBUTING.md) · [Report a bug](https://github.com/n3d7/Chronlyt/issues/new?template=bug_report.yml)

## Make Chronlyt yours

Not everyone needs the same desktop app. Chronlyt is designed so that its core stays focused while you choose which additional capabilities belong in your workspace.

One installation might support a productivity workflow. Another could be shaped around monitoring, automation, analytics, alerts, integrations, or a few focused desktop utilities. Those are examples of what plugins can make possible, not a claim that every such plugin is already published.

This approach lets you:

- install only the capabilities you actually want;
- keep the base application focused;
- combine plugins into a workspace that fits your needs;
- change that workspace as your needs change.

Plugins extend Chronlyt; they do not replace its trusted core. The application remains responsible for plugin identity, permissions, validation, and the narrow capabilities made available to each plugin.

## Local-first by design

Chronlyt is built around local-first, privacy-conscious operation. Core structured data is stored locally by default, and the base application is designed to remain useful without an account or continuous network connection.

Local-first does not mean that Chronlyt never uses the network. Update checks, account features, plugin discovery, and capabilities you explicitly choose may connect to external services. See [Privacy](PRIVACY.md) for the current boundaries.

## A deliberately limited plugin model

Chronlyt v1 plugins run as WebAssembly Components behind a host-controlled interface. They receive only approved capabilities and do not get direct APIs for arbitrary filesystem or network access, process execution, raw SQLite access, or application credentials.

Packages and components are validated before execution, and the runtime applies resource limits. These controls reduce risk; they do not make every plugin inherently trustworthy. Consider a plugin's provenance and requested capabilities before installing it. See the [Security Policy](SECURITY.md) for more detail.

## Current status

Chronlyt is pre-stable (`0.x`). The focused core and public plugin foundation exist, but interfaces and packaging may still change before `1.0`.

The community plugin registry is not yet fully open, and Chronlyt does not currently claim a mature marketplace or large catalogue. Check release notes and the public plugin repository for what is actually available.

## Download Chronlyt

Get current builds from [GitHub Releases](https://github.com/n3d7/Chronlyt/releases). Depending on the release, assets may include:

- Windows 10/11: NSIS installer;
- Fedora and other RPM-based Linux distributions: RPM package;
- Debian/Ubuntu: DEB package;
- other Linux distributions: AppImage.

Package availability can vary. Read the release notes and verification information before installing or updating.

## Plugins and the public ecosystem

The public [Chronlyt-Plugins repository](https://github.com/n3d7/Chronlyt-Plugins) contains the shared plugin contracts, validation tooling, compatibility material, and registry work.

Plugin authors normally keep their source code in their own repositories and publish their own release artifacts. Community registry intake is still evolving, so consult that repository before preparing a submission.

For the user-facing overview, read [How plugins shape Chronlyt](docs/user/plugins.md).

## Contributing and support

The Chronlyt application core is proprietary and closed-source, but there are still useful ways to contribute: report bugs, improve public documentation, describe platform packaging problems, suggest improvements, or create plugins using the public ecosystem contracts.

Start with [CONTRIBUTING.md](CONTRIBUTING.md). Report security vulnerabilities privately as described in [SECURITY.md](SECURITY.md), not through a public issue.

Useful links:

- [User documentation](docs/user/README.md)
- [Getting started](docs/user/getting-started.md)
- [Changelog](CHANGELOG.md)
- [Bug report](https://github.com/n3d7/Chronlyt/issues/new?template=bug_report.yml)
- [Feature request](https://github.com/n3d7/Chronlyt/issues/new?template=feature_request.yml)

## Source availability and ownership

The Chronlyt application core is proprietary and closed-source. Its source is maintained separately and is not published in `n3d7/Chronlyt`; external contributors cannot submit core-source pull requests here.

This repository is the public home for Chronlyt documentation, releases, issue tracking, and project information. The plugin ecosystem, public contracts, validators, and registry foundation are public in [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins).

Chronlyt is maintained by [n3d7](https://github.com/n3d7).
