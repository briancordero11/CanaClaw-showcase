# Sample Output

The following example is fictional and intentionally abbreviated.

## Case type

**Claims Intake**

Purpose: collect, validate, and route a new insurance claim for review.

## Proposed stages

1. Capture submission
2. Validate claimant and policy information
3. Request missing documentation
4. Triage and route
5. Confirm intake completion

## Personas

- Claimant
- Intake specialist
- Claims supervisor
- Assigned adjuster

## Core data objects

- Claim
- Claimant
- Policy
- Incident
- Supporting document
- Triage decision

## Example user story

As an intake specialist, I want incomplete submissions to show missing required fields so that I can request the correct information before routing the claim.

### Acceptance criteria

- Required fields are evaluated against the selected claim type.
- Missing items are shown in a reviewable checklist.
- The system does not send an external request without human approval.
- The approval event is recorded in the audit trail.

## Open questions

- Which claim types require supervisor review?
- What is the authoritative policy system?
- How long may incomplete submissions be retained?
- Which communication channels are approved for follow-up?

## Traceability record

Each artifact should identify its source reference, whether it is explicit or inferred, its reviewer, and its approval state.
