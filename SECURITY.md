# Security policy

## Reporting a vulnerability

Do not open a public issue. Report privately through GitHub's private
vulnerability reporting on this repository:
https://github.com/tahto-app/.github/security/advisories/new — it covers
every Tahto repository. Alternatively use the contact address on
https://tahto.app.

We aim to acknowledge within 2 business days and to give a remediation
timeline within 7 days. Please include reproduction steps and the affected
component.

## Scope

All software published by Tahto: the mobile app, its backend and the
website.

## Handling secrets

Never commit credentials. `.env` files are ignored in every repository; only
`.env.example` with empty values is tracked. A secret that reaches a commit,
even on a branch, is rotated — history rewriting is not a substitute.
