# AI Agent Playbooks & Guardrails

An open, collaborative registry of hardened execution rules, composable prompts, and hardware-specific runtime profiles designed to make AI coding agents more reliable, especially when running with local LLMs.

The content is tool-agnostic plain Markdown intended for use with agents such as OpenHands, VS Code GitHub Copilot (agent mode), Claude Code, Cursor, Cline, and Continue, and with Ollama, LM Studio, vLLM, SGLang, or hosted inference. Compatibility with any specific combination is **Untested** unless a [profile](profiles/README.md) says otherwise. See [Using with different tools](docs/integrations.md).

> **Important:** This repository improves reliability patterns. It does not guarantee deterministic LLM behaviour.

## Why this repository exists

### The Loop Tax

Local models can enter corrective loops after malformed or failed tool calls, lose the original task, or repeatedly re-plan work. Each unnecessary retry consumes time and context while moving the agent farther from the user's objective.

### Hardware Sensitivity

Model behaviour, usable context capacity, and responsiveness can vary significantly with GPU VRAM, system RAM, context size, quantization, inference engine, and runtime settings. A configuration that works on one machine may not work on another.

### Lack of Standardization

Developers repeatedly test the same model, hardware, and tool configurations without a shared evidence format. That makes it hard to distinguish repeatable results from anecdotes, assumptions, and unverified claims.

## What you can use here

1. **Drop-in behavioral guardrails** — reusable rules and prompts for evidence-based reviews, persistent tasks, tool-failure recovery, safe execution, and completion checks.
2. **Hardware/model compatibility profiles** — structured profiles that record runtime configuration, observed limits, and validation status without implying universal results.
3. **Community-contributed reproducible findings** — acceptance tests and a common evidence policy that make reports easier to reproduce and compare.

## Repository map

- [`rules/`](rules/README.md) — composable execution and evidence policies.
- [`prompts/`](prompts/README.md) — task prompts for review, development, GitHub, and DevOps workflows.
- [`profiles/`](profiles/README.md) — hardware/model/runtime observations and a contribution template.
- [`tests/`](tests/README.md) — reproducible acceptance-test scenarios.
- [`docs/`](docs/getting-started.md) — architecture, usage, integrations, methodology, and terminology.
- [`troubleshooting/`](troubleshooting/README.md) — symptoms, diagnosis, and recovery guidance.

## Getting started

1. Read [Getting started](docs/getting-started.md) and choose the rules that fit your agent and risk level.
2. Add the relevant rule and task prompt to your agent's instructions. Adapt tool names to the tools actually available in your environment.
3. Run the corresponding acceptance scenarios in [tests/](tests/README.md).
4. Record your exact setup and evidence using [profiles/TEMPLATE.md](profiles/TEMPLATE.md).

Do not treat a model's own description, a README, or an anecdote as validation. Reports that have not been independently reproduced must be labelled **Experimental**, **Untested**, or **Community Reported**.

## Contributing

Contributions of prompts, sanitized runtime profiles, test improvements, and reproducible findings are welcome. Read [CONTRIBUTING.md](CONTRIBUTING.md) and the [evidence policy](rules/evidence-policy.md) before submitting. Never include credentials, private URLs, personal workstation secrets, or corporate information.

## Safety and support

This repository is not a substitute for human review, backups, access controls, or a project's security process. Start with read-only workflows and explicitly authorize changes. See [SECURITY.md](SECURITY.md) for reporting security issues and [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for community expectations.
