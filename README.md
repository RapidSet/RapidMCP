# rapidmcp

<p align="center">
	<img src="./rapidmcp.svg" alt="rapidmcp icon" width="140" />
</p>

rapidmcp is a standalone MCP server for RapidKit contracts, docs, and validation workflows.
It is intended to run against a RapidKit workspace and communicate over stdio.

## Features

- Loads component, theme, and preset contracts from RapidKit
- Resolves workspace root automatically or from `--root`
- Exposes MCP resources and tools over stdio
- Supports contract and docs validation workflows

## Requirements

- Node.js 20+
- A local RapidKit workspace

## Install

```bash
npm install -g @rapidset/rapidmcp
```

Or run without installing:

```bash
npx @rapidset/rapidmcp --help
```

## Quick Start

From the RapidKit workspace root:

```bash
npx @rapidset/rapidmcp --root "$PWD"
```

Show help:

```bash
npx @rapidset/rapidmcp --help
```

If installed globally:

```bash
rapidmcp --root /absolute/path/to/rapidkit
```

## Root Resolution

If `--root` is not provided, rapidmcp checks these locations in order:

1. Current working directory
2. `rapidkit` under current working directory
3. `../rapidkit` relative to this package

## CLI

```text
rapidmcp [--root /absolute/path/to/rapidkit]
```

## License

MIT
