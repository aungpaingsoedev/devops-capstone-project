# Sprint 3 — Reconstructed planning record

**Reconstructed on November 26, 2026, after implementation.** The original
Sprint 3 planning screenshot is unavailable. This document records the scope
supported by the current repository and lab; it is not an original planning
screenshot and does not establish when sprint planning occurred.

## Goal

Build the Customer Accounts container and run it successfully on Kubernetes.

| Work item | Acceptance criteria | Current evidence |
| --- | --- | --- |
| [Containerize the microservice (#6)](https://github.com/aungpaingsoedev/devops-capstone-project/issues/6) | Build an Accounts image and start the application on port 8080 | `Dockerfile`; successful Docker build |
| [Deploy to Kubernetes (#7)](https://github.com/aungpaingsoedev/devops-capstone-project/issues/7) | Provide a database and service configuration; verify a ready deployment and API response | OpenShift `accounts` deployment; PostgreSQL service; API response |

## Intended work sequence

1. Build and verify the application image.
2. Configure the database, deployment, and service in the lab.
3. Verify rollout, pod readiness, application logs, and an API response.
4. Record verified completion on the project board.

## Verification now available

On November 26 the `accounts` deployment reached 1/1 available replicas and
the Accounts API responded successfully. Tekton run `cd-pipeline-run-bffpc`
subsequently built the image and verified the deployment successfully.
Issues #6 and #7 currently have Done status.

Original sprint dates, capacity, estimates, and a historical backlog snapshot
are not established by this reconstruction.
