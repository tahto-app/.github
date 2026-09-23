# Security policy

## Reporting a vulnerability

Do not open a public issue. Report privately through GitHub's
"Report a vulnerability" button on the affected repository, or email the
address listed on https://tahto.app.

We aim to acknowledge within 2 business days and to give a remediation
timeline within 7 days. Please include reproduction steps and the affected
component.

## Scope

All repositories in the `tahto-app` organisation. The backend (`tahto-api`)
handles authentication, payments and brokerage and is the highest-priority
target.

## Handling secrets

Never commit credentials. `.env` files are ignored in every repository; only
`.env.example` with empty values is tracked. A secret that reaches a commit,
even on a branch, is rotated — history rewriting is not a substitute.
