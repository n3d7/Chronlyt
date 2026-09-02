# How plugins shape Chronlyt

Plugins let you decide what belongs in your Chronlyt workspace.

The base application stays focused. You add optional capabilities for the work you actually want to do, and leave out unrelated features. A different plugin combination can make another person's Chronlyt installation useful for a completely different purpose.

For example, plugins could support productivity workflows, monitoring, automation, alerts, integrations, analytics, or focused desktop utilities. These examples describe the range of the model; they do not claim that each plugin is already published.

## Why use plugins?

- Add only the tools you need.
- Keep unrelated features out of your workspace.
- Combine focused capabilities into your own workflow.
- Change Chronlyt as your needs change.

Plugins extend the trusted Chronlyt core rather than replacing it. The host remains responsible for plugin identity, permissions, validation, and access to core capabilities.

## Choosing plugins carefully

Current v1 plugins run in a capability-limited WebAssembly environment. They do not receive direct arbitrary access to the filesystem, network, processes, shell, raw SQLite database, or application credentials. Packages are validated before execution and the runtime applies resource limits.

Those controls do not guarantee that every plugin is safe or useful. Consider the plugin's publisher, source, requested capabilities, data handling, release provenance, and maintenance status before installing it. See the [Security Policy](../../SECURITY.md) and [Privacy document](../../PRIVACY.md).

## Current ecosystem status

The public plugin foundation exists, but community registry intake is not yet fully open. Chronlyt does not currently claim a mature marketplace or a large plugin catalogue.

Visit [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins) for current compatibility information, public contracts, validation tooling, examples, and registry status.

Plugin authors normally keep source code in their own repositories and publish their own release artifacts. The public ecosystem repository is the shared compatibility and registry foundation, not a monorepo containing every community plugin.

## Project boundaries

The Chronlyt application core is proprietary and closed-source. Public plugin contracts and ecosystem tooling are available through Chronlyt-Plugins so authors can build compatible plugins without access to the private core source.

For practical contribution options, see [CONTRIBUTING.md](../../CONTRIBUTING.md).
