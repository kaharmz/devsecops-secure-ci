# Day 3 – Secret Detection & CI Guardrails

## Objective
Prevent secret leakage using local and CI-based scanning.

## Controls Implemented
- Gitleaks pre-commit hook (filesystem scan)
- Gitleaks CI scan via GitHub Actions
- Custom secret detection rules (.gitleaks.toml)
- Signed commits
- Pull request with mandatory review

## Evidence
- Commit blocked locally when secret detected
- CI fails if secret exists in PR
- Reviewer approval required before merge

## Security Value
- Preventive: pre-commit hook
- Detective: CI scanning
- Governance: branch protection & review
- Audit-ready DevSecOps workflow
