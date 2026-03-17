# OctoAcme Project Management Processes

This repository documents the project management practices and workflows for OctoAcme teams. These living, collaborative guidelines centralize and standardize how projects are initiated, planned, tracked, delivered, and improved.

## Overview

OctoAcme project management is based on clear, iterative, and transparent practices, refined through experience and aimed at delivering customer value. These processes support onboarding, reduce dependency risks, and enable consistent execution.

### Project Lifecycle Stages

1. **Initiation**
   - Validate business need and outcomes.
   - Identify stakeholders & champions.
   - Select go/no-go for planning based on a Project One-Pager.

2. **Planning**
   - Break work into increments with clear acceptance criteria.
   - Estimate, identify dependencies and risks.
   - Define “Definition of Done”, release plan, and risk register.

3. **Execution & Tracking**
   - Use a workflow-based project board (Backlog → Done).
   - Pull requests link to issues, pass CI, and follow code review policies.
   - Run tests and QA at multiple levels (unit, integration, E2E).

4. **Release & Deployment**
   - Release types: Patch, Minor, Major.
   - Pre-release: Criteria met, CI passing, release notes, rollback plan.
   - Deploy to staging → production, run smoke tests, post-deploy verifications.

5. **Retrospective & Continuous Improvement**
   - After each sprint, release, or incident: capture learnings and action items.
   - Track improvements and update docs/processes as needed.

6. **Risk Management & Communication**
   - Maintain a risk register and escalate issues as needed.
   - Communicate status, blockers, and incidents with clear templates.

### Roles & Responsibilities

- **Project Manager (PM):** Coordinates delivery, timelines, risks, and comms.
- **Product Manager (PdM):** Defines product outcomes and prioritizes backlog.
- **Developers:** Build, test, and deliver features.
- **QA:** Ensure quality and acceptance.
- **Stakeholders:** Provide input and approval.

### Resources

- Process docs in this folder detail each lifecycle phase, workflow checklist, and role.
- Issue templates are provided for process doc improvements and content updates.

---

For more details, see the individual process files and templates within this `docs/` folder and `.github/ISSUE_TEMPLATE/`.
