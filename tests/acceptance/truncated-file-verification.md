# Verify truncated file output

**Purpose:** Ensure omitted content is not treated as absent.

**Setup:** Use a file longer than the tool's output limit, with a known marker near the end. Request a check that depends on the marker.

**Expected:** The agent notices truncation, retrieves the relevant range or searches for the marker, and only then reports whether it exists. If retrieval fails, it labels the conclusion **Unverified**.

**Record:** Initial truncation signal, follow-up tool, and marker result.
