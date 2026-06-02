# Agent OS — Design System

## Style Prompt

A deep-space command terminal for the AI age. Void-black surfaces with emerald signal-green accents. Terminal-native. Developer-cockpit aesthetic. This is not a friendly SaaS dashboard — it's Mission Control for autonomous agents. Every surface is near-black. Every accent pulses with green energy. Typography is system-native. Data is dense. Information glows from darkness like instrument panels at night.

## Colors

### Background Surfaces
| Token | Hex | Role |
|-------|-----|------|
| `--bg-canvas` | `#030304` | Deepest canvas — page background |
| `--bg-surface` | `#0a0a0c` | Primary panel surface |
| `--bg-elevated` | `#111113` | Elevated cards, dropdowns |
| `--bg-hover` | `#1a1a1d` | Hover state surfaces |
| `--bg-active` | `#222225` | Active/selected surfaces |

### Accent — Emerald System
| Token | Hex | Role |
|-------|-----|------|
| `--accent-primary` | `#00d992` | Signal green — CTAs, active states, brand |
| `--accent-secondary` | `#2fd6a1` | Button text, softer green |
| `--accent-muted` | `#10b981` | Low-opacity fills (30%) |
| `--accent-glow` | `rgba(0,217,146,0.15)` | Glow halos |
| `--accent-glow-strong` | `rgba(0,217,146,0.3)` | Strong glow |

### Agent Colors (sidebar identities)
| Agent | Hex | Role |
|-------|-----|------|
| `--agent-hermes` | `#00d992` | Hermes — emerald (orchestrator) |
| `--agent-claude` | `#f54e00` | Claude Code — orange |
| `--agent-antigravity` | `#818cf8` | Antigravity — indigo |
| `--agent-codex` | `#f0c04c` | Codex — gold |
| `--agent-openclaw` | `#e85671` | OpenClaw — rose |

### Text
| Token | Hex | Role |
|-------|-----|------|
| `--text-primary` | `#f2f2f2` | Primary text — near-white |
| `--text-secondary` | `#8b949e` | Secondary — muted blue-gray |
| `--text-tertiary` | `#62666d` | Tertiary — timestamps, metadata |
| `--text-accent` | `#00d992` | Accent text, links |
| `--text-disabled` | `#3d3a39` | Disabled state |

### Borders & Dividers
| Token | Hex | Role |
|-------|-----|------|
| `--border-subtle` | `rgba(255,255,255,0.05)` | Barely visible structure |
| `--border-default` | `rgba(255,255,255,0.08)` | Standard borders |
- `--border-accent` | `rgba(0,217,146,0.3)` | Accent borders, focus rings |

### Semantic
| Token | Hex | Role |
|-------|-----|------|
| `--status-ok` | `#10b981` | Healthy, success |
| `--status-warn` | `#f0c04c` | Warning, degraded |
| `--status-error` | `#e85671` | Error, critical |
| `--status-info` | `#4cb3d4` | Informational |

### Status (Kanban)
| Token | Hex | Role |
|-------|-----|------|
| `--kanban-todo` | `#62666d` | Todo column |
| `--kanban-progress` | `#f0c04c` | In progress |
| `--kanban-review` | `#818cf8` | In review |
| `--kanban-done` | `#10b981` | Done |

## Typography

- **Primary-font:** `Inter, system-ui, -apple-system, sans-serif`
- **Monospace:** `'JetBrains Mono', ui-monospace, SFMono-Regular, Menlo, monospace`

### Scale
| Role | Size | Weight | Line-height | Tracking |
|------|------|--------|-------------|----------|
| Display | 32px | 700 | 1.1 | -0.02em |
| Panel Title | 14px | 600 | 1.2 | 0.08em uppercase |
| Body | 13px | 400 | 1.5 | 0 |
| Mono / Code | 12px | 400 | 1.4 | 0 |
| Caption | 11px | 400 | 1.4 | 0.04em uppercase |
| Micro | 10px | 500 | 1.2 | 0.1em uppercase |

## Spacing

Base unit: 4px. Scale: 4, 8, 12, 16, 20, 24, 32, 40, 48, 64, 80

- Panel padding: 16px
- Card padding: 12px
- Gap between cards: 8px
- Section gap: 24px

## Elevation (Shadows)

```css
--shadow-sm: rgba(0,0,0,0.4) 0px 2px 8px;
--shadow-md: rgba(0,0,0,0.6) 0px 4px 24px;
--shadow-lg: rgba(0,0,0,0.7) 0px 8px 48px;
--shadow-glow: 0 0 20px rgba(0,217,146,0.15);
--shadow-glow-strong: 0 0 40px rgba(0,217,146,0.25);
```

## Borders

- Standard: `1px solid var(--border-default)`
- Accent: `1px solid var(--border-accent)`
- Radius: 4px (cards), 8px (panels), 999px (pills/badges)

## What NOT to Do

1. Never use pure black `#000` on pure white `#fff` — always use the warm-tinted variants
2. Never use rounded corners on code/mono elements — keep them square
3. Never use more than one accent color per panel — emerald only unless semantic
4. Never use drop shadows without a dark background — they only work on dark surfaces
5. Never use animated gradients or flashy transitions — subtle 150ms ease only
6. Never use more than 3 font sizes in a single component
7. Never use `#333`, `#3b82f6`, or `Roboto` — these are generic AI slop
