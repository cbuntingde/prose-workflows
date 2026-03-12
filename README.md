> **Note**: These workflows haven't been fully tested yet, so they may not install or run perfectly out of the box. If you run into any issues, feel free to open a new issue!

> **Docs**: [OpenClaw Prose Documentation](https://docs.openclaw.ai/prose)

# Prose Workflows

A collection of multi-agent AI workflows using [OpenProse](https://prose.md), a portable markdown-first programming language for orchestrating AI sessions.

## Overview

This repository contains reusable `.prose` files that spawn multiple specialized AI agents to handle complex, multi-step tasks. Each prose is self-contained and platform-agnostic.

## Platform Support

OpenProse runs on any **Prose Complete** system. These workflows are compatible with:

- **Claude Code** + Opus
- **OpenCode** + Opus  
- **Amp** + Opus

Your `.prose` files work across all supported platforms—no lock-in.

## Installation

Install the OpenProse skill for your platform:

```bash
# For OpenCode
npx skills add openprose/prose

# For Claude Code / Amp - see prose.md for instructions
```

## Available Prose

| Prose | Description |
|-------|-------------|
| [security-reviewer](./security-reviewer/) | Comprehensive security vulnerability scanning |
| [contract-reviewer](./contract-reviewer/) | Contract analysis and risk assessment |
| [financial-modeler](./financial-modeler/) | Financial projections and valuation |
| [board-pack-assembler](./board-pack-assembler/) | Board meeting material assembly |
| [patent-landscaper](./patent-landscaper/) | Patent landscape analysis |
| [due-diligence-analyst](./due-diligence-analyst/) | Company due diligence |

## Usage

Run any prose with:

```bash
/prose run <prose-name>/<prose-name>.prose
```

For example:

```bash
/prose run security-reviewer/security-reviewer.prose
```

## Requirements

- A Prose Complete platform (Claude Code, OpenCode, or Amp)
- Opus model access for synthesis tasks
- Sonnet model for analysis tasks

## Contributing

Contributions welcome! Please open a PR with your new prose workflows.

## License

MIT

## Support

If you find these useful, consider [sponsoring](https://github.com/sponsors/gsxrchris) the project.

---

Copyright © 2026 Created by Chris Bunting
