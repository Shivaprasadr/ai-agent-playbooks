# Git safe.directory

**Symptom:** Git reports that a repository is owned by a different user or is not a safe directory.

**Check:** Verify the intended repository path and its ownership using trusted local information. Do not disable Git's ownership protection globally or trust an unknown path.

**Recovery:** Follow the workstation administrator's approved process for correcting ownership or adding a narrowly scoped trusted directory. Do not change global Git configuration automatically. If unresolved, report that Git-based inspection is unavailable and continue with safe file-based checks where possible.
