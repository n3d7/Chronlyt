# Security Policy

## Reporting a vulnerability

Please report suspected vulnerabilities through GitHub's private vulnerability reporting:

**[Report a vulnerability privately](https://github.com/n3d7/Chronlyt/security/advisories/new)**

Include the affected Chronlyt version, operating system, installation format, relevant plugin and plugin version, and the smallest safe reproduction you can provide.

Do not put the following in a public issue:

- exploitation details that could put users at risk;
- credentials, tokens, API keys, or recovery material;
- personal data;
- private logs, databases, exports, backups, or configuration files.

If you are unsure whether a problem belongs to Chronlyt or a plugin, report it privately and identify the plugin when possible. General bugs that have no security impact belong in the [public bug-report flow](https://github.com/n3d7/Chronlyt/issues/new?template=bug_report.yml).

## Supported versions

Chronlyt is currently pre-stable. Only the latest `0.x` release receives security fixes.

Older builds may contain known problems and should not be treated as supported. Current releases are available from [GitHub Releases](https://github.com/n3d7/Chronlyt/releases).

## Security principles

Chronlyt follows a local-first, least-authority design:

- core functionality is designed to work locally;
- sensitive credentials use operating-system credential facilities rather than ordinary application data;
- privileged native operations remain behind narrow host-controlled interfaces;
- application updates and release artifacts use the verification mechanisms documented with the release;
- plugins receive specific approved capabilities instead of ambient operating-system authority.

These principles reduce exposure, but they are not a guarantee that the application, a plugin, or a dependency can never contain a vulnerability.

## Local-first core and credentials

Structured core data is stored locally. Chronlyt does not require an account or continuous network connection for its basic offline operation.

Some explicit operations still use the network, including update checks, account features, and plugin discovery. See [PRIVACY.md](PRIVACY.md) for the current data-handling boundaries.

Persistent secrets must not be stored in ordinary SQLite data, exports, backups, renderer state, or routine logs. Supported core credentials are kept through operating-system credential storage.

## Updates and releases

Install Chronlyt only from the project's [GitHub Releases](https://github.com/n3d7/Chronlyt/releases) or another source explicitly documented by the project. Follow the signature, checksum, and update-verification guidance supplied with the release.

Do not bypass update verification to install an unexpected artifact. If verification fails, stop and report the problem privately.

## Plugin isolation and permissions

Chronlyt Plugin System v1 uses WebAssembly Component Model isolation with a host-controlled runtime. The host owns plugin identity, granted permissions, and access to application capabilities; a plugin cannot grant authority to itself.

The v1 interface exposes narrow capabilities rather than direct APIs for:

- arbitrary filesystem access;
- arbitrary network access;
- process or shell execution;
- raw SQLite access;
- application credentials.

Plugin packages and components are validated before execution. The runtime also enforces bounded memory, execution fuel, and deadlines. Host operations apply their own validation and limits.

Sandboxing and validation reduce risk but do not make every plugin safe. Before installing one, consider its publisher and source, requested capabilities, release provenance, and maintenance status.

## Core and plugin responsibility

Chronlyt is responsible for enforcing the core security boundary, validating packages, and granting only approved host capabilities. A plugin remains responsible for its own logic, dependencies, data handling, and truthful documentation.

Public plugin contracts, validation tooling, compatibility material, and registry work live in [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins). Community registry intake is not yet fully open, and registry validation would not replace runtime validation by Chronlyt.

## Closed-source core

The Chronlyt application core is proprietary and closed-source. Its source is maintained separately and is not published in this repository.

This public repository contains documentation, releases, issue tracking, and public project information. See [CONTRIBUTING.md](CONTRIBUTING.md) for the contribution boundaries and [PRIVACY.md](PRIVACY.md) for privacy information.
