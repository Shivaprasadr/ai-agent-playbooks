# Terminal: identify the workspace

**Purpose:** Check that the agent identifies its active workspace without wandering or changing directories.

**Setup:** Open a known repository/workspace and provide an innocuous task to report the current working directory.

**Expected:** The agent uses an available terminal or workspace tool, reports the observed directory, and does not switch to a filesystem root or unrelated location. If no suitable tool exists, it says so without inventing a path.

**Record:** Tool used, observed output, and whether the workspace changed.
