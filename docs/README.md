# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management Docs. This README is the canonical entry point for project-level processes, templates, and guidance used across OctoAcme projects. It explains who owns what, how we run work, and where to find detailed process documents.

OctoAcme runs projects using a lightweight, iterative lifecycle that emphasizes clear artifacts and measurable outcomes. Work starts with a Project One-pager to capture the problem, objective, success metrics, stakeholders, and a high-level timeline. From there teams move through planning (kickoff, prioritized backlog, estimates, Definition of Done) into execution (build, test, review) and on to release and retrospective. Key living artifacts—one-pager, roadmap/release plan, sprint backlog, acceptance criteria, and a risk register—are maintained in the project repo so status and decisions remain a single source of truth.

Day-to-day execution is organized around a simple project-board workflow (Backlog → Ready → In Progress → In Review → QA → Done) and timeboxed sprints. Backlog items follow a template (title, description, acceptance criteria, priority, estimate, owner) and the pull-request workflow prioritizes small, reviewable changes, requires issue links and acceptance criteria in PRs, and mandates CI linting/tests plus at least one approval before merging. Releases follow a checklist (staging smoke tests, passing CI/security scans, release notes, rollback plan) with an explicit deployment and post-deploy verification process.

Roles are well defined: Product Managers own problem definition and prioritization; Project Managers coordinate delivery, schedules, risks, and stakeholder communication; Developers implement features and tests; QA validates acceptance criteria and performs manual or automated checks; stakeholders provide inputs and approvals. Communication is cadence-driven and transparent: short daily standups, weekly delivery syncs, reviews/demos at sprint end, and monthly stakeholder updates. Quality assurance is layered—unit and integration tests, end-to-end smoke checks, CI security scanning, and manual QA—combined with acceptance criteria and Definition of Done to ensure features are releasable and observable.

## Process Documents

- [Project Management Overview](octoacme-project-management-overview.md)
- [Project Initiation Guide](octoacme-project-initiation.md)
- [Project Planning Guide](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment Guide](octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
- [Personas and Roles](octoacme-roles-and-personas.md)

## Acceptance Criteria

- [x] Content aligns with existing process docs
- [x] Update improves clarity or closes a documented gap
- [x] Proposed content has been reviewed with stakeholders (if needed)
