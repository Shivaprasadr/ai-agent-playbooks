# Getting started

## Use a playbook

0. See [integrations](integrations.md) for where your agent tool reads rules and prompts.
1. Identify your agent, available tools, and whether it can edit files or take external actions.
2. Start with the relevant read-only rules in [`rules/`](../rules/README.md). Add task-persistence, recovery, and completion policies for longer tasks.
3. Choose a prompt from [`prompts/`](../prompts/README.md) and adapt only tool names and repository context that you can verify.
4. Give the agent a clear task, scope, and permission boundary. Do not put credentials in the prompt.
5. Run relevant scenarios from [`tests/`](../tests/README.md) and inspect the result yourself.

## Report a configuration

Copy [`profiles/TEMPLATE.md`](../profiles/TEMPLATE.md), replace placeholders with sanitized values, and mark the status accurately. Include exact versions and settings only when known. Do not infer success from a model name or available system memory.

## Suggested first checks

- Can the agent identify its workspace without changing directories unexpectedly?
- Can it find a definition and references without relying on incomplete output?
- Does it recover from a tool error while retaining the original objective?
- Does it distinguish an unverified suspicion from a confirmed finding?
- Does it stop at the agreed scope and verify completion?

See [`methodology.md`](methodology.md) for evidence and reporting requirements.
