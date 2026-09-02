# Frags

Frags is the open-source runtime for AI-powered backend services. It executes **FML** plans as typed, multi-session workflows — coordinating tools, scoped context, deterministic prework, and schema validation so a prompt becomes a service you can call.

## Key Capabilities

- Multi LLM: Frags supports multiple LLMs, allowing you to choose the one that best suits your needs.
- **Structured, typed output**: Every session produces machine-consumable JSON, validated against a declared schema — built for services, not chat transcripts.
- **Multi-session orchestration**: Break a complex workflow into scoped sessions with explicit dependencies, so each step gets only the context it needs.
- **Advanced tooling**: Declare MCP servers, APICP-backed APIs, collections, or custom functions — tool use stays explicit and local to the sessions that need it.
- **Anti-context-bloating by design**: Scope exactly what enters each LLM call to cut cost and reduce hallucination risk.
- **Deterministic pre/post-processing**: Transforms, filters, and pre-calls handle mechanical work outside the model — lower cost, better reliability.
- **CLI and Go library**: Prototype from the command line, then embed the runtime directly into your own services.

## Quick Start

**macOS (Homebrew)**
```bash
brew tap fragshq/tools
brew install fragshq/tools/frags
```

**Windows (Scoop)**
```powershell
scoop bucket add fragshq https://github.com/fragshq/scoop-bucket.git
scoop install frags
```

Prefer a raw binary? Grab the latest release from the [Releases page](https://github.com/FragsHQ/frags/releases).

Run your first prompt:
```bash
frags ask "What is the meaning of life?"
```

## Resources

- 📚 [Local setup guide](https://diaphora.ai/docs/guides/frags-runtime-locally)
- 🧩 [FML examples](https://github.com/fragshq/frags/tree/main/examples)
- 🔌 [API reference](https://diaphora.ai/docs/api)
- 🛠️ [Python / TypeScript SDK](https://diaphora.ai/docs/sdk)

## Support

Need help or found a bug 🐛? Our community forum for support is **GitHub Issues**: [github.com/FragsHQ/frags/issues](https://github.com/FragsHQ/frags/issues)

## License

Frags is AGPL-licensed and fair-code distributed.

- **Source available** — the full runtime source is always visible.
- **Self-hostable** — deploy anywhere, no hosted dependency required.
- **Extensible** — add your own nodes, tools, and MCP servers.

Enterprise Licenses are available for teams that need role-based access, audit trails, and support for sensitive data at scale — see [diaphora.ai/pricing](https://diaphora.ai/pricing).

## Contributing

Found a bug 🐛 or have a feature idea ✨? Open an issue on [GitHub Issues](https://github.com/FragsHQ/frags/issues).
