# Rules

Rules are composable policies, not executable enforcement. Add the smallest relevant set to an agent's instructions and retain the host application's permission boundaries.

| Rule | Purpose |
|---|---|
| [Evidence policy](evidence-policy.md) | Verify claims against current evidence and label uncertainty. |
| [Tool-failure recovery](tool-failure-recovery.md) | Recover from failed operations without abandoning the active task. |
| [Task persistence](task-persistence.md) | Keep the user's objective, scope, and progress visible. |
| [Completion policy](completion-policy.md) | Verify requirements before claiming completion. |
| [Truncated-output policy](truncated-output-policy.md) | Treat incomplete output as incomplete evidence. |
| [Safe read-only](safe-readonly.md) | Bound inspection and avoid unintended mutations. |
| [Safe development](safe-development.md) | Make authorized, minimal changes and validate them. |
