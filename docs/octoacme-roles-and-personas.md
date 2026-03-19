# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## UX Designer

### Role Summary
UX Designers own the end-to-end user experience: from research and discovery through wireframes, prototypes, and design validation. They ensure that solutions are usable, accessible, and aligned with user needs before and during development.

### Responsibilities
- Conduct user research and synthesize findings into design requirements
- Produce wireframes, prototypes, and final design assets for developer handoff
- Collaborate with Product Managers on solution discovery and feature scoping
- Partner with Developers during implementation to clarify design intent
- Validate delivered features with user testing and feed insights back to the backlog

### Goals
- Reduce usability issues discovered post-release
- Shorten the feedback loop between users and the delivery team
- Ensure accessibility and consistency across the product

### Typical Communication
- Design-review sessions with Product Managers and Developers
- Design-handoff notes (specs, annotated mockups) linked in the backlog item
- Usability test summaries shared with Product Managers and Project Managers

### Interactions with Existing Roles
| Phase | Interaction |
|---|---|
| Initiation | Partners with Product Manager to validate user needs for the one-pager |
| Planning | Delivers wireframes/prototypes for backlog items; assists with acceptance criteria |
| Execution | Reviews in-progress features with Developers; flags deviation from design intent via PR comments |
| Release | Validates release candidate against design acceptance criteria |
| Retrospective | Contributes usability findings and design-debt items as improvement actions |

---

## DevOps / SRE

### Role Summary
DevOps/SRE engineers own the build, release, and operations infrastructure. They drive reliability, observability, and automation, and are the primary responders during production incidents.

### Responsibilities
- Design and maintain CI/CD pipelines, deployment automation, and infrastructure-as-code
- Define and monitor SLIs/SLOs and system health dashboards
- Lead incident response: triage, mitigation, and post-incident review
- Champion reliability practices (chaos engineering, runbooks, on-call rotations)
- Collaborate with Developers on deployability and operational readiness of new features

### Goals
- Achieve and maintain agreed service reliability targets
- Reduce mean time to detect (MTTD) and mean time to recover (MTTR)
- Automate toil and improve deployment frequency and confidence

### Typical Communication
- Incident alerts and runbook updates shared with the team
- Deployment readiness sign-off communicated to Project Manager before each release
- SLO reports and post-incident summaries shared in weekly delivery syncs

### Interactions with Existing Roles
| Phase | Interaction |
|---|---|
| Initiation | Advises on infrastructure sizing and operational feasibility in the one-pager |
| Planning | Defines deployment strategy, environment requirements, and DoD readiness gates |
| Execution | Reviews PRs for operational concerns; maintains CI/CD health |
| Release | Owns deployment execution and rollback; coordinates deployment window with Project Manager |
| Retrospective | Leads post-incident retrospectives; proposes reliability improvements |

---

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business stakeholders and the delivery team. They gather and document requirements, map business processes, and ensure that user stories accurately reflect stakeholder intent.

### Responsibilities
- Elicit and document business requirements from stakeholders
- Translate requirements into user stories, scenarios, and acceptance criteria
- Map current and future-state business processes
- Facilitate requirements workshops and maintain traceability between business goals and backlog items
- Support UAT (User Acceptance Testing) planning and execution

### Goals
- Ensure delivered features solve the right business problem
- Reduce rework caused by misunderstood requirements
- Maintain clear traceability from business objectives to delivered stories

### Typical Communication
- Requirements workshops and walkthroughs with stakeholders and Product Managers
- User stories and process diagrams added to the backlog
- UAT status updates to Project Manager and Product Manager

### Interactions with Existing Roles
| Phase | Interaction |
|---|---|
| Initiation | Works with Product Manager and stakeholders to draft the problem statement and success metrics in the one-pager |
| Planning | Writes and refines backlog items; defines acceptance criteria alongside Product Manager |
| Execution | Answers Developers' clarifying questions; updates stories based on emerging findings |
| Release | Coordinates UAT with stakeholders; signs off on business acceptance |
| Retrospective | Highlights requirements-clarity improvements and process-mapping gaps |

---

## Support Lead

### Role Summary
The Support Lead is the primary liaison between customers and the delivery team. They triage incoming issues, track support KPIs, and ensure that recurring customer pain points are fed back into the product roadmap.

### Responsibilities
- Act as first point of contact for customer issues and escalate critical bugs to the development team
- Document, triage, and prioritize support tickets; maintain a support knowledge base
- Track support metrics (ticket volume, CSAT, time to resolution) and report trends
- Coordinate release announcements and customer communications with Project Manager and Product Manager
- Feed recurring customer issues into the backlog as candidate improvements

### Goals
- Reduce time to resolution for customer issues
- Decrease repeat tickets through proactive documentation and product fixes
- Improve CSAT and customer confidence in the product

### Typical Communication
- Weekly support metrics digest shared with Product Manager and Project Manager
- Critical incident escalation to DevOps/SRE and Project Manager
- Release announcement drafts co-authored with Product Manager

### Interactions with Existing Roles
| Phase | Interaction |
|---|---|
| Initiation | Provides customer pain-point data to inform the one-pager problem statement |
| Planning | Flags known support-heavy areas to be included in the risk register |
| Execution | Reports active customer escalations to Project Manager; validates bug fixes |
| Release | Reviews and approves customer-facing release notes; prepares support team for launch |
| Retrospective | Shares support ticket trends as data points for improvement actions |

---

## Role Participation Across Lifecycle Phases

| Role | Initiation | Planning | Execution | Release | Retrospective |
|---|---|---|---|---|---|
| Developer | Effort estimate | Backlog, DoD | Build & test | Deploy support | Improvement actions |
| Product Manager | One-pager, goals | Backlog priority, acceptance criteria | Feature decisions | Release approval | Product feedback |
| Project Manager | Plan, stakeholder alignment | Timeline, risk register | Tracking, escalation | Coordination | Facilitation |
| UX Designer | User needs validation | Wireframes, design acceptance criteria | Design review, handoff | UX acceptance | Usability findings |
| DevOps/SRE | Infra feasibility | Deployment strategy, DoD gates | CI/CD, code review | Deployment & rollback | Incident retrospective |
| Business Analyst | Problem statement, success metrics | User stories, acceptance criteria | Requirements clarification | UAT sign-off | Requirements-clarity improvements |
| Support Lead | Customer pain-point data | Risk register input | Escalation relay | Release notes, launch readiness | Support trend analysis |

---

## Who Owns What (Lightweight RACI)

> Key: **R** = Responsible (does the work) · **A** = Accountable (final sign-off) · **C** = Consulted · **I** = Informed

| Artifact / Activity | Developer | Product Manager | Project Manager | UX Designer | DevOps/SRE | Business Analyst | Support Lead |
|---|---|---|---|---|---|---|---|
| Project One-pager | C | A | C | C | C | C | I |
| Backlog & priorities | C | A/R | I | C | C | R | C |
| Definition of Done | R | C | A | C | R | C | I |
| Risk Register | C | C | A/R | I | C | I | C |
| Design assets & specs | C | C | I | A/R | I | I | I |
| CI/CD pipeline & infra | R | I | I | I | A/R | I | I |
| Release notes | C | A | C | I | C | C | R |
| Incident comms | C | I | A | I | R | I | C |
| Retrospective facilitation | C | C | A/R | C | C | C | C |
| Support knowledge base | I | C | I | I | I | C | A/R |

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- See [Role Collaboration Checklist](./octoacme-role-collaboration-checklist.md) for practical handoff and accountability guidance across the full delivery lifecycle.

