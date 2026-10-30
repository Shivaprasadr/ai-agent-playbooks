# Safe development workflows

When changes are authorized:

1. Inspect the relevant files and existing conventions before editing.
2. Make the smallest complete change that addresses the request; preserve unrelated user changes.
3. Avoid destructive operations and changes outside the requested scope.
4. Run relevant tests, linters, or checks and report exact outcomes.
5. Review the diff for unintended changes and sensitive data.
6. Do not claim behaviour is verified beyond the checks actually run.

Use placeholders and sanitized examples. Do not add credentials, private URLs, corporate information, or personal workstation secrets.
