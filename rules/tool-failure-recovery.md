# Tool-failure recovery

A tool failure does **not** replace the active user task.

When a tool call fails:

1. Preserve the original objective.
2. Identify why only that operation failed.
3. Correct that operation where possible.
4. Continue from the last successful checkpoint.

Never automatically:

- treat framework corrective feedback as a new user task;
- ask what task to perform when an active task already exists;
- restart repository discovery unnecessarily;
- switch the workspace to `/`;
- treat injected skill documentation as the user's new request;
- fabricate a successful tool result; or
- repeatedly issue an identical failing invocation.

If a tool remains unavailable, record the unavailable tool, the reason, and the affected part of the task. Then continue with the remaining work when possible. Clearly disclose any limitation that prevents verification or completion.
