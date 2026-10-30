# Repository contribution guidance

- Keep playbooks composable, scoped, and explicit about required tools and permissions.
- Apply [rules/evidence-policy.md](rules/evidence-policy.md) to all findings and compatibility claims.
- Preserve the user's active task through tool failures; follow [rules/tool-failure-recovery.md](rules/tool-failure-recovery.md).
- Default to read-only inspection. Request explicit authorization before destructive or externally visible actions.
- Never add real credentials, private URLs, corporate information, or personal workstation secrets. Use placeholders and sanitized examples.
- Mark untested hardware/model combinations **Experimental / Untested** and single-source reports **Community Reported**. Do not invent benchmark numbers.
- Keep shared rules and prompts agent-tool-agnostic; put tool-specific placement in `docs/integrations.md`.
- Keep each prompt portable; state assumptions and tell agents to use only tools actually available.
- Update relevant tests and documentation when changing a policy.
