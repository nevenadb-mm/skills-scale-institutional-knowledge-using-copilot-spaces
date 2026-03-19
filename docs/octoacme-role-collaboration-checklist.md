# OctoAcme — Role Collaboration Checklist

This checklist supports cross-functional teams in aligning roles, managing handoffs, and maintaining clear ownership at each stage of the delivery lifecycle. Use it alongside the [Roles & Personas](./octoacme-roles-and-personas.md) reference doc.

---

## 1. Kickoff Role Alignment

Run this at project or major-feature kickoff to confirm every role is covered and informed.

- [ ] Project Manager has scheduled the kickoff meeting and shared the agenda
- [ ] Product Manager has prepared the one-pager and initial problem statement
- [ ] Business Analyst has reviewed stakeholder requirements and drafted initial user stories
- [ ] UX Designer has been briefed on user research goals and design scope
- [ ] DevOps/SRE has reviewed infrastructure and deployment requirements
- [ ] Support Lead has been informed of scope and potential customer impact areas
- [ ] All roles agree on the Definition of Done and acceptance-criteria standard
- [ ] RACI ownership confirmed for key artifacts (one-pager, backlog, risk register, design assets)
- [ ] Communication cadence (standups, syncs, demos) agreed and calendared

---

## 2. Design → Development Handoff

Complete before a backlog item moves from design to active development.

- [ ] UX Designer has delivered final design assets (wireframes, specs, annotated mockups) and linked them to the backlog item
- [ ] UX Designer has walked Developers through the design intent in a handoff session
- [ ] Acceptance criteria updated to include design/UX requirements
- [ ] Business Analyst has confirmed that the story still aligns with documented requirements
- [ ] Developers have acknowledged the design assets and raised any technical constraints
- [ ] Open design questions logged and assigned an owner and due date
- [ ] DevOps/SRE has reviewed for any new infrastructure or deployment considerations introduced by the feature

---

## 3. Release Readiness Roles

Run before deploying any Minor or Major release (see [Release & Deployment Guide](./octoacme-release-and-deployment.md)).

- [ ] **Developer**: all acceptance criteria met; PRs merged; CI green; unit and integration tests passing
- [ ] **Product Manager**: release approved; release notes reviewed
- [ ] **Project Manager**: deployment window confirmed; stakeholder communications prepared
- [ ] **UX Designer**: design acceptance criteria validated against the release candidate
- [ ] **DevOps/SRE**: staging smoke tests passing; rollback plan documented and tested; monitoring alerts configured
- [ ] **Business Analyst**: UAT completed and signed off (if applicable)
- [ ] **Support Lead**: release notes reviewed; support team briefed; knowledge base updated; customer communications drafted

---

## 4. Incident Escalation Roles

Use when a production incident is declared (see [Risks & Communication](./octoacme-risks-and-communication.md) for escalation paths).

| Step | Owner | Action |
|---|---|---|
| Detect | DevOps/SRE | Confirm incident; assess severity; page on-call |
| Triage | DevOps/SRE + Developer | Identify scope and immediate mitigation |
| Notify (internal) | Project Manager | Send initial incident communication to stakeholders |
| Communicate (customer) | Support Lead + Project Manager | Draft and send customer-facing status update |
| Mitigate | Developer + DevOps/SRE | Apply fix or initiate rollback |
| Resolve & update | Project Manager | Confirm resolution; send all-clear communication |
| Post-incident review | DevOps/SRE (facilitates) | Schedule and run blameless retrospective; log action items |

- [ ] Incident severity determined and communicated to the team within 15 minutes of detection
- [ ] Support Lead notified so customer communications can be prepared
- [ ] Product Manager informed of customer-facing impact
- [ ] Business Analyst updated if requirements changes are needed as a result
- [ ] Post-incident retrospective scheduled within 48 hours of resolution

---

## 5. Support Feedback Loop

Run at the end of each sprint or milestone to ensure customer insights flow back to the team.

- [ ] Support Lead has prepared a support metrics digest (ticket volume, CSAT, top issues)
- [ ] Digest shared with Product Manager and Project Manager before the planning meeting
- [ ] Recurring issues identified and converted into backlog candidates by Business Analyst or Product Manager
- [ ] DevOps/SRE reviewed for operational/reliability-related patterns in support tickets
- [ ] UX Designer informed of usability-related issues for design backlog consideration
- [ ] Agreed backlog additions communicated back to Support Lead to close the loop

---

## Reference Docs

| Document | Description |
|---|---|
| [Roles & Personas](./octoacme-roles-and-personas.md) | Full role definitions, RACI matrix, and lifecycle participation |
| [Project Initiation](./octoacme-project-initiation.md) | One-pager template and initiation checklist |
| [Project Planning](./octoacme-project-planning.md) | Backlog template, DoD, and planning checklist |
| [Execution & Tracking](./octoacme-execution-and-tracking.md) | Team rhythm, PR workflow, and blocker escalation |
| [Release & Deployment](./octoacme-release-and-deployment.md) | Deployment checklist and rollback playbook |
| [Risks & Communication](./octoacme-risks-and-communication.md) | Risk register, escalation paths, and communication templates |
| [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) | Retrospective structure and action item tracking |
