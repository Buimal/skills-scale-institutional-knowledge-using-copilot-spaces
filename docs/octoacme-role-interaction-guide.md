# OctoAcme Role Interaction Guide

## Purpose
Provide guidance on how different roles collaborate, communicate, and hand off work throughout the project lifecycle.

## Overview
Successful project execution depends on clear role clarity, timely communication, and smooth handoffs between roles. This guide explains how the personas defined in [OctoAcme Personas](octoacme-roles-and-personas.md) interact across the project lifecycle.

---

## Phase 1: Initiation

### Key Roles
- **Sponsor/Stakeholder** – Sets business vision and approves go-ahead
- **Product Manager** – Refines problem statement and success metrics
- **Project Manager** – Coordinates kickoff and initial planning

### Handoff Sequence

1. **Sponsor → Product Manager**
   - Business objective and constraints
   - Stakeholder list and approval authority
   - Budget and resource constraints

2. **Product Manager → Project Manager**
   - Problem statement and success metrics
   - Prioritized backlog outline
   - Known risks and dependencies

3. **Project Manager → All Teams**
   - Project charter and kickoff meeting schedule
   - Communication cadence and decision process
   - Timeline and milestone framework

### Communication Cadence
- **Kickoff Meeting:** All roles participate; define goals, roles, and schedule
- **Stakeholder Alignment:** PM + PdM + Sponsor; confirm go-ahead

---

## Phase 2: Planning

### Key Roles
- **Product Manager** – Refines backlog and acceptance criteria
- **Project Manager** – Creates plan and manages dependencies
- **Technical Lead** – Assesses technical feasibility
- **QA/Testing Lead** – Defines QA strategy
- **Security Officer** – Identifies security and compliance requirements

### Handoff Sequence

1. **Product Manager → Technical Lead**
   - Feature description and acceptance criteria
   - User personas and use cases
   - Performance and scalability needs

2. **Technical Lead → Developers**
   - Architecture and design approach
   - Technical constraints and assumptions
   - Integration points and dependencies

3. **Product Manager → QA/Testing Lead**
   - Acceptance criteria and Definition of Done
   - Test scenarios and edge cases
   - Quality standards and coverage targets

4. **Security Officer → All Teams**
   - Security requirements and threat assessment
   - Compliance checklist (privacy, regulatory, etc.)
   - Secure design patterns and tooling

5. **Project Manager → All Teams**
   - Sprint/iteration plans with capacity and estimates
   - Risk register with owners and mitigation plans
   - Dependency map and critical path

### Communication Cadence
- **Planning Kickoff:** PM + PdM + Tech Lead + QA Lead; scope and approach
- **Design Review:** Tech Lead + Developers + Security Officer; approve architecture
- **Sprint Planning:** All team members; commit to backlog and capacity

---

## Phase 3: Execution (Build & Test)

### Key Roles
- **Developers** – Implement features
- **QA/Testing Lead** – Execute tests, validate criteria
- **Technical Lead** – Mentor and review code
- **Project Manager** – Track progress and manage risks
- **Security Officer** – Review code and designs for vulnerabilities

### Handoff Sequence

1. **Developers → Code Review (Tech Lead + Security Officer)**
   - Code and supporting tests
   - Design decisions and trade-offs
   - Known issues and limitations

2. **Developers → QA/Testing Lead**
   - Feature ready for testing (meets Definition of Done)
   - Test environment access and data setup
   - Any special testing instructions

3. **QA/Testing Lead → Developers (if defects found)**
   - Defect report with clear reproduction steps
   - Expected vs. actual behavior
   - Proposed fix acceptance criteria

4. **Project Manager → Sponsor (if blockers arise)**
   - Blocker description and impact
   - Proposed mitigation and timeline impact
   - Decision needed / escalation authority

### Communication Cadence
- **Daily Standup:** Quick sync on progress, blockers, and help needed
- **Code Review:** Ongoing, typically 24-48 hour turnaround
- **Sprint Review:** Demo of completed work to Product Manager and Stakeholders
- **Risk Review (Weekly):** PM + Tech Lead; discuss emerging risks

---

## Phase 4: Release Preparation

### Key Roles
- **Release Manager** – Orchestrates release process
- **QA/Testing Lead** – Conducts smoke tests and release verification
- **Security Officer** – Runs security scans and compliance checks
- **Product Manager** – Validates release notes and scope
- **Project Manager** – Coordinates timeline and stakeholder communication

### Handoff Sequence

1. **Project Manager → Release Manager**
   - All accepted features and bug fixes merged
   - Release notes draft
   - Timeline and deployment window

2. **Release Manager → QA/Testing Lead**
   - Staging deployment and environment setup
   - Smoke test checklist and acceptance criteria
   - Timeline for validation

3. **QA/Testing Lead → Release Manager (sign-off)**
   - Smoke test results and pass/fail status
   - Any last-minute concerns or risks
   - Approval to proceed to production

4. **Security Officer → Release Manager (sign-off)**
   - Security scan results
   - Compliance checklist verification
   - Approval for production deployment

5. **Release Manager → All Stakeholders**
   - Release notes and impact summary
   - Deployment schedule and expected downtime
   - Rollback plan (if applicable)

### Communication Cadence
- **Release Planning:** Release Manager + PM + PdM; confirm scope and timeline
- **Pre-Deploy Readiness:** Release Manager + QA + Security; verify gates
- **Deployment:** Release Manager + on-call team; coordinate live deployment
- **Post-Deploy:** Release Manager → Stakeholders; confirm success

---

## Phase 5: Close & Retrospective

### Key Roles
- **Project Manager** – Facilitates retrospective and captures learnings
- **All Teams** – Participate in reflection and feedback
- **Sponsor/Stakeholder** – Attends post-project review

### Handoff Sequence

1. **Project Manager → All Teams**
   - Retrospective agenda and ground rules
   - Guide discussion: what went well, what could improve

2. **All Teams → Project Manager**
   - Action items and improvements
   - Lessons learned and best practices
   - Feedback on process and tools

3. **Project Manager → Sponsor**
   - Project summary and outcomes
   - Retrospective action items
   - Recommendations for future projects

### Communication Cadence
- **Retrospective:** All teams; 45–75 minutes, structured format
- **Action Item Follow-up:** PM tracks progress over 4–6 weeks
- **Post-Project Review:** PM + Sponsor; wrap-up and business impact

---

## Decision Rights & Escalation

### Decision Authority by Role

| Decision | Owner | Consulted | Informed |
|----------|-------|-----------|----------|
| Product priorities & roadmap | Product Manager | Sponsor, Project Manager | Developers, QA |
| Technical approach & architecture | Technical Lead | Product Manager, Security Officer | Developers, QA |
| Acceptance criteria & quality standards | Product Manager & QA/Testing Lead | Developers, Technical Lead | Project Manager |
| Schedule & milestone dates | Project Manager | Sponsor, Product Manager, Technical Lead | All teams |
| Release timing & scope | Project Manager & Product Manager | Sponsor, Release Manager | QA, Security, Developers |
| Security & compliance requirements | Security Officer | Technical Lead, Product Manager | All teams |
| Blocker escalation & unblocking | Project Manager | Sponsor (if needed) | Affected teams |

### Escalation Paths

**Level 1 – Team Resolution (same day)**
- Issue: Technical disagreement, unclear acceptance criteria, resource conflict
- Owner: Project Manager + relevant lead (Tech Lead or QA Lead)
- Action: Facilitate discussion, make recommendation, document decision

**Level 2 – Manager Escalation (1–2 days)**
- Issue: Cross-team dependency delay, scope creep, resource unavailability
- Owner: Project Manager escalates to Product Manager or Sponsor
- Action: Triage impact, trade-offs, and mitigations; make go/no-go call

**Level 3 – Sponsor Escalation (immediate)**
- Issue: Business-impacting delay, security vulnerability, critical blocker
- Owner: Project Manager escalates to Sponsor
- Action: Review business impact, approve workaround or delay, communicate broadly

**Security Incident (immediate)**
- Issue: Suspected vulnerability, data breach, compliance violation
- Owner: Security Officer escalates per security incident runbook
- Action: Follow security playbook; notify on-call and leadership; coordinate response

---

## Communication Best Practices

### Documentation & Transparency
- **Single Source of Truth:** Use the project board and shared docs for status, decisions, and risks
- **Decision Logs:** Record key decisions, rationale, and trade-offs (in README or wiki)
- **Risk Register:** Update weekly; shared with all stakeholders
- **Meeting Notes:** Capture attendees, decisions, action items, and owners

### Synchronous Communication
- **Daily Standup:** 15 min; focus on progress, blockers, help needed
- **Weekly Sync:** PM + PdM + Tech Lead; review risks, dependencies, and progress
- **Bi-weekly Stakeholder Update:** PM reports to Sponsor; progress, risks, decisions needed
- **Ad-hoc Escalations:** Triggered by blockers; target 24-hour response time

### Asynchronous Communication
- **Slack / Email:** For updates that don't require immediate response
- **GitHub Issues & PRs:** For technical feedback and code review
- **Project Board:** Source of truth for status and next steps
- **Weekly Digest:** PM summarizes progress and upcoming milestones

### Feedback & Learning
- **Code Review:** Constructive, timely feedback within 24–48 hours
- **Retrospectives:** Blame-free, focused on improving processes
- **Action Item Follow-up:** Track progress and celebrate improvements

---

## Handoff Checklist Template

Use this template when handing off work between phases or roles:

- [ ] **What?** – Clearly describe what is being handed off
- [ ] **Why?** – Explain the context and business rationale
- [ ] **Dependencies?** – List any upstream or downstream dependencies
- [ ] **Success Criteria?** – Define how to know the handoff succeeded
- [ ] **Timeline?** – When is this due / when should work start?
- [ ] **Questions?** – Identify open questions and clarify before proceeding
- [ ] **Approval?** – Confirm receiver understands and agrees to acceptance criteria

---

## Related Documentation
- [OctoAcme Roles & Personas](octoacme-roles-and-personas.md)
- [Project Initiation](octoacme-project-initiation.md)
- [Project Planning](octoacme-project-planning.md)
- [Execution & Tracking](octoacme-execution-and-tracking.md)
- [Risk Management & Communication](octoacme-risks-and-communication.md)
- [Release & Deployment](octoacme-release-and-deployment.md)
