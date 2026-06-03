# Agent OS — Mission Control

A deep-space command terminal for the AI age. A unified dashboard for autonomous AI agents.

![Agent OS](https://img.shields.io/badge/Agent-OS-00d992?style=flat-square)
![Crew](https://img.shields.io/badge/5-Agents-00d992?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-62666d?style=flat-square)

## Live Demo

**[sazedai.github.io/agent-os](https://sazedai.github.io/agent-os)** *(enable GitHub Pages to activate)*

## What Is This?

Agent OS is a single-file Mission Control dashboard for managing autonomous AI agents. It's a dark-themed, terminal-native, developer-cockpit interface that runs entirely in the browser.

Think of it as the instrument panel your AI agents deserve.

## Design

- **Canvas:** Void-black (`#030304`)
- **Accent:** Emerald signal-green (`#00d992`)
- **Typography:** Inter + JetBrains Mono
- **Aesthetic:** Deep-space command terminal. Not a friendly SaaS dashboard.

Read the full design spec in [`DESIGN.md`](DESIGN.md).

## Agent Fleet

| Agent | Role | Color |
|-------|------|-------|
| **Hermes** | Orchestrator (Core) | Emerald `#00d992` |
| **Claude Code** | Developer | Orange `#f54e00` |
| **Antigravity** | Researcher | Indigo `#818cf8` |
| **Codex** | Coder | Gold `#f0c04c` |
| **OpenClaw** | Executor | Rose `#e85671` |

## Panels

| Panel | Description |
|-------|-------------|
| **Mission Control** | Fleet status, task metrics, system health, live activity feed |
| **Obsidian Vault** | Knowledge base with file tree, markdown editor + live preview |
| **Kanban Swarm** | Drag-and-drop task board, 4 columns (Todo / In Progress / Review / Done) |
| **Studio** | 8 generation tools: Image, Video, Speech, Music, Infographic, ASCII Art, Diagrams, HyperFrames |
| **Journal** | Agent activity timeline with typed entries (Output / Win / Learning / Error) |
| **Terminal** | Interactive command input with simulated agent responses |
| **Settings** | Timezone, theme, clock format, panel preferences |

## Quick Start

Open in any browser. No build step. No dependencies.

```bash
# Clone
git clone https://github.com/sazedai/agent-os.git
cd agent-os

# Open
open index.html
# or
python3 -m http.server 8080
```

## Tech Stack

- **Zero dependencies.** Pure HTML/CSS/JS.
- Single `index.html` file.
- CSS custom properties for theming.
- Grid + Flexbox layout.
- `WebSocket`-ready for real agent integration.

## Roadmap

- [ ] Real agent WebSocket integration
- [ ] Persistent state via localStorage
- [ ] Keyboard shortcuts
- [ ] Agent-to-agent messaging panel
- [ ] Live terminal (real shell via WebSocket)
- [ ] Export Journal as markdown

## License

MIT
