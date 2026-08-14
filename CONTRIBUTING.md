# Contributing to Ashmere Software Projects

Thank you for contributing to an Ashmere Software project.

Individual repositories may contain project-specific instructions. Where they do, those instructions take precedence over this organisation-wide default.

## Before you start

1. Search existing issues and pull requests.
2. For substantial architectural, security-sensitive or breaking changes, open an issue or discussion before investing significant work.
3. Never include production credentials, real secrets, private keys, customer data or other sensitive information in issues, commits, screenshots, logs or pull requests.
4. Keep changes focused. Unrelated refactors should normally be separate pull requests.

## Branches

Use short, descriptive branch names, for example:

- `feature/add-audit-export`
- `fix/session-rotation`
- `security/tenant-scope-check`
- `docs/deployment-guide`

Do not work directly on protected release branches unless the repository's documented process explicitly allows it.

## Commits

Write commits that explain the intent of the change. Prefer small, reviewable commits over large mixtures of unrelated work.

Where the repository enforces signed commits, contributors must satisfy that requirement before merge.

## Pull requests

Ashmere Software uses a detailed pull request template because pull requests are expected to be independently reviewed and security challenged before merge.

A pull request should:

- explain what changed and why;
- identify affected components and trust boundaries;
- document security, privacy and operational impact;
- include test evidence;
- disclose migrations, dependencies and compatibility changes;
- provide a reproducible red-team handoff;
- document rollback where a production change is involved.

Do not remove template sections merely because they are inconvenient. Use `N/A` with a short reason when a section genuinely does not apply.

## Testing

Run the repository's documented test, lint, type-check and build commands before requesting review.

New behaviour should normally have automated coverage. Security fixes should include a regression test where practical.

Reviewers may ask for additional adversarial tests, including authentication bypass, authorisation bypass, tenant crossover, injection, replay, concurrency, unsafe file handling, secret leakage, dependency risk and business-logic abuse.

## Security

Do not open a public issue for a vulnerability that could put users or deployments at risk.

Follow the repository's `SECURITY.md` and, where enabled, use GitHub Private Vulnerability Reporting.

## Code quality

Contributions should favour:

- explicit security boundaries;
- least privilege;
- server-side authorisation;
- safe defaults;
- clear validation at trust boundaries;
- deterministic migrations;
- useful auditability;
- graceful failure;
- readable code over clever code;
- tests that prove behaviour rather than only implementation details.

## Documentation

Update documentation when a change affects:

- installation;
- configuration;
- environment variables;
- APIs or protocols;
- permissions;
- deployment;
- security behaviour;
- operator workflows;
- user-facing behaviour.

## Review and merge

A pull request is not considered ready merely because it builds.

Repositories may require CI, code review, red-team/security review, resolved conversations, migration review and other branch/ruleset checks before merge.

Maintainers may close changes that are unsafe, unmaintainable, out of scope or incompatible with the project's direction.

## Licence

By contributing, you agree that your contribution may be distributed under the licence used by the repository receiving the contribution.
