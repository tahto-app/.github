# Contributing

- Branch from `main`. Every change reaches `main` through a pull request; no
  direct pushes.
- One PR = one concern. Squash merge; the PR title becomes the commit subject.
- CI must be green: typecheck / build, `npm audit --audit-level=high`, secret
  scan (gitleaks).
- A change touching auth, payments, brokerage, KYC, database schema or CI
  permissions is security-relevant: tick the box in the PR template and
  request review from a second owner.
- Rollback procedures: see `tahto-infra/runbooks`.
