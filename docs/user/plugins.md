# Plugins

Plugins are what turn the Chronlyt base application into a tool for a particular purpose.

Chronlyt provides the shared desktop foundation. A plugin contributes a focused capability. Choosing a different set of plugins can therefore produce a very different application without requiring every feature to live permanently in the core.

Possible plugins could support productivity workflows, monitoring, automation, alerts, service integrations, analytics, or small desktop utilities. These examples explain the model; they do not claim that specific plugins are already implemented.

## Plugin repository

Plugin development is organized in [n3d7/Chronlyt-Plugins](https://github.com/n3d7/Chronlyt-Plugins).

Use that repository to check:

- which plugins currently exist;
- which ideas are only planned or experimental;
- plugin-specific setup and usage instructions;
- the compatibility information available for a plugin.

This documentation does not promise a stable plugin API, installation method, compatibility contract, or security boundary that has not been published by the project.

## Choosing a plugin

Treat plugin code and plugin-provided instructions as separate from the Chronlyt core. Before using a plugin, review its source or provenance, documentation, data handling, network behavior, and current maintenance status when that information is available.
