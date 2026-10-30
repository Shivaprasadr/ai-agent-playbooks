# No tool call

**Symptom:** The agent describes an action but does not invoke an available tool.

**Check:** Confirm the task requires an observable operation, the tool is actually available, and permissions allow it. Ask for the next concrete operation, not a new task description.

**Recovery:** Restate the active objective and request one specific, bounded tool action. If the tool is unavailable, record that limitation and continue with other possible work. Do not claim the operation ran.
