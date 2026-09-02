# trippapi-ai-hq-pilot

**AI HQ Pilot: v1**

Pilot repository for the AI HQ agent integration. Used to validate the
GitHub App permission model end-to-end before touching any production repo.

## Scope

This repo is intentionally minimal. It exists so an AI agent (via a
scoped GitHub App) can:

- read repository metadata and contents
- push branches and commits
- open and update pull requests
- read check results

It explicitly **cannot** merge, administer, manage secrets, environments,
or Actions secrets.

## Branch policy

`main` is protected. All changes land through a pull request that passes
the `pilot-check` workflow.
