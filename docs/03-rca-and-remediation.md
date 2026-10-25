# RCA and Remediation

## 5 Whys Example

### Problem
Terminated-user access is not always removed within the approved SLA.

### Why 1
Termination requests are processed manually.

### Why 2
The application does not receive automated termination events.

### Why 3
The application was not included in the IAM integration scope.

### Why 4
The onboarding process did not mandate IAM integration.

### Why 5
The onboarding control checklist lacked a mandatory access-lifecycle requirement.

### Root Cause
A process/control design gap in application onboarding resulted in incomplete IAM integration.

## Corrective Action

1. Add IAM integration as a mandatory onboarding requirement.
2. Integrate HR termination events with IAM.
3. Perform a one-time access recertification.
4. Update the onboarding SOP.
5. Test the revised control.

## Preventive Action

Use a mandatory checklist and approval gate so future applications cannot enter production without confirming access lifecycle integration.

## Evidence

- Updated SOP
- IAM configuration
- Test records
- Access-removal logs
- Approval evidence
- Recertification report
