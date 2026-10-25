# ServiceNow Configuration Guide

## Issue Fields

| Field | Type | Mandatory | Example |
|---|---|---:|---|
| Number | Auto number | Yes | GRC-ISS-0001 |
| Short description | String | Yes | Delayed access removal |
| Description | HTML/Text | Yes | Detailed issue |
| Source | Choice | Yes | Complaint |
| Category | Choice | Yes | Access Management |
| State | Choice | Yes | New |
| Priority | Choice | Yes | High |
| Risk rating | Choice | Yes | High |
| Risk | Reference | Recommended | Unauthorized Access |
| Control | Reference | Recommended | Access Removal SLA |
| Policy | Reference | Recommended | Access Control Policy |
| Issue owner | Reference | Yes | GRC Analyst |
| Due date | Date | Yes | 2026-09-30 |
| Root cause | HTML/Text | Yes before closure | Process gap |
| Corrective action | HTML/Text | Yes before remediation completion | IAM automation |
| Validation result | Choice | Yes before closure | Pass |
| Closure notes | HTML/Text | Yes before closure | Validated and approved |

## Business Rules

### Close Gate

Prevent closure when:

- RCA is empty
- Corrective Action is empty
- Evidence is missing
- Validation is not Pass
- Closure approval is incomplete

### High-Risk Escalation

For High/Critical risk:

- Notify Risk Owner
- Notify GRC Manager
- Require due date
- Require closure approval

### Overdue Rule

If `Due Date < Today` and `State != Closed`:

- Set overdue flag
- Notify Issue Owner
- Escalate to GRC Manager

## Notifications

Recommended notifications:

- Issue assigned
- High-risk issue created
- Remediation due in 7 days
- Remediation overdue
- Validation failed
- Closure approval requested
- Issue closed
