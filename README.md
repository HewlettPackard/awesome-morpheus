# Awesome Morpheus

> A curated list of **community plugins**, and **Copilot agents & skills**, for [Morpheus Data](https://morpheusdata.com), a hybrid cloud management and orchestration platform.

This list covers plugins published on the [Morpheus Marketplace](https://share.morpheusdata.com) that are community-contributed, i.e. **not** marked "Official" or "Partner" on the marketplace. For officially supported or partner plugins, see the [Morpheus Marketplace](https://share.morpheusdata.com) directly or the [HewlettPackard](https://github.com/HewlettPackard) and [gomorpheus](https://github.com/gomorpheus) GitHub organizations.

Each entry links to its direct download page (e.g. Morpheus Marketplace) and, where available, its public source repository.

Contributions welcome, see [Contributing](#contributing).

## Disclaimer

These are **community-contributed** plugins, agents, and skills, not developed, maintained, or officially supported by Hewlett Packard Enterprise. They are provided **as-is, with no warranty of any kind**. Use at your own risk, review the source and test thoroughly before deploying in production.

## Contents

- [What is Morpheus?](#what-is-morpheus)
- [Disclaimer](#disclaimer)
- [Morpheus Plugins](#morpheus-plugins)
  - [IPAM & DNS](#ipam--dns)
  - [Credential Stores & Secrets](#credential-stores--secrets)
  - [AI / LLM Integrations](#ai--llm-integrations)
  - [FinOps & Cost Management](#finops--cost-management)
  - [Monitoring & Observability](#monitoring--observability)
  - [Localization](#localization)
  - [Platform Utilities](#platform-utilities)
- [Copilot Agents & Skills](#copilot-agents--skills)
  - [Agents](#agents)
  - [Skills](#skills)
- [Related Resources](#related-resources)
- [Contributing](#contributing)
- [License](#license)

## What is Morpheus?

[Morpheus Data](https://morpheusdata.com) is a hybrid/multi-cloud management platform providing self-service provisioning, orchestration, governance, and cost management across public clouds, private clouds, and Kubernetes. Its functionality is extended through a plugin SDK (see [morpheus-plugin-core](https://github.com/HewlettPackard/morpheus-plugin-core)) covering cloud providers, IPAM/DNS, backup, credential stores, load balancers, and more.

## Morpheus Plugins

Plugins are server-side extensions installed into a Morpheus instance via the [Marketplace](https://share.morpheusdata.com), extending its core functionality (cloud providers, IPAM/DNS, monitoring, etc.) using the [plugin SDK](https://github.com/HewlettPackard/morpheus-plugin-core).

### IPAM & DNS

- **NetBox** - NetBox IPAM integration. [Marketplace](https://share.morpheusdata.com/plugin/morpheus-netbox-plugin) · [Source](https://github.com/gomorpheus/morpheus-netbox-plugin)
- **Micetro** - Micetro (Men & Mice) IPAM integration. [Marketplace](https://share.morpheusdata.com/plugin/morpheus-micetro-plugin) · [Source](https://github.com/gomorpheus/morpheus-micetro-plugin)

### Credential Stores & Secrets

- **Fortanix DSM** - Fortanix DSM integration with Cypher and Credential Provider. [Marketplace](https://share.morpheusdata.com/plugin/dsm-plugin) · [Source](https://github.com/fortanix/dsm-hpe-morpheus-plugin)

### AI / LLM Integrations

- **GitHub Copilot** - LLM engine integration plugin for GitHub Copilot. [Marketplace](https://share.morpheusdata.com/plugin/copilot-llm-plugin) · [Source](https://github.com/HewlettPackard/morpheus-copilot-plugin)
- **Local LLM** - LLM engine integration plugin for Ollama and OpenAI-compatible APIs. [Marketplace](https://share.morpheusdata.com/plugin/local-llm-plugin) · [Source](https://github.com/gomorpheus/morpheus-local-llm-plugin)

### FinOps & Cost Management

- **Exivity FinOps** - Custom tab and analytics page for Exivity FinOps. [Marketplace](https://share.morpheusdata.com/plugin/exivity-finops) · [Source](https://github.com/exivity/Morpheus-plugin)

### Monitoring & Observability

- **DataDog** - Adds a DataDog monitoring tab to instance detail pages. [Marketplace](https://share.morpheusdata.com/plugin/datadog-plugin) · [Source](https://github.com/martezr/morpheus-datadog-instance-tab-plugin)

### Localization

- **Crowdin Localization Plugin** - UI localization helper integrating with Crowdin. [Marketplace](https://share.morpheusdata.com/plugin/crowdin-localization-plugin) · [Source](https://github.com/cpdtaylor/morpheus-crowdin-plugin)

### Platform Utilities

- **Morpheus Uplink** - DNS/IPAM delegation to a parent Morpheus instance. [Marketplace](https://share.morpheusdata.com/plugin/morpheus-morpheusuplink-plugin) · [Source](https://github.com/gomorpheus/morpheus-morpheusuplink-plugin)

## Copilot Agents & Skills

Unlike plugins, these are client-side [GitHub Copilot](https://github.com/features/copilot) customizations. They run in your Copilot client (CLI/IDE), not inside Morpheus itself, and interact with Morpheus externally (e.g. via its REST API, CLI, or MCP Server) to automate tasks.

### Agents

Specialized Copilot agents/personas for Morpheus automation and operations. See [`agents/`](agents/).

### Skills

Self-contained, task-specific Copilot skills for Morpheus workflows. See [`skills/`](skills/).

## Related Resources

- [Morpheus Marketplace](https://share.morpheusdata.com) - Official plugin catalog (source of truth for this list).
- [morpheus-plugin-core](https://github.com/HewlettPackard/morpheus-plugin-core) - Plugin SDK defining all provider interfaces.
- [morpheus-plugin-samples](https://github.com/HewlettPackard/morpheus-plugin-samples) - Reference plugin implementations.
- [morpheus-docs](https://github.com/HewlettPackard/morpheus-docs) - User-facing documentation source.
- [morpheus-openapi](https://github.com/HewlettPackard/morpheus-openapi) - Morpheus REST API OpenAPI specification.

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. In short:

- **Plugins**: Include a link to the plugin's Marketplace page, and its public source repository where available. Keep descriptions short (one line) and place entries in the most relevant category, alphabetically.
- **Agents & Skills**: Must interact with Morpheus specifically and follow the format described in [`agents/`](agents/) and [`skills/`](skills/).

## License

This project is licensed under the Apache License, Version 2.0. See [LICENSE](LICENSE).
