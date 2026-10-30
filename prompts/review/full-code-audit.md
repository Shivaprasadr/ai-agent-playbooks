# Full code audit

Audit the explicitly requested scope for concrete correctness, reliability, and security defects. This is a bounded review, not a claim that the entire system is defect-free.

1. Confirm scope and inspect the current source, definitions, and relevant references.
2. Trace the relevant paths and use tests or checks where reasonably possible.
3. Follow the [evidence policy](../../rules/evidence-policy.md). Do not report inferred absence or rely on truncated output.
4. Report each confirmed issue with severity, file, line/function, evidence tool/command, relevant evidence, impact, and a focused recommendation.
5. Separate confirmed findings from unverified hypotheses. Retract any finding contradicted by later evidence.
6. Summarize scope, files examined, checks run, and limitations.

Do not change files. Scope: `<SCOPE>`
