# Security Policy

Security issues should be reported privately.

## Do not report exploitable vulnerabilities in public issues

If a vulnerability could expose data, bypass authentication or authorisation, cross a tenant boundary, compromise infrastructure, leak secrets, enable code execution or otherwise put users at risk, do **not** publish exploit details in a normal GitHub issue.

## Preferred reporting method

Where the repository has **GitHub Private Vulnerability Reporting** enabled:

1. Open the repository.
2. Select **Security**.
3. Open **Advisories**.
4. Choose **Report a vulnerability**.
5. Provide a clear, reproducible report.

If private vulnerability reporting is not enabled, contact the repository maintainers privately using the project-specific security contact published in that repository or on the official Ashmere Software website.

Do not send secrets or sensitive exploit evidence through public channels.

## What to include

A useful report should contain:

- affected repository and version/commit;
- vulnerability class;
- required attacker access;
- step-by-step reproduction;
- expected versus actual security behaviour;
- impact;
- affected endpoints/components;
- proof-of-concept evidence where safe;
- suggested mitigation if known.

Please remove credentials, personal data and unrelated sensitive information.

## Coordinated disclosure

Please allow maintainers reasonable time to validate, remediate and release a fix before public disclosure.

We may ask for additional reproduction information, test environment details or confirmation against a patched build.

## Scope

Security scope is repository-specific. A project may publish additional rules in its own `SECURITY.md`; those rules override this default.

Unless a project explicitly authorises it, do not:

- test production systems without permission;
- access or modify data belonging to other users;
- perform denial-of-service testing;
- intentionally persist access;
- use social engineering;
- exfiltrate secrets or data beyond what is necessary to demonstrate impact;
- target third-party services that are outside Ashmere Software's control.

## Security fixes

Security fixes should normally include a regression test and should follow the same pull-request review process as other changes, including independent security/red-team review where applicable.
