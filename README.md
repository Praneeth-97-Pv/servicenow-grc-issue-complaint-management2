# ServiceNow GRC - Issue & Complaint Management

This portfolio project demonstrates an end-to-end Issue and Complaint Management process in ServiceNow Governance, Risk, and Compliance (GRC). It focuses on how organizations can capture complaints, compliance findings, control deficiencies, and risk-related issues in a structured, transparent, and auditable manner.

The process starts when a complaint or potential issue is identified and continues through investigation, risk assessment, root cause analysis, remediation, evidence collection, validation, approval, and formal closure. The objective is to ensure that every issue has clear ownership, appropriate risk treatment, documented evidence, and an auditable resolution path.

## Process Flow

Complaint Raised -> Issue Created -> Triage -> Risk Assessment -> Policy/Risk/Control Mapping -> Root Cause Analysis -> Remediation -> Evidence Collection -> Validation -> Approval -> Closure

## Key Activities

- Created and classified GRC issues based on source, category, business impact, and priority
- Performed initial triage to determine issue validity, ownership, impact, and urgency
- Assessed financial, operational, regulatory, security, customer, and reputational impacts
- Linked issues with relevant policies, risks, controls, business processes, and compliance requirements
- Performed Root Cause Analysis using the 5 Whys methodology
- Identified process gaps, control weaknesses, and contributing factors
- Created corrective-action and remediation tasks with owners and target dates
- Monitored remediation progress, dependencies, overdue tasks, and escalations
- Collected supporting evidence such as procedures, system records, approvals, screenshots, and test results
- Performed control validation and retesting to confirm remediation effectiveness
- Defined closure criteria, approval requirements, and final closure documentation
- Designed SLA monitoring, escalation rules, dashboards, and management reporting

## Example Use Case

A complaint is raised regarding delayed removal of access for terminated employees. The issue is assessed as a potential access-control deficiency.

The issue is mapped to:

- Policy: Access Control Policy
- Risk: Unauthorized access due to delayed termination processing
- Control: Terminated-user access must be removed within the approved SLA
- RCA: Process and control design gap between HR and IAM
- Remediation: Automated termination notifications and workflow improvement
- Validation: Sample testing of termination and access-removal timestamps
- Final Status: Closed after successful validation and approval

## ServiceNow GRC Modules

- GRC: Policy and Compliance
- GRC: Risk Management
- GRC: Audit Management
- Advanced Risk - Issues

## Skills Demonstrated

ServiceNow GRC | Issue Management | Complaint Management | Risk Management | Control Management | Policy & Compliance | RCA | Remediation | Control Testing | Evidence Management | Audit Readiness | GRC Reporting | Compliance Management

## Project Documentation

This project covers the complete issue lifecycle, from intake through validated closure:

1. Complaint or observation is raised and an issue is created.
2. The issue is triaged, and its validity, risk, and impact are assessed.
3. The issue is mapped to relevant policies, risks, and controls.
4. The root cause is investigated and corrective actions are assigned.
5. Remediation evidence is collected and independently validated.
6. Closure is approved and recorded in the audit trail.

### Scope and Success Criteria

The process includes issue creation, triage, risk assessment, governance-object mapping, root cause analysis, remediation, evidence collection, validation, closure, and reporting.

- Every issue has an owner.
- High-risk issues receive risk-owner review.
- Remediation has an owner and due date.
- Evidence is required before remediation is completed.
- Closure requires successful validation.
- The full lifecycle is recorded in an audit trail.

### Exception Paths

- **Invalid issue:** `New → Rejected → Closed`
- **Failed validation:** `Pending Validation → Failed → Remediation In Progress`
- **Overdue remediation:** `Remediation In Progress → Overdue → Escalation`

### Root Cause and Remediation Example

For delayed removal of terminated-user access, a 5 Whys analysis identifies a process and control design gap: application onboarding did not require IAM integration or access-lifecycle controls.

Corrective and preventive actions include:

- Make IAM integration a mandatory onboarding requirement.
- Integrate HR termination events with IAM.
- Perform a one-time access recertification.
- Update the onboarding procedure and checklist.
- Add an approval gate and test the revised control.

Supporting evidence may include the updated procedure, IAM configuration, test records, access-removal logs, approvals, and the recertification report.

### Control Validation

To validate that terminated-user access is removed within the approved SLA:

1. Obtain the population of terminated users and select a sample.
2. Compare termination timestamps with access-removal timestamps.
3. Record exceptions and conclude whether the control passed or failed.
4. Confirm remediation is implemented, evidence is authentic and relevant, and the control operates as intended before closure.

The detailed documentation is available here:

- [Complete project blueprint](docs/ServiceNow_GRC_Issue_Complaint_Management_Project.md)
- [Project overview](docs/01-project-overview.md)
- [Process flow and RACI](docs/02-process-flow.md)
- [Root cause analysis and remediation](docs/03-rca-and-remediation.md)
- [Control validation](docs/04-control-validation.md)
