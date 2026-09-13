# Project Charter

| | |
|---|---|
| **Project Title** | Accessibility Compliance Manager |
| **Sponsor by** | RAMP LLC. |
| **Project Start Date** | September 7th, 2026 |
| **Budget Allocation** | TBD |

## Content table

- [Project Objectives](#Project-Objectives)
- [Main Project Success Criteria](#Main-Project-Success-Criteria)
- [Scope](#Scope)
- [Out-of-Scope](#Out-of-Scope)
- [Milestones](#Milestones)
- [Problem Context](#Problem-Context)
- [Problem Statement](#Problem-Statement)
- [Impact](#Impact)
- [Solution Scope](#Solution-Scope)
- [Assumptions](#Assumptions)
- [Constraints](#Constraints)
- [Still Unknown](#Still-Unknown)
- [Risk and Mitigation Plan](#Risk-and-Mitigation-Plan)
- [Stakeholder Register](#Stakeholder-Register)
- [Team-Agreement](#team-agreement)
- [Repository-&-Workspace-Evidence](#repository--workspace-evidence)


## Project Objectives

1. **Centralize Accessibility Defect Tracking**: Develop a centralized platform to log and manage accessibility defects across digital products.
2. **Automate Compliance Reporting**: Automate reporting by generating standard (VPAT) and custom compliance reports summarizing defects by severity, WCAG success criteria, status, affected area and more, through a standard scoring model based on defect severity, category and WCAG success criteria, enabling stakeholders to track compliance health.
3. **Establish a Custom Accessibility Scoring Methodology**: Design and implement a scoring system to quantify accessibility health based on defect severity, frequency and impact allowing teams to benchmark progress.
4. **Secondary Objectives**
    - Deliver actionable improvement and recommendations
    - Improve visibility and accountability
    - Enable continuous improvement

## Main Project Success Criteria

- **Logging accuracy**: All defects are logged in system with complete metadata (severity, WCAG criterion, affected page/component, date, product)
- **Reporting**: Reports can be generated on demand for all products, reflecting real-time accessibility defect and health status, reducing reporting time by 80% compared to manual spreadsheets approach.
- **Adoption**: At least 60% of relevant teams (QA, Dev, Product, Design) actively use the tool for logging and tracking defects within 9 months of launch.
- **Scoring methodology**: New scoring method is validated, documented, and actively used to measure compliance health across at least 10 teams.
- **Audit**: The tool produces sufficient reports to demonstrate compliance status during internal or external accessibility audits.
- **Reduced recurring defects**: Decrease in recurring defect types over time, indicating that recommendations are driving proactive fixes.

## Scope

- Defect logging module (manual entry + potential integration with scanning/testing)
- Custom scoring engine to calculate accessibility compliance scores
- Automated report generation by product, severity, WCAG criterion, team and more
- Recommendation engine to suggest remediation actions
- Dashboards for real-time visibility into accessibility health and trends
- Integration with existing tools (e.g., Jira, Azure DevOps) for defect assignment and tracking
- Alignment with WCAG 2.1/2.2 standards

## Out-of-Scope

- Automated accessibility defect resolution. (The tool suggests options for logged defects, but neither find nor auto-fix, issues)
- Legal compliance (Tool supports audit-readiness but doesn't replace formal legal review)
- Accessibility testing of non-digital assets (e.g., physical spaces)
- Real-time automated scanning of production environments

## Milestones

- Project Charter and roles and responsibilities approval     - **September 13th, 2026**
- Tech stack approval                                         - **September 18th, 2026**
- Project stakeholder's kick off meeting                      - **September 21st, 2026**
- Environment setup and development kick off                  - **September 24th, 2026**


## Business Context Summary
Organizations today manage multiple digital products or a single product built from multiple components, tools, 
and integrations maintained by different teams. Each product (or team) may serve multiple clients, sometimes with client-specific 
implementations, and each is subject to accessibility requirements such as WCAG, ADA, and Section 508.

Accessibility compliance is not a one-time activity, but is continuously required for internal audits, external audits, 
client requests, RFP responses, leadership reporting, and legal/regulatory obligations. With increasing clients, products,
 teams and tools, the complexity of tracking, testing and reporting on accessibility grows exponentially.

## Problem Statement

Currently, accessibility testing and defect tracking are fragmented across teams using disconnected tools, spreadsheets, or informal processes. Because of this, the organization faces the following recurring issues:

- Accessibility defects and test results are scattered across different teams, tools, and formats.
- Producing a report for a product made up of multiple teams requires manual collecting and compiling of data from each team.
- Teams independently initiate new accessibility tests with no shared visibility into what's already been tested or found resulting in duplicate defects and redundant testing.
- Resolving a defect relies on manual back-and-forth communication between the accessibility tester (defect logger) and developers for recommendations, clarifications, and approvals.
- Reports must be manually compiled and updated per team, consuming significant time and introducing risk of error or inconsistency.
- Leadership and stakeholders cannot easily answer basic questions like: Is our accessibility posture improving or worsening? What is our current compliance status across the organization?
- Audits, RFPs, and client requests are delayed because data must be gathered and compiled reactively rather than being readily available.

## Impact

- Delayed, missed, or rejected RFPs.
- Terminated or at-risk client contracts.
- Increased legal and regulatory risk.
- Wasted time and resources on manual reporting and redundant work.
- Poor organizational visibility.
- Reputational risk with clients and partners.

## Solution Scope

- Log and manage accessibility defects across all digital products, teams, and client implementations in one system.
- Generate on-demand, standardized compliance reports and eliminating manual cross-referencing.
- Apply a custom accessibility scoring methodology to quantify compliance health and trends over time.
- Providing actionable remediation recommendations, reducing reliance on manual back-and-forth communication.
- Dashboards for real-time accessibility status, trends, and ownership visibility.
- Maintain a structured, traceable history of tests, defects, and resolutions for audit requests.


## Assumptions

- Relevant teams are willing to adopt the tool and migrate away from existing processes.
- Accessibility testers/QA teams have (or will be trained on) the knowledge to log defects consistently.
- Existing ticketing tools (e.g., Jira, Azure DevOps) have APIs available for integration.
- Leadership will support standardizing on a single scoring methodology across all teams.
- Current defect records are reasonably clean or can be normalized without excessive manual cleanup for migration.

## Constraints

- Must align with existing recognized accessibility standards (WCAG 2.1/2.2, ADA, Section 508, EN 301 549).
- Must integrate with existing defect/ticketing systems already in use by dev teams.
- No existing industry-standard scoring model is mandated, which limits ability to benchmark against external organizations at launch.
- Tool must support role-based access (testers, developers, leadership, possibly external auditors/clients).
- Data privacy and security requirements may restrict how client-specific data is stored, shared, or exposed in reports.

## Still Unknown
- Exact list of teams/products that will onboard.
- Whether client-facing reporting is in scope.
- Final formula for the custom accessibility scoring model.
- Which specific testing tools will feed data into the system, and whether integration is automated or manual entry.
- Volume of current defect data to migrate, and its quality.

## Risk and Mitigation Plan
| Risk | Description | Preliminary Mitigation Strategy |
|---|---|---|
| **Low team adoption** | Teams may continue using existing informal tracking instead of migrating to the new tool. | Involve team leads early in design/dev phase; provide training; consider starting with willing teams; leadership mandate for adoption in mature phase. |
| **Inconsistent defect logging quality** | If testers log defects with inconsistent/missing detail (missing severity, WCAG mapping, etc.), scoring and reporting accuracy will suffer. | Enforce required fields and validation at data-entry; provide standardized logging templates; periodic data-quality checks. |
| **Scoring methodology lacks credibility** | A custom score not sourced from an industry-recognized standard may be questioned by auditors, clients, or leadership. | Document scoring methodology transparently; back test against past/known compliant and non-compliant data. |
| **Integration failures with existing tools (Jira, ADO, etc.)** | API limitations, permission issues, or data-mapping mismatches could break integrations. | Check key tools for integrations early; identify manual-import options. |
| **Historical data migration issues** | Legacy defect data may be incomplete, inconsistent, or in incompatible formats. | Start data quality audit before migration; define standard metadata requirement for reports and dashboard. |

# Stakeholder Register

|           Stakeholder        | Category                 | Interest in the project | Influence | Decision responsibility |
|------------------------------|--------------------------|-------------------------|-----------|-------------------------|
| Leadership / Project Sponsor | Internal | Wants organization-wide visibility into compliance and a clear return on the investment; needs to answer to clients and regulators | High      | 	Approves budget, scope, and the standardized scoring methodology; can mandate adoption. Final authority on go/no-go                   |
| Accessibility Testers / QA teams | Internal (primary users)|     The people logging defects daily — they care most about whether the tool is faster and clearer than their current spreadsheets                   | Medium     | Own the accuracy and completeness of logged defects; feedback shapes the logging module design |
| Developers / Dev teams | Internal (users)         |  Receive defect assignments and remediation recommendations; care about clean integration with their existing workflow | Medium                    | 	Decide how the tool integrates with their ticketing systems; own defect resolution
| Product Managers / Product teams | Internal (users)         | Need real-time compliance health per product to plan releases and respond to client commitments                        | Medium      | 	Prioritize which defects and products get attention; consumers of dashboards                    |
| Team Leads / Project Sponsor | Internal          |  Key to adoption — their buy-in determines whether their teams actually migrate to the tool                      | Medium-High      | Drive adoption within their teams; early design input                    |
| Clients | External | 	Request accessibility reports for RFPs and contracts; their expectations set the compliance bar. | High | Cannot direct the project, but their demands drive its requirements and urgency | 


# Team Agreement 
This agreement sets out how our team works together on the Accessibility Compliance Manager project. It is meant to be practical and enforceable. 

|   Member  |                    Role                    |                               Responsibility                                |
|-----------|--------------------------------------------|-----------------------------------------------------------------------------|
| Purab     | Business Analyst / QA & Accessibility Lead | Requirements, test cases, defect-logging standards, documentation           |
| Manjinder | Project Lead                               | Runs meetings, tracks milestones, main point of contact with the instructor |
| Raj       | Backend Developer                          | Data model, scoring engine, reporting logic, API integrations.              |
| Jose      | Frontend Developer                         | Dashboards, defect-logging UI, report views.                                |


Meetings:- 
One standing team meeting per week, over Discord voice, lasting up to an hour.
Attendance is expected. If you can't make it, you tell the team in advance and read the notes.

Decision-making:-
We talk about it and agree.
Anything that changes scope, budget, or a milestone is escalated to the Project Lead and confirmed with the sponsor/instructor before we act on it.

Task Ownership:- 
All work is tracked as GitHub Issues on a shared project board.
Every task has one named owner and a due date. "Owned by everyone" means owned by no one, so we avoid it.
The owner is responsible for the task getting done.

Conflict resolution:-
Talk directly and professionally with the person involved first.
If it isn't resolved within 24 hours, bring it to the full team at the next sync (or sooner) and decide together.

Missed work and absences:-
Give as much notice as possible if you'll miss a deadline or a meeting, and propose how your part will be covered.
A missed task is re-assigned or rescheduled by the team so the milestone isn't put at risk.

Professional conduct:-
We treat each other with respect, assume good faith, and keep feedback about the work, not the person.
We meet the commitments we make, and we're honest early when we can't.
We follow academic-integrity rules: the work we submit is our own, sources are cited, and every member understands the work well enough to explain and defend it.
 

# Repository & Workspace Evidence
The project workspace is a private GitHub repository that only team members and the instructor can access. It holds both the codebase and the documentation, so every decision and change is tracked and attributable.

Repository: [link to your private GitHub repo] 
Access: Private; team members added as collaborators with write access; instructor invited as a collaborator/viewer.
