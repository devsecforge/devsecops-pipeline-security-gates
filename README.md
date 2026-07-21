# 🔐 DevSecOps Pipeline Security Gates

*By S. Naz · Cybersecurity, Cloud & AI Security Leader*

Reusable CI/CD security gates — SAST, SCA, IaC scanning, and policy checks — that block insecure code before it merges, not after it ships.

![CI/CD](https://img.shields.io/badge/CI/CD-2088FF&logo=githubactions&logoColor=white?style=flat-square) ![SAST](https://img.shields.io/badge/SAST-D22730?style=flat-square) ![Policy as Code](https://img.shields.io/badge/Policy_as_Code-1F4E79?style=flat-square) ![DevSecOps](https://img.shields.io/badge/DevSecOps-00A36C?style=flat-square)

## What's Inside

- Reusable GitHub Actions workflows for SAST, dependency (SCA) scanning, and IaC scanning (tfsec/checkov)
- Policy-as-code gate using OPA — merges block on policy violations, not just on scanner noise
- Severity-based gating: critical findings block the merge, low findings surface as PR comments
- Baseline suppression file so legacy findings don't drown out new ones

## Key Practices

- Gates run on every PR, not just on a nightly schedule — feedback lands before merge, not after
- False-positive suppressions require a written justification tied to a ticket

## Status

- Actively maintained — adding secret-scanning as a first-class gate.

---

*Part of the [devsecforge](https://github.com/devsecforge/devsecforge) open security program — framework-mapped, hands-on, and actively growing.*
