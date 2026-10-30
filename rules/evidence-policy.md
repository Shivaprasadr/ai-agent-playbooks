# Evidence policy

Never classify a finding as **Confirmed** solely from:

- model reasoning or model memory;
- README or other documentation claims;
- partial source content;
- truncated tool output; or
- inferred absence.

## Before confirming a finding

1. Verify it against the current repository or other current target under review.
2. Use suitable tools such as `grep`, `rg`, `glob`, terminal commands, AST tooling, tests, or appropriate file tools.
3. Search definitions and references where relevant.
4. Obtain current file, line, or function evidence.
5. Run an applicable test or check where reasonably possible.

If tool output is truncated, do not infer that omitted content does not exist. Retrieve the missing content with targeted reads or searches.

If verification cannot be completed, set **Status = Unverified** and state what evidence is missing. Do not upgrade a claim because it sounds plausible.

Every **Confirmed** finding must contain:

- severity;
- file;
- line or function;
- evidence command or tool;
- relevant evidence;
- impact; and
- recommended fix.

If later evidence contradicts an earlier finding, explicitly retract the earlier finding and correct any summary that included it.
