# Chronlyt

**One desktop application, shaped by the plugins you choose.**

Chronlyt is becoming a modular desktop platform: Chronlyt provides the base application, and plugins determine what it can do.

Instead of shipping every idea as a permanent built-in feature, Chronlyt is designed to let you add only the capabilities you need. Different plugin combinations can make the same base application useful for very different purposes.

Plugin development lives in the **[Chronlyt Plugins repository](https://github.com/n3d7/Chronlyt-Plugins)**. Check that repository for available plugins, work in progress, and current plugin documentation.

[Downloads](#downloads) · [Documentation](docs/user/README.md) · [Plugins](https://github.com/n3d7/Chronlyt-Plugins) · [Report a bug](https://github.com/n3d7/Chronlyt/issues/new?template=bug_report.yml)

## The idea

Chronlyt provides a common desktop foundation. Plugins add the parts that make the application useful to you.

A plugin could, for example, add a productivity workflow, system monitoring, automation, alerts, an external-service integration, analytics, or a focused utility. These are examples of what the platform direction can support—not a list of functionality that is already available.

This approach means:

- you choose the functionality you actually want;
- two Chronlyt installations can serve very different purposes;
- new ideas can grow as separate plugins instead of turning the core into one large collection of unrelated features;
- plugin work can evolve independently from the base application.

## Current status

Chronlyt is under active development and remains pre-stable (`0.x`). The project is transitioning from its earlier fixed-feature application into the plugin-based platform described here.

The plugin experience, compatibility expectations, and available functionality are still evolving. Do not assume that an example on this page is implemented. Use the [Chronlyt Plugins repository](https://github.com/n3d7/Chronlyt-Plugins) and release notes as the sources for what is currently available.

## Downloads

Published builds are available from [GitHub Releases](https://github.com/n3d7/Chronlyt/releases).

Release assets may include:

- **Windows 10 / 11:** NSIS installer
- **Fedora and other RPM-based Linux distributions:** RPM package
- **Debian / Ubuntu:** DEB package
- **Other Linux distributions:** AppImage

Because Chronlyt is pre-stable, interfaces, packaging, data formats, and plugin behavior may change before `1.0`. Read the release notes before updating.

## Documentation

Start with the [Chronlyt documentation](docs/user/README.md) for the platform concept, project status, releases, privacy, and frequently asked questions.

The public documentation intentionally does not present the old built-in productivity feature set as the current product. Plugin-specific usage and development information belongs with the plugin work in [Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins).

## Privacy and security

Local-first and privacy-conscious operation remain important project principles. The base application and individual plugins do not necessarily have identical data or network behavior, so review the documentation for any plugin you choose to use.

See the [Privacy document](PRIVACY.md) for the current scope and the [Security Policy](SECURITY.md) for responsible vulnerability reporting.

## Repository roles

This public repository contains Chronlyt project documentation, release information, issue tracking, and other public resources for the base application.

The closed-source Chronlyt application implementation is maintained separately and is not published here. Plugin development is organized in [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins).

## Licensing

Chronlyt is proprietary, closed-source software. This repository contains public documentation and project resources; it does not contain the Chronlyt application source code.
