# Agentfactory

**Build, run, and share AI agent pipelines — no coding required.**

Agentfactory is a desktop app for creating multi-agent AI workflows. Design pipelines where specialized agents collaborate: researchers find information, analysts process it, writers produce the output. Connect to any OpenAI-compatible API (Ollama, OpenRouter, LM Studio, OpenAI, etc).

## Features

- **Visual Pipeline Builder** — Drag-and-drop agent pipelines with multi-step workflows
- **Agent Blueprints** — Create reusable agents with custom roles, tools, and system prompts
- **Marketplace** — Browse and install 160+ community template packs with one click
- **Council System** — Multi-agent debate, voting, and judge arbitration for better decisions
- **Council Presets** — 12 pre-built councils (Writing, Code Review, Decision, Research, Creative, Strategy, Automation, Business, Data, Content, Finance) — one click to create
- **Smart Intake** — Describe what you want in plain English, get a ready-to-run pipeline
- **Conversation Mode** — Continue chatting with your pipelines after they run
- **Markdown Output** — Agent responses rendered with full formatting (headings, code blocks, lists, tables)
- **Memory System** — Agents remember context across runs using vector embeddings
- **Knowledge Bases** — Organize memories into named collections for better retrieval
- **Memory Explorer** — Filter, pin, bulk-manage, and search agent memories
- **Inline Tune Panel** — Adjust model, temperature, max tokens, and system prompt on the fly
- **Quick-Tune Presets** — One-click creative, precise, verbose, or concise modes
- **A/B Compare** — Run two configurations side-by-side and pick the winner
- **Blueprint Versioning** — Auto-snapshot blueprints before tuning changes
- **Factory Floor** — Monitor all running agents in real-time
- **Workbench** — Quick one-shot agent interactions with memory preview
- **Multiple API Backends** — Works with Ollama (local), OpenRouter, LM Studio, OpenAI, and any OpenAI-compatible endpoint
- **Export & Share** — Export your pipelines as templates for others to use
- **Scheduled Runs** — Set pipelines to run on a cron schedule
- **Tool System** — Agents can use web_fetch, file_read, file_write, shell, and more

## Download

Go to the [Releases](https://github.com/neo3738-ai/agentfactory/releases) page and download the latest version for your platform:

| Platform | File |
|----------|------|
| **Linux** | `agentfactory-v0.3.1-linux-x86_64.tar.gz` |
| **Windows** | `agentfactory-v0.3.1-windows-x86_64.zip` |

### Linux Installation

```bash
# Download and extract
tar xzf agentfactory-v0.3.1-linux-x86_64.tar.gz
cd agentfactory-v0.3.1-linux

# Run directly
chmod +x agentfactory
./agentfactory
```

**Requirements:** WebKitGTK is needed on Linux. On Ubuntu/Debian:
```bash
sudo apt install libwebkit2gtk-4.1-0
```

### Windows Installation

Download and extract `agentfactory-v0.3.1-windows-x86_64.zip`, then run `agentfactory.exe`. No installation needed.

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

Browse 160+ pre-built templates in the Marketplace tab, organized into 10 packs:

- **Information & News** — News briefings, deep research, Reddit summaries, site monitoring
- **Content Creation** — Blog posts, emails, stories, newsletters, social media
- **Developer Tools** — Code review, bug analysis, API design, documentation
- **Productivity** — Daily planning, meeting notes, brainstorming, goal setting
- **Personal & Lifestyle** — Meal planning, workouts, travel, language learning
- **Finance & Money** — Budget analysis, stock research, price tracking, crypto
- **Learning & Study** — Study guides, flashcards, topic deep-dives, tutoring
- **Data & Analysis** — CSV analysis, log parsing, SEO auditing
- **Automation** — Workflow automation, scheduling, monitoring, notifications
- **Business** — Business planning, marketing, HR, customer service

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
