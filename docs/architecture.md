# Architecture

This repository is a human-maintained registry of reusable text artifacts and reproducible test scenarios. It is not an agent runtime, model evaluator, or compatibility guarantee.

## Layers

1. **Rules** define cross-cutting behaviour: evidence, task persistence, recovery, completion, safe access, and truncated-output handling.
2. **Prompts** combine selected rules with a specific task such as code review, bug investigation, or infrastructure troubleshooting.
3. **Profiles** record the exact model, hardware class, inference engine, settings, observations, and validation status for a reported setup.
4. **Acceptance tests** describe observable scenarios for checking whether an agent follows a playbook.
5. **Examples and troubleshooting** demonstrate application and explain common failures without replacing the underlying policies.

## Use and composition

Select only the rules needed for the task, then add a task prompt. Preserve the active user objective and follow the host agent's permission model. The repository does not assume a particular agent product, tool namespace, or that any external tool is available. See [integrations](integrations.md) for per-tool placement.

Keep policy separate from claims about performance. A prompt can request verification; only recorded evidence from a particular run can establish what happened in that run. Profiles and test results are environment-specific and should be dated and labelled accordingly.
