# Using with different tools

The rules and prompts are plain Markdown. Only the place you put them changes per tool. Adapt tool names to those your agent actually has.

> **Note:** File locations below are common conventions and may change between tool versions. Check each tool's current documentation. They have not been validated by this repository's acceptance tests unless a profile says so.
| Tool | Where to put the rules | Where to use the prompts |
|---|---|---|
| OpenHands | Microagents / repo `AGENTS.md`, or paste into the task | Paste a file from `prompts/` as the task |
| VS Code GitHub Copilot | [`.github/copilot-instructions.md`](../.github/copilot-instructions.md) or `.github/instructions/*.instructions.md` | Copy to `.github/prompts/*.prompt.md`, run with `/name` in chat |
| Claude Code | `CLAUDE.md` (can import `AGENTS.md`) | Paste, or save as a custom slash command |
| Cursor | `.cursor/rules/*.mdc` | Paste into chat/agent |
| Cline / Continue / others | Their rules file; many read `AGENTS.md` | Paste into chat |

## Recommended workflow

1. Copy the rules you need from [`rules/`](../rules/README.md) into your tool's instruction location.
2. Pick a prompt from [`prompts/`](../prompts/README.md).
3. Validate with [`tests/`](../tests/README.md) and record results with the [profile template](../profiles/TEMPLATE.md), naming the agent tool and version used.

Tool-specific adapter files should live in this document or in a clearly named folder, never change the shared rules to fit a single tool.
