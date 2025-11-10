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

## Quality Assurance Lead

### Role Summary
Quality Assurance Leads ensure that delivered software meets acceptance criteria, quality standards, and functional requirements. They coordinate testing activities, manage QA resources, and collaborate with developers and project managers to validate features before release.

### Responsibilities
- Define test strategy and test plans for projects
- Coordinate manual and automated testing activities
- Review acceptance criteria and validate feature completeness
- Report on quality metrics, test coverage, and defect trends
- Facilitate bug triage and coordinate retesting of fixes
- Ensure QA sign-off before releases

### Goals
- Prevent defects from reaching production
- Maintain comprehensive test coverage
- Reduce mean time to detect and resolve issues
- Enable fast, confident releases

### Typical Communication
- Daily coordination with developers on feature readiness
- Weekly quality reports to Project Manager and Product Manager
- Test plan reviews during sprint planning
- Bug triage meetings and defect status updates

### RACI Interactions
- **Accountable** for: QA sign-off, test execution, quality reports
- **Responsible** for: creating test plans, executing tests, defect management
- **Consulted** by: Developers (on testability), Project Managers (on release readiness), Release Coordinator (on quality gates)
- **Informed** by: Product Managers (on acceptance criteria changes), Change Manager (on scope changes impacting testing)

### Key Handoff Points
- **From Product Manager**: Receives acceptance criteria and feature specifications for test planning
- **To/From Developers**: Collaborates on test cases, receives builds for testing, reports defects
- **To Project Manager**: Reports quality status, risks, and blockers
- **To Release Coordinator**: Provides QA sign-off as prerequisite for release

---

## Stakeholder Liaison

### Role Summary
Stakeholder Liaisons bridge the gap between project teams and external stakeholders (executives, customers, partners, support teams). They ensure stakeholder needs are understood, expectations are managed, and communication flows effectively in both directions.

### Responsibilities
- Identify and maintain stakeholder register with communication needs
- Gather and communicate stakeholder requirements and feedback
- Schedule and facilitate stakeholder updates and decision-making forums
- Manage stakeholder expectations and address concerns proactively
- Translate technical updates into stakeholder-appropriate language
- Escalate stakeholder issues and dependencies to the project team

### Goals
- Maintain stakeholder satisfaction and engagement
- Ensure timely stakeholder input and approvals
- Minimize surprises and miscommunication
- Build trust and alignment across organizational boundaries

### Typical Communication
- Weekly stakeholder status updates and reports
- Monthly stakeholder review meetings
- Ad-hoc briefings for executive or customer escalations
- Communication templates for announcements and change notices

### RACI Interactions
- **Accountable** for: stakeholder satisfaction, external communication, managing expectations
- **Responsible** for: gathering stakeholder input, distributing status updates, facilitating stakeholder meetings
- **Consulted** by: Project Manager (on communication plans), Product Manager (on customer feedback), Change Manager (on change communications)
- **Informed** by: All project roles (for status updates to relay to stakeholders)

### Key Handoff Points
- **From Stakeholders**: Receives requirements, feedback, concerns, and approval decisions
- **To Product Manager**: Communicates stakeholder needs and priorities
- **To Project Manager**: Reports stakeholder risks, dependencies, and decision requirements
- **From Release Coordinator**: Receives release announcements to communicate to stakeholders
- **To/From Change Manager**: Coordinates messaging about scope or timeline changes

---

## Change Manager

### Role Summary
Change Managers coordinate and control changes to project scope, requirements, and deliverables. They ensure changes are evaluated, approved, and communicated systematically to minimize disruption and maintain project control.

### Responsibilities
- Facilitate change request assessment and impact analysis
- Coordinate Change Control Board (CCB) or approval processes
- Document approved changes and update project artifacts
- Communicate change impacts to all affected parties
- Track change metrics and trends
- Ensure scope changes align with project governance

### Goals
- Prevent uncontrolled scope creep
- Maintain project predictability and stability
- Ensure informed decision-making on changes
- Protect team velocity while accommodating necessary changes

### Typical Communication
- Change request reviews with Project Manager and technical leads
- Change impact summaries for stakeholders and sponsors
- Updated scope documentation and backlog adjustments
- Change log maintenance and reporting

### RACI Interactions
- **Accountable** for: change control process, scope integrity, change documentation
- **Responsible** for: evaluating change requests, facilitating approvals, updating artifacts
- **Consulted** by: Project Manager (on change impacts), Developers (on technical feasibility), Product Manager (on priority changes)
- **Informed** by: All roles who identify change needs or are affected by approved changes

### Key Handoff Points
- **From Any Role**: Receives change requests or identifies scope changes
- **To Project Manager**: Provides change impact analysis and recommendations
- **To Product Manager**: Seeks prioritization decisions for scope changes
- **To Developers**: Communicates approved changes affecting implementation
- **To QA Lead**: Notifies of changes impacting test plans
- **To Stakeholder Liaison**: Provides change information for stakeholder communication

---

## Release Coordinator

### Role Summary
Release Coordinators orchestrate the end-to-end release process, ensuring that deployments are planned, executed smoothly, and properly communicated. They coordinate across teams to manage release logistics, timing, and risk.

### Responsibilities
- Plan and schedule release windows and deployment activities
- Coordinate release readiness reviews and go/no-go decisions
- Manage release checklists and gate criteria
- Facilitate deployment execution and monitoring
- Coordinate rollback procedures if needed
- Ensure release documentation and announcements are complete
- Track release metrics and post-release health

### Goals
- Deliver successful, low-risk deployments
- Minimize deployment-related incidents
- Ensure smooth coordination across teams during releases
- Maintain release predictability and stakeholder confidence

### Typical Communication
- Release planning meetings with Project Manager and development team
- Pre-release readiness reviews with QA Lead and technical leads
- Deployment status updates during release windows
- Post-release reports and retrospectives

### RACI Interactions
- **Accountable** for: release execution, deployment success, release communication
- **Responsible** for: coordinating release activities, managing release checklist, executing deployments
- **Consulted** by: Project Manager (on release planning), QA Lead (on release readiness), Developers (on deployment procedures)
- **Informed** by: Change Manager (on last-minute changes), Stakeholder Liaison (on stakeholder concerns)

### Key Handoff Points
- **From Project Manager**: Receives release schedule and project milestones
- **From QA Lead**: Receives QA sign-off before proceeding with release
- **From Developers**: Receives deployment artifacts and procedures
- **To Operations/DevOps**: Hands off deployment packages and coordinates execution
- **To Stakeholder Liaison**: Provides release status for stakeholder communication
- **To Project Manager**: Reports release outcomes and any issues for retrospective

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- For role interactions and collaboration patterns, see [Role Collaboration Checklist](./octoacme-role-collaboration-checklist.md).

