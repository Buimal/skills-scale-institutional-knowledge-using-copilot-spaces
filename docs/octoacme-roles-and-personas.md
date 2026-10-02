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

### Interaction with Other Roles
- **With Technical Lead/Architect:** Receive technical guidance and architecture reviews
- **With QA/Testing Lead:** Collaborate on test coverage and acceptance criteria validation
- **With Project Manager:** Provide status updates and identify blockers

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

### Interaction with Other Roles
- **With Stakeholders/Sponsors:** Align on business objectives and priorities
- **With Project Manager:** Coordinate on timeline and release planning
- **With QA/Testing Lead:** Define acceptance criteria and quality standards

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

### Interaction with Other Roles
- **With Stakeholders/Sponsors:** Report progress and escalate blockers
- **With Product Manager:** Align on priorities and milestone planning
- **With Release Manager:** Coordinate release timelines and dependencies
- **With All Teams:** Facilitate standups, planning, and retrospectives

---

## QA/Testing Lead

### Role Summary
QA/Testing Leads ensure quality standards are met and coordinate testing efforts across the project lifecycle. They define test strategies, validate acceptance criteria, and manage testing workflows.

### Responsibilities
- Define test plans and QA approach for each feature or release
- Validate acceptance criteria and definition of done
- Coordinate manual and automated testing activities
- Identify quality gaps and report defects with clear reproduction steps
- Ensure test coverage aligns with risk and criticality
- Participate in release readiness reviews
- Advocate for test automation and continuous improvement

### Goals
- Deliver high-quality software that meets acceptance criteria
- Reduce bugs reaching production
- Provide clear quality signals to the team and stakeholders
- Improve testing efficiency through automation

### Typical Communication
- Sprint planning and sprint reviews
- Defect reports and quality metrics
- Release readiness verification
- Collaboration with developers on test automation and coverage
- Participation in planning discussions to understand acceptance criteria early

### Interaction with Other Roles
- **With Developers:** Collaborate on test coverage, automation, and quality gates
- **With Product Manager:** Clarify acceptance criteria and definition of done
- **With Release Manager:** Validate readiness for deployment and sign-off
- **With Project Manager:** Report quality metrics and risks

### Referenced in Process Documents
- [Execution & Tracking](octoacme-execution-and-tracking.md#quality--testing) — Quality and Testing section
- [Release & Deployment](octoacme-release-and-deployment.md#pre-release-requirements) — Pre-release validation

---

## Technical Lead/Architect

### Role Summary
Technical Leads provide architectural guidance, ensure technical feasibility, and help the team navigate complex technical decisions. They mentor developers and reduce technical risk.

### Responsibilities
- Review technical approach and architecture for new features
- Assess technical feasibility and propose solutions to complex problems
- Mentor developers and facilitate knowledge sharing
- Identify technical risks and propose mitigations
- Guide code quality standards and best practices
- Participate in design reviews and technical spikes
- Ensure scalability, maintainability, and performance considerations

### Goals
- Ensure solutions are scalable, maintainable, and performant
- Reduce technical debt and rework
- Build team technical capability
- De-risk complex technical initiatives

### Typical Communication
- Design reviews and technical spike discussions
- Code review feedback and mentoring
- Architecture documentation and decisions
- Technical risk assessments during planning
- Knowledge-sharing sessions and pair programming

### Interaction with Other Roles
- **With Developers:** Provide architectural guidance and mentoring
- **With Project Manager:** Identify and escalate technical risks and dependencies
- **With Product Manager:** Discuss technical trade-offs and feasibility
- **With Security/Compliance Officer:** Integrate security design patterns

### Referenced in Process Documents
- [Project Planning](octoacme-project-planning.md#risk--dependency-management) — Risk identification
- [Execution & Tracking](octoacme-execution-and-tracking.md#quality--testing) — Quality standards

---

## Stakeholder/Sponsor

### Role Summary
Sponsors and key stakeholders provide business context, approve high-level decisions, and champion the project. They remove organizational blockers and ensure alignment with business goals.

### Responsibilities
- Define business objectives and success criteria
- Approve go/no-go decisions at project gates
- Remove organizational blockers and secure resources
- Provide feedback on progress and priorities
- Communicate project status to broader organization
- Champion the project within their sphere of influence
- Participate in critical decision forums and risk escalations

### Goals
- Ensure project delivers business value
- Maintain stakeholder alignment and support
- Remove barriers to project success
- Enable rapid decision-making

### Typical Communication
- Project kickoff and gate reviews
- Monthly or milestone-based status updates
- Decision forums and escalations
- Post-project retrospectives
- Ad-hoc check-ins on critical issues

### Interaction with Other Roles
- **With Project Manager:** Receive status updates and approve escalations
- **With Product Manager:** Review business outcomes and ROI
- **With All Teams:** Provide strategic direction and remove blockers

### Referenced in Process Documents
- [Project Initiation](octoacme-project-initiation.md#minimum-deliverables) — Stakeholder identification and alignment
- [Risk Management & Communication](octoacme-risks-and-communication.md#escalation-paths) — Escalation authority
- [Release & Deployment](octoacme-release-and-deployment.md#deployment-checklist) — Stakeholder announcements

---

## Release Manager

### Role Summary
Release Managers orchestrate the release process, coordinate deployment activities, and ensure smooth transitions to production with minimal risk.

### Responsibilities
- Plan and schedule release windows
- Coordinate pre-release validation (smoke tests, security scans, etc.)
- Manage deployment procedures and runbooks
- Verify post-deploy health and monitor early incidents
- Coordinate rollback if needed
- Document release notes and communicate to stakeholders
- Track deployment metrics and postmortem insights

### Goals
- Minimize release risk and time-to-production
- Ensure smooth deployments with rapid incident response
- Maintain visibility into release status
- Build confidence in release process through clear communication

### Typical Communication
- Release planning meetings
- Deployment runbooks and checklists
- Pre-release and post-deploy status reports
- Incident response coordination
- Communication to support, marketing, and customers

### Interaction with Other Roles
- **With Project Manager:** Coordinate release timeline and gate approvals
- **With QA/Testing Lead:** Validate smoke tests and release readiness
- **With Developers:** Coordinate hotfixes and rollback procedures
- **With Stakeholders:** Communicate release status and impact

### Referenced in Process Documents
- [Release & Deployment Guide](octoacme-release-and-deployment.md) — Complete release orchestration
- [Execution & Tracking](octoacme-execution-and-tracking.md#blocker-escalation) — Escalation for release blockers

---

## Security/Compliance Officer

### Role Summary
Security and Compliance roles ensure projects meet security standards, privacy requirements, and regulatory obligations. They identify and help mitigate security risks.

### Responsibilities
- Review designs and code for security vulnerabilities
- Ensure compliance with privacy and regulatory requirements
- Conduct or coordinate security assessments and audits
- Maintain a security incident runbook and coordinate response
- Advise on secure coding practices and security tooling
- Participate in risk assessments and threat modeling
- Provide security training and guidance to the team

### Goals
- Reduce security and compliance risk
- Build security culture within the team
- Ensure customer trust and legal compliance
- Enable secure-by-design practices

### Typical Communication
- Design and code reviews
- Security risk assessments during planning
- Incident response coordination
- Compliance and audit activities
- Security policy and tooling updates

### Interaction with Other Roles
- **With Technical Lead/Architect:** Integrate security into architectural decisions
- **With Developers:** Provide security guidance and code review feedback
- **With Project Manager:** Report security risks and escalate incidents
- **With Release Manager:** Verify security gates before production deployment

### Referenced in Process Documents
- [Risk Management & Communication](octoacme-risks-and-communication.md#escalation-paths) — Security incident escalation
- [Execution & Tracking](octoacme-execution-and-tracking.md#quality--testing) — Security scanning in CI
- [Release & Deployment](octoacme-release-and-deployment.md#pre-release-requirements) — Security scans pre-release

---

## Role Accountability Matrix

This matrix shows primary ownership (●) and participation (○) for key project activities:

| Activity | PM | PdM | Dev | QA | Tech Lead | Release | Security | Sponsor |
|----------|----|----|-----|----|-----------|---------|---------|---------|
| Project Kickoff | ● | ● | ○ | ○ | ○ | | | ● |
| Planning & Estimation | ● | ● | ● | ○ | ○ | | | ○ |
| Design Reviews | ○ | ○ | ● | ○ | ● | | ○ | |
| Security Assessment | ○ | ○ | ○ | ○ | ○ | | ● | ○ |
| Test Plan & Execution | ○ | ○ | ○ | ● | ○ | | | |
| Code Review | ○ | | ● | ○ | ● | | ○ | |
| Release Planning | ● | ● | ○ | ○ | | ● | ○ | ○ |
| Pre-Deploy Validation | ○ | | ○ | ● | ○ | ● | ● | |
| Deployment | | | ○ | | | ● | ○ | |
| Post-Deploy Verification | ○ | | ○ | ○ | ○ | ● | ○ | |
| Incident Response | ○ | | ○ | ○ | ● | ● | ● | ○ |
| Retrospective | ● | ○ | ● | ● | ○ | ○ | ○ | |

**Legend:**
- ● = Primary Ownership (accountable, makes decisions)
- ○ = Participation (contributes, provides input)

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Refer to the Accountability Matrix when planning project activities to ensure the right people are involved.
