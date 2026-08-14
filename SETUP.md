# Ashmere Software GitHub Baseline

This repository is intended to become the public `AshmereSoftware/.github` repository.

## Included

- `profile/README.md` — organisation Overview
- `PULL_REQUEST_TEMPLATE.md` — concise PR handoff for independent red-team review
- `RED_TEAM_PROMPT.md` — reusable red-team prompt
- `CONTRIBUTING.md`
- `SECURITY.md`
- `SUPPORT.md`
- `GOVERNANCE.md`
- `CODE_OF_CONDUCT.md`
- `.github/ISSUE_TEMPLATE/bug_report.yml`
- `.github/ISSUE_TEMPLATE/feature_request.yml`
- `.github/ISSUE_TEMPLATE/documentation.yml`
- `.github/ISSUE_TEMPLATE/config.yml`

## Recommended repository protection

For important Ashmere repositories:

1. Require pull requests before merge.
2. Require at least one approval.
3. Dismiss stale approvals after reviewable changes.
4. Require all review conversations to be resolved.
5. Require CI checks.
6. Require a named red-team/security status check once automated.
7. Block force pushes on protected branches.
8. Consider requiring signed commits.
9. Enable Private Vulnerability Reporting on public repositories.
10. Add repository-specific CODEOWNERS for sensitive areas.

## Recommended red-team flow

Each PR should provide:

1. PR description from `PULL_REQUEST_TEMPLATE.md`.
2. Complete PR diff.
3. Repository/current code context.
4. Runnable authorised local/staging environment where practical.

Feed those into `RED_TEAM_PROMPT.md`.

The red team should review the exact current PR head SHA. Security-relevant commits pushed after review should invalidate or trigger re-review of the affected areas.
