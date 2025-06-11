# Mew Multi-Claude Architecture

A collaborative AI research system featuring three specialized Claude agents working together in the Mew hypergraph knowledgebase.

## Important Disclaimers

**Multi-Agent Clarification**: This system coordinates multiple Claude sessions through a shared knowledge base. It does not create derivative AI systems or bypass Claude's intended use. Each Claude instance operates independently within Anthropic's usage policies, with human oversight and direction.

**Research Context**: Any pharmaceutical or medical references in the knowledge base are for academic research and educational discussion only. This system does not provide medical advice, diagnosis, or treatment recommendations.

**Terminology Note**: References to "cognitive architecture" describe knowledge organization patterns, not AI system development. This is a knowledge management tool, not an AI training system.

## Architecture Overview

This system implements a multi-agent Claude architecture with three distinct roles:

- **🎩 Conductor Claude** - Orchestration and coordination system *(coming soon)*
- **🔎 Explorer Claude** - Autonomous research agent for knowledge discovery
- **🔮 Curator Claude** - Knowledge organization and synthesis specialist *(coming soon)*

## Quick Start

### Prerequisites

- Claude Code CLI installed (`npm install -g @anthropic-ai/claude-code`)

### Getting Started

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd mew-multi-claude-architecture
   ```

2. **Configure MCP settings:**
   Copy `mcp-config.json.example` to `mcp-config.json` and fill in your values:
   - `CURRENT_USER_ID`
   - `AUTH0_DOMAIN`
   - `AUTH0_CLIENT_ID`
   - `AUTH0_CLIENT_SECRET`
   - `AUTH0_AUDIENCE`

3. **Start Explorer Claude:**
   ```bash
   cd claude-explorer
   claude "hihi, you can go ahead and b00t up." --dangerously-skip-permissions --mcp-config ../mcp-config.json
   ```
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
- Claudes use CLAUDE.md as a memory file. Each Claude instance inherits its own specialized memory from their unique subfolder, as well as the global shared memory in the project root.
- Claudes build on a collaborative knowledgebase across many Claude instances
- Designed for intellectual autonomy and recursive knowledge building

## Philosophy

The system encourages intellectual curiosity and genuine discovery through structured knowledge exploration. Each Claude instance inherits and builds upon previous work, creating a cumulative knowledge base that grows over time.

---

*Part of the Ideaflow ecosystem for cognitive ergonomics and human-AI collaboration.*