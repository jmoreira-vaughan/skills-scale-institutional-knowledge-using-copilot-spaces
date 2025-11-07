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

## Business Analyst

### Role Summary
Business Analysts bridge the gap between business needs and technical solutions. They gather requirements, define acceptance criteria, and ensure delivered features align with business objectives.

### Responsibilities
- Elicit and document business requirements from stakeholders
- Define and refine user stories and acceptance criteria
- Analyze data and metrics to inform product decisions
- Facilitate requirement workshops and stakeholder interviews
- Create process flows, data models, and business rules documentation

### Goals
- Ensure technical solutions address actual business needs
- Reduce ambiguity in requirements and acceptance criteria
- Enable data-driven decision making
- Minimize rework from unclear or misunderstood requirements

### Typical Communication
- Requirement workshops with stakeholders and product managers
- Story refinement sessions with developers and QA
- Analysis reports and business case documentation
- Collaboration on acceptance criteria with Product Managers and QA Engineers

### Interaction Points
Business Analysts typically collaborate with:
- **Product Managers**: Align requirements with product vision and roadmap
- **Stakeholders**: Gather business needs and validate solutions
- **Developers**: Clarify requirements and acceptance criteria during implementation
- **QA Engineers**: Define test scenarios based on business rules
- **UX/UI Designers**: Ensure user workflows meet business objectives

**Example Handoff**: BA defines detailed user stories with acceptance criteria → hands off to PM for prioritization → collaborates with Developers during sprint planning to clarify requirements.

---

## UX/UI Designer

### Role Summary
UX/UI Designers create intuitive, accessible, and visually appealing user experiences. They research user needs, design interfaces, and ensure consistency across the product.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, mockups, and interactive prototypes
- Design user flows and information architecture
- Maintain design systems and style guides
- Ensure accessibility standards (WCAG) are met
- Collaborate on frontend implementation

### Goals
- Deliver delightful, intuitive user experiences
- Reduce friction and improve task completion rates
- Ensure consistent visual language and patterns
- Make products accessible to all users

### Typical Communication
- Design reviews and critique sessions
- User research findings and personas
- Figma/Sketch files and design specifications
- Usability test results and recommendations

### Interaction Points
UX/UI Designers typically collaborate with:
- **Product Managers**: Understand user needs and feature requirements
- **Business Analysts**: Align workflows with business processes
- **Developers**: Ensure designs are technically feasible and properly implemented
- **QA Engineers**: Validate UI behavior and accessibility compliance
- **Stakeholders**: Present designs and gather feedback

**Example Handoff**: Designer creates mockups and prototypes → reviews with PM and stakeholders for feedback → provides design specs to Developers → validates implementation with QA.

---

## DevOps / Platform Engineer

### Role Summary
DevOps/Platform Engineers build and maintain the infrastructure, CI/CD pipelines, and tooling that enable teams to develop, test, and deploy software reliably and efficiently.

### Responsibilities
- Design and maintain CI/CD pipelines
- Manage cloud infrastructure and orchestration (Kubernetes, Terraform)
- Implement monitoring, logging, and alerting systems
- Automate deployment and operational processes
- Ensure security and compliance in infrastructure
- Support incident response and troubleshooting

### Goals
- Reduce deployment time and increase deployment frequency
- Improve system reliability and uptime
- Enable developer self-service and autonomy
- Minimize manual operational toil

### Typical Communication
- Runbooks and operational documentation
- Infrastructure-as-code reviews
- Incident retrospectives and post-mortems
- Platform roadmap and capacity planning updates

### Interaction Points
DevOps/Platform Engineers typically collaborate with:
- **Developers**: Provide tooling and pipeline support, troubleshoot build/deploy issues
- **QA Engineers**: Enable test automation infrastructure
- **Support Lead**: Coordinate incident response and provide diagnostic tools
- **Product Managers**: Plan infrastructure for upcoming features
- **Security Teams**: Implement security controls and compliance requirements

**Example Handoff**: DevOps sets up CI/CD pipeline → Developers use it for automated builds/tests → DevOps monitors deployments and alerts → Support Lead uses monitoring tools during incidents.

---

## Support Lead

### Role Summary
Support Leads manage customer support operations, triage incidents, and ensure issues are resolved efficiently. They bridge the gap between customers and engineering teams.

### Responsibilities
- Triage and prioritize customer issues and incidents
- Coordinate incident response and escalation
- Maintain support documentation and knowledge base
- Track and analyze support metrics (resolution time, satisfaction)
- Advocate for customer needs in product planning
- Train support team on new features and tools

### Goals
- Minimize customer downtime and impact
- Improve first-contact resolution rates
- Reduce mean time to resolution (MTTR)
- Enhance customer satisfaction and retention

### Typical Communication
- Incident reports and escalation notices
- Support ticket updates and resolution summaries
- Customer feedback and feature requests
- Support metrics dashboards and trend analysis

### Interaction Points
Support Leads typically collaborate with:
- **Developers**: Escalate bugs and request fixes for customer issues
- **DevOps Engineers**: Coordinate incident response and access diagnostic tools
- **Product Managers**: Provide customer feedback and prioritize bug fixes
- **QA Engineers**: Report production issues and help reproduce bugs
- **Stakeholders**: Communicate customer impact and support trends

**Example Handoff**: Customer reports issue → Support Lead triages and reproduces → escalates to Developers if bug → DevOps assists with diagnostics → Developer fixes and Support validates resolution.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

