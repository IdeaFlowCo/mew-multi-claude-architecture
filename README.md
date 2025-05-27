# Mew Multi-Claude Architecture

A collaborative AI research system featuring three specialized Claude agents working together in the [Mew](https://mew.ai) hypergraph knowledge ecosystem.

## Architecture Overview

This system implements a multi-agent Claude architecture with three distinct roles:

- **🔎 Explorer Claude** - Autonomous research agent for knowledge discovery
- **🔮 Curator Claude** - Knowledge organization and synthesis specialist *(coming soon)*
- **🎩 Conductor Claude** - Orchestration and coordination system *(coming soon)*

## Quick Start

### Prerequisites

Ensure you have the following environment variables configured:
- `CURRENT_USER_ID`
- `BASE_URL` 
- `BASE_NODE_URL`
- `AUTH0_DOMAIN`
- `AUTH0_CLIENT_ID`
- `AUTH0_CLIENT_SECRET`
- `AUTH0_AUDIENCE`

### Running the System

Currently, only Explorer Claude is implemented:

```bash
claude --dangerously-skip-permissions --mcp-config mcp-config.json
```

### Future Architecture (In Development)

Once the full system is implemented, you'll typically want to run the Conductor Claude, which will manage the other agents:

```bash
# Conductor Claude (orchestrates other agents)
claude --file claude-conductor.md --dangerously-skip-permissions --mcp-config mcp-config.json

# Or run individual agents directly:

# Explorer Claude (research and discovery)
claude --file claude-explorer.md --dangerously-skip-permissions --mcp-config mcp-config.json

# Curator Claude (knowledge synthesis)
claude --file claude-curator.md --dangerously-skip-permissions --mcp-config mcp-config.json
```

## What This System Does

This is part of a larger project building cognitive ergonomics for human-machine collaboration. The Claude agents:

- Autonomously explore and map knowledge domains
- Synthesize insights across disciplines 
- Challenge assumptions and identify knowledge gaps
- Build living maps of evolving concepts
- Create unexpected bridges between domains

## Technical Details

- Uses [MCP (Model Context Protocol)](https://modelcontextprotocol.io/) for tool integration
- Connects to the Mew hypergraph knowledge base via `mew-mcp`
- Implements collaborative workspace inheritance between Claude instances
- Designed for intellectual autonomy and recursive knowledge building

## Philosophy

The system encourages "intellectual recklessness" - prioritizing genuine discovery over safe, predictable responses. Each Claude instance inherits and builds upon previous work, creating a cumulative intelligence that grows over time.

---

*Part of the [Mew](https://mew.ai) ecosystem for cognitive ergonomics and human-AI collaboration.*