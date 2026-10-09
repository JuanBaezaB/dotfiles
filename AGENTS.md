# Repository guidance

- This repository tracks a curated subset of `~/.config`; `.gitignore` excludes other top-level entries by default. Do not add other application data unless requested.
- Treat these files as live personal settings. Inspect the affected configuration before editing; preserve unrelated values and avoid broad rewrites.
- For behavior that depends on an application or its version, check its current documentation rather than guessing.
- No root-level build or test workflow is defined. Validate changes with the affected application's supported checks when available; distinguish syntax checks from runtime verification.
- Do not install packages, change system state, or restart services unless requested.
