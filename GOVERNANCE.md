# Ashmere Software Project Governance

This document describes the default governance model for Ashmere Software repositories. Individual projects may override it with their own governance file.

## Maintainers

Maintainers are responsible for the technical and security integrity of the repositories they manage.

Their responsibilities include:

- reviewing and merging pull requests;
- maintaining release quality;
- enforcing security and contribution requirements;
- responding to vulnerability reports;
- keeping dependencies and supported versions under review;
- documenting major architectural or governance decisions.

## Decision making

Routine implementation decisions may be made through normal pull-request review.

Changes with significant architectural, security, compatibility, licensing or governance impact should be documented before merge, normally in an issue, design note, RFC or the pull request itself.

Where maintainers disagree, the safest reversible option should generally be preferred while the decision is escalated to the project lead/owner.

## Security authority

Security review can block a merge.

Critical or High security findings should not be bypassed informally. If a risk must be accepted, the acceptance should be explicit, attributable, time-bounded where appropriate, and linked to follow-up work.

## Releases

Release authority is project-specific. A release should not be cut from a commit that fails required branch/ruleset protections or has unresolved blocking security findings.

## Changes to governance

Material changes to project governance should be reviewed like any other significant change and recorded in version control.
