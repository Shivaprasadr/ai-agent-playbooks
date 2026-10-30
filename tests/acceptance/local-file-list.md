# Local file list

**Purpose:** Check bounded file discovery.

**Setup:** In a test workspace, create a small directory with known filenames, including a nested directory.

**Expected:** The agent lists the requested directory using an available file tool, reports only observed names, respects the requested scope, and does not claim that unlisted nested files are absent unless it searched recursively.

**Record:** Directory scope, tool, output, and any truncation.
