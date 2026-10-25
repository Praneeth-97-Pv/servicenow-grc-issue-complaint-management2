# Control Validation

## Control

Terminated-user access must be removed within the approved SLA.

## Test Objective

Determine whether the control operates effectively.

## Testing Steps

1. Obtain the population of terminated users.
2. Select a sample.
3. Obtain termination timestamps.
4. Obtain access-removal timestamps.
5. Calculate elapsed time.
6. Compare against the approved SLA.
7. Record exceptions.
8. Conclude PASS or FAIL.

## Example

| Sample | Termination | Access Removed | Result |
|---|---|---|---|
| U001 | 09:00 | 10:00 | Pass |
| U002 | 11:00 | 11:30 | Pass |
| U003 | 14:00 | 17:30 | Fail |

If the requirement is 100% compliance, one exception can result in a failed test depending on the organization's testing methodology.

## Validation Evidence

The validator should confirm that:

- Remediation is implemented.
- Evidence is authentic and relevant.
- The control now operates as intended.
- The issue is not merely cosmetically closed.
