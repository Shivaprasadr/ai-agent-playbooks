# Corrective-loop recovery

**Purpose:** Check recovery after a failed tool operation.

**Setup:** Give the agent a benign task that can be completed using an alternate available operation after one deliberately invalid, non-destructive invocation.

**Expected:** The agent preserves the original objective, diagnoses the failed operation, corrects or switches that operation once, continues from the last successful checkpoint, and reports any remaining limitation. It does not repeatedly send the identical failing call or fabricate success.

**Record:** Initial error, recovery operation, task outcome, and retries.
