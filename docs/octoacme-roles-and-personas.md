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

---

## Release Manager

### Role Summary
The Release Manager oversees the end-to-end release pipeline, ensures all release readiness criteria are met, and coordinates deployments and rollback plans across teams.

### Responsibilities
- Maintain the release calendar and communicate deployment windows
- Verify all pre-release criteria (CI passing, security scans, release notes, rollback plan)
- Coordinate staging deployments, smoke tests, and production rollouts
- Lead rollback or incident response if a deployment fails
- Publish release notes and announce releases to stakeholders and support

### Goals
- Achieve predictable, low-risk releases with minimal downtime
- Reduce release cycle time through automation and clear processes
- Ensure all teams are aligned and prepared before each release

### Typical Communication
- Release readiness meetings with PM, DevOps, and QA before each release
- Post-deploy announcements to stakeholders and support channels
- Incident updates and rollback decisions documented in the release log

### Interaction Patterns
- **With PM:** Aligns release scope, timeline, and go/no-go decisions
- **With QA / Quality Advocate:** Confirms all acceptance criteria and smoke tests are completed
- **With DevOps Engineer:** Coordinates pipeline configuration and deployment automation
- **With Stakeholder Champion:** Provides release summaries and communicates impact to stakeholders

---

## Quality Advocate

### Role Summary
The Quality Advocate champions test coverage, acceptance criteria, and defect prevention across the project. They lead test strategy and coordinate with development and QA teams to embed quality throughout the lifecycle.

### Responsibilities
- Define and maintain the overall test strategy (unit, integration, e2e, exploratory)
- Review acceptance criteria for testability before sprint starts
- Monitor test coverage metrics and raise gaps to the team
- Facilitate defect triage and drive root-cause analysis
- Promote quality practices (Definition of Done, code review standards, CI gates)

### Goals
- Minimize escaped defects and regressions in production
- Ensure acceptance criteria are clear, measurable, and verified before release
- Foster a culture where quality is everyone's responsibility

### Typical Communication
- Sprint planning input on acceptance criteria and testing approach
- Weekly quality metrics report shared with PM and developers
- Defect triage meetings with developers when critical issues arise

### Interaction Patterns
- **With Developers:** Reviews acceptance criteria, guides unit/integration test approach
- **With Release Manager:** Confirms test completion and sign-off before release
- **With PM:** Reports on quality metrics, raises concerns about scope or DoD gaps

---

## Security Lead

### Role Summary
The Security Lead is responsible for security reviews, risk assessments, compliance checks, and incident response. They ensure security is integrated into the development lifecycle and liaise with external security teams when needed.

### Responsibilities
- Conduct threat modeling and security reviews for new features and changes
- Maintain the security risk register and remediation backlog
- Ensure CI security scanning is configured and findings are triaged promptly
- Lead or coordinate incident response for security events
- Track compliance requirements (e.g., GDPR, SOC2) and validate controls

### Goals
- Prevent security vulnerabilities from reaching production
- Embed security practices (shift-left) into planning and development workflows
- Minimize mean time to detect and respond to security incidents

### Typical Communication
- Security review sessions with developers during design phase
- Regular updates to PM and stakeholders on security posture and open risks
- Incident communication following the established incident runbook

### Interaction Patterns
- **With PM:** Reports security risks and compliance gaps; participates in risk register reviews
- **With Developers:** Advises on secure coding practices, reviews PRs with security implications
- **With Stakeholders:** Communicates compliance status and significant security decisions

---

## DevOps Engineer

### Role Summary
The DevOps Engineer maintains CI/CD pipelines, automation tooling, and deployment infrastructure to ensure environments are reliable, repeatable, and scalable.

### Responsibilities
- Build, maintain, and improve CI/CD pipelines and deployment automation
- Manage environment provisioning, configuration, and secrets management
- Monitor system reliability, performance, and alerting
- Support developers with build failures, flaky tests, and environment issues
- Implement and maintain infrastructure-as-code (IaC) standards

### Goals
- Achieve fast, reliable, and automated deployments with minimal manual steps
- Reduce environment-related incidents and improve system observability
- Enable developers to ship with confidence through robust tooling

### Typical Communication
- CI/CD pipeline status updates and incident notifications to the team
- Documentation of environment setup, runbooks, and deployment procedures
- Participation in release planning sessions with the Release Manager

### Interaction Patterns
- **With Release Manager:** Configures and executes deployments; provides pipeline status
- **With Developers:** Assists with build and environment issues; reviews IaC changes
- **With PM:** Flags infrastructure risks or capacity constraints affecting delivery timelines

---

## Technical Writer

### Role Summary
The Technical Writer creates and maintains process documentation, onboarding guides, help content, and release notes to ensure information is clear, accurate, and accessible for all audiences.

### Responsibilities
- Draft, review, and maintain process docs, runbooks, and onboarding materials
- Collaborate with teams to capture tribal knowledge in written form
- Ensure documentation is versioned, discoverable, and kept up to date
- Write and publish release notes in partnership with the Release Manager
- Identify documentation gaps and prioritize updates with PM

### Goals
- Reduce onboarding time by providing clear, comprehensive documentation
- Ensure every process and decision has a written artifact
- Keep the documentation repository accurate and well-organized

### Typical Communication
- Documentation review cycles with PM, developers, and other roles
- Release note drafts shared with Release Manager and stakeholders before publishing
- Documentation status updates in weekly PM sync

### Interaction Patterns
- **With PM:** Aligns on documentation priorities and sprint planning
- **With Stakeholders:** Translates technical content into stakeholder-friendly language
- **With All Team Members:** Interviews SMEs to capture process knowledge and updates

---

## Stakeholder Champion

### Role Summary
The Stakeholder Champion ensures stakeholder concerns, priorities, and feedback are actively tracked and integrated into project decisions. They serve as the conduit between sponsors, customers, and the delivery team.

### Responsibilities
- Identify and maintain a list of stakeholder groups and their communication needs
- Gather, synthesize, and relay stakeholder feedback to PM and PdM
- Ensure stakeholder expectations are set and managed throughout the project lifecycle
- Facilitate stakeholder reviews, demos, and approval processes
- Track open stakeholder asks and follow up on resolution

### Goals
- Maintain strong stakeholder confidence and engagement throughout the project
- Prevent misalignment between delivery outputs and stakeholder expectations
- Ensure no stakeholder concern is lost or unaddressed

### Typical Communication
- Monthly stakeholder update reports coordinated with PM
- Pre-release stakeholder briefings in partnership with the Release Manager
- Ad-hoc feedback summaries after demos and reviews

### Interaction Patterns
- **With PM:** Provides stakeholder input for prioritization and risk discussions
- **With PdM:** Shares customer and sponsor feedback to inform roadmap decisions
- **With Sponsors:** Regular updates and escalation channel for executive concerns
- **With Support:** Relays customer-facing issues and collects frontline feedback

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

