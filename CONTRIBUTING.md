# Contributing

Thank you for helping make agent workflows more reliable and reproducible.

## What is useful

- Small, composable rules and prompts with clear scope.
- Reproducible acceptance scenarios and troubleshooting guidance.
- Hardware/model/runtime profiles with exact sanitized settings and honest limitations.
- Corrections to claims that lack evidence or have become outdated.

## Before opening a pull request

1. Search for an existing rule, prompt, or profile to extend instead of duplicating it.
2. Keep examples sanitized. Use placeholders such as `<YOUR_LOCAL_MODEL>` and `https://example.invalid`; never add PATs, API keys, real credentials, private URLs, corporate information, or personal workstation secrets.
3. Label untested claims **Experimental / Untested**. Label a single contributor's observation **Community Reported** until it has been independently reproduced.
4. Include enough context to reproduce a result: software/runtime versions, model identifier and quantization, relevant hardware class, settings, test steps, expected result, observed result, and limitations.
5. Follow the [evidence policy](rules/evidence-policy.md). A model's reasoning or documentation claim alone is not evidence.
6. Update related documentation and acceptance tests when behaviour or guidance changes.

## Profiles and benchmark claims

Do not invent benchmark numbers or describe an untested combination as proven. Distinguish measured facts from observations and hypotheses. Include dates and environment details where useful, but omit hostnames, usernames, serial numbers, network addresses, and other identifying details. Use the [profile template](profiles/TEMPLATE.md).

## Pull requests

Keep changes focused. Explain the problem, the proposed change, how it was checked, and any known limitations in the [pull request template](.github/PULL_REQUEST_TEMPLATE.md). Documentation-only changes generally need no automated validation, but check links and examples manually.

## Reporting issues

Use the issue templates where possible. Do not paste secrets or sensitive logs into public issues. Redact identifying and confidential data before sharing diagnostic output.
