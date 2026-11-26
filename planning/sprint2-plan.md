# Sprint 2 — Reconstructed planning record

**Reconstructed on November 26, 2026, after implementation.** The original
Sprint 2 planning screenshot is unavailable. This document records the scope
supported by the current repository; it is not an original planning screenshot
and does not establish when sprint planning occurred.

## Goal

Validate every change automatically and add application security controls to
the Customer Accounts service.

| Work item | Acceptance criteria | Current evidence |
| --- | --- | --- |
| [Add continuous integration (#8)](https://github.com/aungpaingsoedev/devops-capstone-project/issues/8) | Run lint and tests automatically; require at least 95% coverage | `.github/workflows/ci-build.yaml`; passing CI |
| [Add security headers and CORS (#9)](https://github.com/aungpaingsoedev/devops-capstone-project/issues/9) | Configure Flask-Talisman and Flask-CORS; verify behavior with regression tests | `service/__init__.py`; security tests; commit `8136663` |

## Intended work sequence

1. Configure and validate the CI workflow.
2. Implement security controls and regression tests.
3. Run the complete suite and inspect response headers.
4. Record verified completion on the project board.

## Verification now available

The November 26 Tekton run `cd-pipeline-run-bffpc` passed all 29 tests with
95% coverage and completed all four pipeline stages. The CI and security
tracking issues were created retrospectively; both currently have Done status.

Original sprint dates, capacity, estimates, and a historical backlog snapshot
are not established by this reconstruction.
