# OctoAcme Role Collaboration Checklist

## Purpose
This document provides practical frameworks, checklists, and RACI matrices to facilitate cross-team collaboration and clarify handoff points between roles. Use this alongside the [Roles and Personas](./octoacme-roles-and-personas.md) document for day-to-day coordination.

---

## RACI Matrix for Key Activities

Use this matrix to quickly identify who is **Responsible**, **Accountable**, **Consulted**, and **Informed** for major project activities.

| Activity | Project Manager | Product Manager | Developer | QA Lead | Release Coordinator | Change Manager | Stakeholder Liaison |
|----------|----------------|-----------------|-----------|---------|---------------------|----------------|---------------------|
| **Project Initiation** | A | R | I | I | I | I | C |
| **Backlog Prioritization** | C | A/R | C | I | I | C | C |
| **Sprint Planning** | A | C | R | C | I | I | I |
| **Feature Development** | I | I | A/R | C | I | I | I |
| **Code Review** | I | I | A/R | C | I | I | I |
| **Test Planning** | C | C | C | A/R | I | I | I |
| **Test Execution** | I | I | C | A/R | I | I | I |
| **QA Sign-off** | I | I | I | A/R | C | I | I |
| **Change Request Evaluation** | C | C | C | C | I | A/R | C |
| **Scope Change Approval** | C | A | I | I | I | R | C |
| **Release Planning** | C | C | C | C | A/R | I | I |
| **Deployment Execution** | I | I | C | C | A/R | I | I |
| **Release Communication** | C | I | I | I | C | I | A/R |
| **Stakeholder Updates** | C | C | I | I | I | I | A/R |
| **Risk Management** | A/R | C | C | C | C | C | C |
| **Retrospectives** | A | C | R | R | R | R | C |

**Legend:**
- **R** = Responsible (does the work)
- **A** = Accountable (ultimate ownership, approves)
- **C** = Consulted (provides input)
- **I** = Informed (kept up to date)

---

## Key Handoff Checklists

### 1. Requirements to Development Handoff

**From: Product Manager → To: Developers**

- [ ] Feature specifications documented with clear acceptance criteria
- [ ] User stories prioritized in backlog
- [ ] Success metrics defined
- [ ] Product Manager available for questions during implementation

**Quality Assurance Lead consulted on:**
- [ ] Testability of acceptance criteria
- [ ] Test data requirements

**Change Manager informed of:**
- [ ] Initial scope baseline for change control

---

### 2. Development to QA Handoff

**From: Developers → To: QA Lead**

- [ ] Feature implemented and code merged to staging branch
- [ ] Unit tests passing
- [ ] PR description includes testing notes and edge cases
- [ ] Known limitations documented
- [ ] Test environment ready with required data/configuration

**QA Lead validates:**
- [ ] Feature meets acceptance criteria
- [ ] Integration tests executed successfully
- [ ] Defects logged and prioritized

**Project Manager informed of:**
- [ ] QA progress and any blockers
- [ ] Timeline impacts from defects

---

### 3. QA Sign-off to Release Handoff

**From: QA Lead → To: Release Coordinator**

- [ ] All acceptance criteria validated
- [ ] Critical and high-priority defects resolved
- [ ] Regression testing completed
- [ ] Test summary report provided
- [ ] **QA Sign-off formally granted**

**Release Coordinator validates:**
- [ ] QA sign-off received
- [ ] Release notes reviewed
- [ ] Rollback plan in place

**Stakeholder Liaison prepared with:**
- [ ] Release announcement draft
- [ ] Known issues summary for stakeholder communication

---

### 4. Release Coordination Checklist

**Release Coordinator ensures:**

**Pre-Release:**
- [ ] QA sign-off obtained from QA Lead
- [ ] Release window scheduled and communicated
- [ ] Deployment checklist reviewed with DevOps
- [ ] Stakeholder Liaison notified of release timing
- [ ] Rollback procedures confirmed
- [ ] Change Manager confirms no pending scope changes

**During Release:**
- [ ] Deployment executed per checklist
- [ ] Post-deployment smoke tests coordinated with QA Lead
- [ ] Monitoring in place for errors/performance
- [ ] Project Manager updated on deployment status

**Post-Release:**
- [ ] Release announcement sent via Stakeholder Liaison
- [ ] Release metrics captured
- [ ] Project Manager informed of release success/issues
- [ ] Post-release retrospective scheduled

---

### 5. Change Management Handoff

**When a change request is submitted:**

**Change Manager coordinates:**
- [ ] Change request documented (requester, description, rationale)
- [ ] Impact assessment conducted:
  - [ ] Consult Developers on technical feasibility and effort
  - [ ] Consult QA Lead on testing impact
  - [ ] Consult Project Manager on schedule/resource impact
  - [ ] Consult Product Manager on priority and business value
- [ ] Change approval obtained (per governance process)
- [ ] All affected parties informed of approved change:
  - [ ] Project Manager updates project plan
  - [ ] Developers update backlog and estimates
  - [ ] QA Lead updates test plans
  - [ ] Stakeholder Liaison notifies stakeholders
- [ ] Change log updated

---

### 6. Stakeholder Communication Workflow

**Stakeholder Liaison manages:**

**Weekly Updates:**
- [ ] Gather status from Project Manager
- [ ] Gather quality/risk info from QA Lead
- [ ] Gather release schedule from Release Coordinator
- [ ] Gather change impacts from Change Manager
- [ ] Translate to stakeholder-appropriate language
- [ ] Distribute via agreed channels
- [ ] Capture stakeholder feedback/questions
- [ ] Route feedback to appropriate project team members

**Escalations:**
- [ ] Receive escalation from stakeholder
- [ ] Brief Project Manager immediately
- [ ] Facilitate rapid response
- [ ] Follow up with stakeholder on resolution

---

## Cross-Role Collaboration Best Practices

### Daily Collaboration Patterns

1. **Developers ↔ QA Lead**
   - Daily: Share build status and testing progress
   - As needed: Collaborate on reproducing and fixing defects
   - Sprint boundary: Review test coverage and quality trends

2. **Project Manager ↔ All Roles**
   - Daily standup: Gather progress, blockers, dependencies
   - Weekly: Review risk register with all roles
   - Sprint/milestone: Facilitate planning and retrospectives

3. **Release Coordinator ↔ QA Lead**
   - Pre-release: Validate quality gates met
   - During release: Coordinate smoke testing
   - Post-release: Review release metrics

4. **Stakeholder Liaison ↔ Product Manager**
   - Weekly: Align on customer/stakeholder feedback
   - As needed: Clarify requirements from stakeholders
   - Monthly: Joint stakeholder reviews

### Escalation Paths

```
Normal Flow:
Individual Role → Project Manager → Product Manager → Sponsor

Quality Issues:
Developer → QA Lead → Project Manager → Product Manager

Stakeholder Concerns:
Stakeholder → Stakeholder Liaison → Project Manager → appropriate role

Scope Changes:
Any Role → Change Manager → Project Manager/Product Manager → Approval Authority

Release Issues:
Release Coordinator → Project Manager + QA Lead → Incident Response
```

---

## Meeting Coordination

### Who Should Attend What

| Meeting | PM | PdM | Dev | QA Lead | Rel Coord | Change Mgr | Stakeholder Liaison |
|---------|----|----|-----|---------|-----------|------------|---------------------|
| Daily Standup | A | O | R | R | O | O | O |
| Sprint Planning | A | R | R | R | O | C | O |
| Sprint Review/Demo | A | R | R | C | O | O | C |
| Retrospective | A | C | R | R | R | R | C |
| Risk Review | A | C | C | R | C | C | C |
| Release Readiness | C | C | C | R | A | I | I |
| Change Control Board | C | C | C | C | I | A | C |
| Stakeholder Updates | C | C | O | O | O | O | A |

**Legend:**
- **A** = Accountable/leads the meeting
- **R** = Required attendee
- **C** = Consulted, should attend if available
- **O** = Optional
- **I** = Informed of outcomes but doesn't attend

---

## Quick Reference: Who to Contact For...

- **Project Status**: Project Manager
- **Feature Priority Questions**: Product Manager
- **Technical Implementation**: Developers
- **Quality/Testing Status**: QA Lead
- **Release Schedule**: Release Coordinator
- **Scope Change Requests**: Change Manager
- **Stakeholder Concerns**: Stakeholder Liaison
- **Risk or Blockers**: Project Manager (coordinates resolution)

---

## Templates for Handoff Communications

### Developer → QA Handoff Email Template
```
Subject: Ready for QA: [Feature Name]

Hi [QA Lead],

Feature [Name] is ready for testing.

- PR Link: [link]
- Acceptance Criteria: [link or summary]
- Test Environment: [staging URL or details]
- Test Data: [any specific test accounts or data needed]
- Known Limitations: [list any known issues]
- Expected Completion: [when you need QA sign-off]

Let me know if you have questions!
```

### QA → Release Coordinator Sign-off Template
```
Subject: QA Sign-off: [Feature Name]

Hi [Release Coordinator],

QA testing is complete for [Feature Name].

✅ **QA SIGN-OFF GRANTED**

- All acceptance criteria validated
- Critical defects: None
- High-priority defects: None
- Medium defects: [X resolved, Y deferred to post-release]
- Test Summary: [link to test report]

Ready for release coordination.
```

### Change Manager → Team Change Notification Template
```
Subject: Approved Change: [Change ID] - [Brief Description]

Team,

The following change has been approved:

- Change ID: [ID]
- Description: [summary]
- Approved By: [authority]
- Impact:
  - Scope: [description]
  - Schedule: [impact on timeline]
  - Resources: [impact on team/resources]
  
Action Items:
- [Project Manager]: Update project plan by [date]
- [Developers]: Update sprint backlog by [date]
- [QA Lead]: Adjust test plan by [date]
- [Stakeholder Liaison]: Communicate to stakeholders by [date]

Full details: [link to change request]
```

---

## Continuous Improvement

This collaboration framework should be reviewed and updated based on:
- Retrospective feedback from project teams
- Identified handoff gaps or bottlenecks
- Organizational changes in roles or processes
- Lessons learned from project post-mortems

**Owners**: Project Manager coordinates reviews; Change Manager ensures updates are documented.
