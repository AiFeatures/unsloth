# Fork Customizations

> Upstream: [unslothai/unsloth](https://github.com/unslothai/unsloth)
> Fork maintained by: @ashsolei
> Last reviewed: 2026-04-08
> Fork type: **active-dev**
> Sync cadence: **monthly**

## Purpose of Fork

Unsloth fine-tuning fork; iAiFy carries local patches for enterprise training pipelines.

## Upstream Source

| Property | Value |
|---|---|
| Upstream | [unslothai/unsloth](https://github.com/unslothai/unsloth) |
| Fork org | AiFeatures |
| Fork type | active-dev |
| Sync cadence | monthly |
| Owner | @ashsolei |

## Carried Patches

Local commits ahead of `upstream/main` at last review:

- `25bb43f5 chore(deps): bump transformers (#2)`
- `bc77b239 chore: sync CLAUDE.md and copilot-instructions docs`
- `90fb3ff9 ci: add github-actions ecosystem to dependabot`
- `d3ba94cd docs: update FORK-CUSTOMIZATIONS.md with upstream source`
- `732ee470 docs: add FORK-CUSTOMIZATIONS.md per enterprise fork governance`
- `eb955df5 ci: add copilot-setup-steps.yml for Copilot Workspace`
- `eb76a661 chore: add AGENTS.md`
- `3aee2029 chore: add CLAUDE.md`
- `d0a92de9 chore: add copilot-instructions.md`
- `75d1ce7f chore: add Copilot Coding Agent setup steps`
- `d0508660 chore: remove misplaced agent files from .github/copilot/agents/`
- `18a4a8df chore: deploy core custom agents from AgentHub`
- `dbfeba7e chore: deploy core Copilot agents from AgentHub`
- `23208289 docs: add FORK-CUSTOMIZATIONS.md`
- `54530316 chore: add dependabot.yml [governance-orchestrator]`
- `bfe642e7 chore: remove workflow stale.yml — enterprise cleanup`

## Supported Components

- Root governance files (`.github/`, `CLAUDE.md`, `AGENTS.md`, `FORK-CUSTOMIZATIONS.md`)
- Enterprise CI/CD workflows imported from `Ai-road-4-You/enterprise-ci-cd`

## Out of Support

- All upstream source directories are tracked as upstream-of-record; local edits to core source are discouraged.

## Breaking-Change Policy

1. On upstream sync, classify per `governance/docs/fork-governance.md`.
2. Breaking API/license/security changes auto-classify as `manual-review-required`.
3. Owner triages within 5 business days; conflicts are logged to the `fork-sync-failure` issue label.
4. Revert local customizations only after stakeholder sign-off.

## Sync Strategy

This fork follows the [Fork Governance Policy](https://github.com/Ai-road-4-You/governance/blob/main/docs/fork-governance.md)
and the [Fork Upstream Merge Runbook](https://github.com/Ai-road-4-You/governance/blob/main/docs/runbooks/fork-upstream-merge.md).

- **Sync frequency**: monthly
- **Conflict resolution**: Prefer upstream; reapply iAiFy customizations on a sync branch
- **Automation**: [`Ai-road-4-You/fork-sync`](https://github.com/Ai-road-4-You/fork-sync) workflows
- **Failure handling**: Sync failures create issues tagged `fork-sync-failure`

## Decision: Continue, Rebase, Refresh, or Replace

| Option | Current Assessment |
|---|---|
| Continue maintaining fork | yes - active iAiFy product scope |
| Full rebase onto upstream | feasible on request |
| Fresh fork (discard local changes) | not acceptable without owner review |
| Replace with upstream directly | not possible (local product value) |

## Maintenance

- **Owner**: @ashsolei
- **Last reviewed**: 2026-04-08
- **Reference runbook**: `ai-road-4-you/governance/docs/runbooks/fork-upstream-merge.md`
