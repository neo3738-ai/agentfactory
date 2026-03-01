# Agentfactory

**Build, run, and share AI agent pipelines — no coding required.**

Agentfactory is a desktop app for creating multi-agent AI workflows. Design pipelines where specialized agents collaborate: researchers find information, analysts process it, writers produce the output. Connect to any OpenAI-compatible API (Ollama, OpenRouter, LM Studio, OpenAI, etc).

## Features

- **Visual Pipeline Builder** — Drag-and-drop agent pipelines with multi-step workflows
- **Agent Blueprints** — Create reusable agents with custom roles, tools, and system prompts
- **Marketplace** — Browse and install 52+ community template packs with one click
- **Council System** — Multi-model debate and consensus for better decisions
- **Smart Intake** — Describe what you want in plain English, get a ready-to-run pipeline
- **Memory System** — Agents remember context across runs using vector embeddings
- **Factory Floor** — Monitor all running agents in real-time
- **Workbench** — Quick one-shot agent interactions
- **Multiple API Backends** — Works with Ollama (local), OpenRouter, LM Studio, OpenAI, and any OpenAI-compatible endpoint
- **Export & Share** — Export your pipelines as templates for others to use
- **Scheduled Runs** — Set pipelines to run on a cron schedule
- **Tool System** — Agents can use web_fetch, file_read, file_write, shell, and more

## Download

Go to the [Releases](https://github.com/neo3738-ai/agentfactory/releases) page and download the latest version for your platform:

| Platform | File |
|----------|------|
| **Linux** | `agentfactory` (standalone binary) |
| **Windows** | `agentfactory.exe` (standalone binary) |

### Linux Installation

```bash
# Download the binary
chmod +x agentfactory
./agentfactory
```

**Requirements:** WebKitGTK is needed on Linux. On Ubuntu/Debian:
```bash
sudo apt install libwebkit2gtk-4.1-0
```

### Windows Installation

Download `agentfactory.exe` and run it. No installation needed.

**Requirements:** WebView2 runtime (comes pre-installed on Windows 10/11).

## Quick Start

1. **Set up your API** — Go to Settings and configure your AI backend (Ollama recommended for local/free usage)
2. **Try Smart Intake** — Go to the Home tab, type what you want (e.g., "Research the latest AI news and write a summary"), and let Agentfactory build and run a pipeline for you
3. **Browse Marketplace** — Install template packs for common tasks like research, writing, coding, and more
4. **Build Custom Pipelines** — Use the Builder tab to create your own multi-agent workflows

## API Setup

Agentfactory works with any OpenAI-compatible API:

| Backend | URL | Notes |
|---------|-----|-------|
| **Ollama** (recommended) | `http://localhost:11434` | Free, local, private |
| **OpenRouter** | `https://openrouter.ai/api/v1` | Many models, pay-per-use |
| **LM Studio** | `http://localhost:1234/v1` | Local GUI for models |
| **OpenAI** | `https://api.openai.com/v1` | GPT-4, etc. |

## Community Templates

Browse 52+ pre-built templates in the Marketplace tab, organized into packs:

- **Information & News** — News briefings, deep research, Reddit summaries, site monitoring
- **Content Creation** — Blog posts, emails, stories, newsletters, social media
- **Developer Tools** — Code review, bug analysis, API design, documentation
- **Productivity** — Daily planning, meeting notes, brainstorming, goal setting
- **Personal & Lifestyle** — Meal planning, workouts, travel, language learning
- **Finance & Money** — Budget analysis, stock research, price tracking, crypto
- **Learning & Study** — Study guides, flashcards, topic deep-dives, tutoring
- **Data & Analysis** — CSV analysis, log parsing, SEO auditing

Want to contribute a template? Visit [agentfactory-templates](https://github.com/neo3738-ai/agentfactory-templates).

## Architecture

Agentfactory is built with:
- **Rust** backend (Tauri v2) for performance and security
- **Alpine.js** frontend for a lightweight, reactive UI
- **SQLite** for local data storage
- All data stays on your machine — no cloud dependency

## License

Agentfactory is proprietary software. Free to use for personal and commercial purposes. Source code is not included.

Community templates are open source under MIT License.
