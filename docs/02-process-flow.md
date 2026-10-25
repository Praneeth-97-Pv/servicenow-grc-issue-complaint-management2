# Process Flow

## Lifecycle

1. Complaint/Observation Raised
2. Issue Created
3. Triage
4. Validity Decision
5. Risk & Impact Assessment
6. Policy/Risk/Control Mapping
7. RCA
8. Remediation Plan
9. Evidence Collection
10. Validation
11. Closure Approval
12. Closed

## Exception Paths

### Invalid Issue
`New → Rejected → Closed`

### Failed Validation
`Pending Validation → Failed → Remediation In Progress`

### Overdue
`Remediation In Progress → Overdue → Escalation`

## RACI

| Activity | Reporter | GRC Analyst | Risk Owner | Control Owner | Validator | GRC Manager |
|---|---|---|---|---|---|---|
| Raise issue | R | A | I | I | I | I |
| Triage | I | R/A | I | C | I | I |
| Risk assessment | I | R | A | C | I | I |
| RCA | I | C | C | R/A | I | I |
| Remediation | I | C | C | R/A | I | I |
| Validation | I | C | I | C | R/A | I |
| Closure | I | C | A | C | R | A |
