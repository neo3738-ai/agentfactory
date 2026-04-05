# AgentFactory

AI agent pipeline builder — create, run, and automate multi-agent workflows powered by local Ollama models or any OpenAI-compatible endpoint.

## Features

- **Agent pipelines** — chain multiple AI agents together with configurable steps and memory
- **Daemon mode** — persistent background job queue via SQLite (`agentfactory --daemon`)
- **HTTP bridge** (port 3849) — full async job management API for external integrations
- **MCP server** — 13+ tools for AI assistant integration (works with Claude, NeoCode, etc.)
- **Marketplace** — install and share agent pipeline templates
- **Conductor integration** — connects with [Conductor](https://github.com/neo3738-ai/conductor) for project/task context
- **Ollama resource scheduling** — `delay_seconds` and `af_await_job` prevent model conflicts
- **Name-based dispatch** — reference agents and pipelines by name, no UUID needed

## Downloads

See [Releases](https://github.com/neo3738-ai/agentfactory/releases) for the latest binaries.

| Platform | File |
|----------|------|
| Linux | `.tar.gz` standalone binary or `.deb` installer |
| Windows | `.zip` archive or `.exe` installer |

## Requirements

- [Ollama](https://ollama.com) running locally (or any OpenAI-compatible endpoint)

## Part of the Horizon AI Protocol suite

Works great alongside [Conductor](https://github.com/neo3738-ai/conductor) and [RPE](https://github.com/neo3738-ai/rpe).

---
Built by [Horizon AI Protocol](https://horizonaiprotocol.com)
