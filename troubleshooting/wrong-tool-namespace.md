# Wrong tool namespace

**Symptom:** The agent invokes a plausible but unavailable tool or namespace.

**Check:** Inspect the tools actually exposed by the host. Do not guess at tool names or signatures.

**Recovery:** Use the matching available tool, or state the unavailable tool and affected operation. Preserve the task and proceed with alternate evidence sources where reasonable; do not fabricate results or repeat an identical failed invocation.
