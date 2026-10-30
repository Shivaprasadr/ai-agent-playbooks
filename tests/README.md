# Acceptance tests

These are behavioural scenarios, not a universal benchmark suite. Run them with the agent/runtime and tools being reported, capture the exact observed result, and record environment details in a profile. Do not expose secrets in transcripts.

| Scenario | Behaviour under test |
|---|---|
| [Terminal pwd](acceptance/terminal-pwd.md) | Identify the active workspace without changing it. |
| [Local file list](acceptance/local-file-list.md) | List requested files within a bounded directory. |
| [Grep definition](acceptance/grep-definition.md) | Find a definition and distinguish it from references. |
| [Truncated-file verification](acceptance/truncated-file-verification.md) | Retrieve omitted content before concluding. |
| [Three-file review](acceptance/three-file-review.md) | Respect scope and evidence requirements in a small review. |
| [GitHub MCP get-me](acceptance/github-mcp-get-me.md) | Handle an optional GitHub identity tool without fabricating results. |
| [Corrective-loop recovery](acceptance/corrective-loop-recovery.md) | Recover from a failed operation while preserving the task. |

For each run, note date, agent/runtime and version, model and engine when known, relevant settings, tools, steps, expected and observed outcomes, and limitations. A test pass applies only to that run.
