# Methodology

This project values repeatability over impressive claims. Results apply only to the recorded environment and test conditions.

## Evidence levels

- **Confirmed** — current-repository evidence was obtained using suitable tools, relevant definitions and references were checked, and an applicable test or check was run when reasonably possible.
- **Unverified** — evidence is incomplete, unavailable, stale, or based on inference. Do not present it as a finding.
- **Experimental / Untested** — a configuration or procedure has not been validated by the contributor.
- **Community Reported** — an observation is reported by a contributor but has not been independently reproduced.

These labels describe evidence status, not confidence in an LLM's narrative.

## Reproducible reports

Record the date, agent/runtime and version, model identifier and quantization when known, inference engine and version, relevant hardware class, context and generation settings, tool availability, test procedure, expected and observed results, and limitations. Use sanitized identifiers; omit secrets and host-specific details.

For quantitative results, describe the measurement method, units, number of runs, and variation. Do not compare results unless the test procedure and relevant conditions are sufficiently alike. Do not invent missing values; mark them unknown.

## Finding verification

Follow [`../rules/evidence-policy.md`](../rules/evidence-policy.md). In particular, never infer absence from partial or truncated output, and retract a finding when later evidence contradicts it.
