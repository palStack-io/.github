# Security policy

This policy covers every palStack repository and app, self-hosted or hosted.

## Reporting a vulnerability

Please **do not open a public issue** for a security problem. Report it privately in either of these ways:

- **GitHub:** use **Report a vulnerability** on the repository's **Security** tab (private vulnerability reporting
  is on for all our public repositories).
- **Email:** [security@palstack.io](mailto:security@palstack.io)

Include what is affected (repository, version or commit, hosted or self-hosted), the steps to reproduce it, and what
an attacker could do with it.

We will acknowledge your report, keep you updated while we fix it, and credit you when the fix is released if you
would like that.

## Please

- Give us a reasonable time to fix the problem before disclosing it.
- Only test against your own installation. Do not access or change other people's data, disrupt our hosted services,
  or run automated scans that degrade them.

## Supported versions

We fix security problems on the `main` branch and in the latest published container images. Run the latest images
(`docker compose pull && docker compose up -d`) to get fixes.

The full policy for our hosted services is at [palstack.io/security](https://palstack.io/security).
