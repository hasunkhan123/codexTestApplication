# Codex repo instructions (Git + PR hygiene)

## Branching / sync rules (must follow every time)
- Before making any changes, sync with the base branch:
  - `git fetch origin`
  - ensure you are based on `origin/main` (or the repo’s default base branch)
- Create a fresh branch off the latest base for every task/PR.

## Conflict avoidance
- Do not reformat files unless explicitly requested.
- Avoid touching unrelated files (especially index.html, package.json, lockfiles) unless required.
- Prefer minimal, surgical diffs.

## Pre-PR check
- If your branch is behind base, rebase on `origin/main` before opening the PR.
- If conflicts arise, resolve them locally during the rebase (don’t leave it for GitHub UI).
