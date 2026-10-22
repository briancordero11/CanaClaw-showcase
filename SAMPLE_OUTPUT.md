# Can.AI Example Session and Output

This fictional example accompanies the [Northstar customer journey](CASE_STUDY.md). It illustrates the proposed experience, not output from a released Can.AI product. All identifiers and usage quantities are synthetic.

## Employee request

> Review the approved claims-discovery notes, suggest edits to the requirements workbook, and draft an intake test checklist. Show the changes before applying them.

## Session panel

| Field | Example value |
| --- | --- |
| Organization | Northstar Delivery Services |
| Session | `demo-intake-001` |
| Office host | `office-demo-01` |
| Requester | Assigned delivery analyst |
| PowerTools profile | `Delivery Office v1` |
| Agent role | Editing assistant |
| Provider access | Customer-authorized runtime and billing route |
| Scope | Read approved notes; propose changes in the working-output folder |
| State | Awaiting approval |
| Review needed | Apply the displayed workbook changes |

The user can inspect suggested changes, request revisions, or cancel. Desktop actions are available only through tools explicitly configured and verified on this host.

## Decision request delivered through OpenClaw

**Session:** `demo-intake-001`  
**Decision:** Apply the reviewed workbook edits?  
**Affected artifact:** `working-output/claims-requirements.xlsx`  
**Proposed change:** Add missing-field validation criteria and four unresolved questions.  
**Execution boundary:** This working file only; no production-system update.  
**Reviewer:** Assigned project supervisor.  
**Available decisions:** Approve this change, request revision, or reject.  
**Expiry:** Fifteen minutes in this illustrative profile; expired requests require a fresh decision.

OpenClaw routes the request and response to the correct session. The session manager verifies reviewer identity and action scope before the tool applies an approved change. Sending the request does not itself approve it.

## Deliverable excerpt

### Claims-intake workflow

Suggested stages: capture submission, validate policy details, request missing documents, triage, and confirm intake completion.

### Proposed acceptance criteria

- Evaluate required fields against the selected claim type.
- Show missing items in a reviewable checklist.
- Draft follow-up communication for review before any external send.
- Record the reviewer and approval state with the artifact version.

### Unresolved questions

- Which claim types require supervisor review?
- Which system is authoritative for policy information?
- What retention period applies to incomplete submissions?
- Which channels are approved for follow-up?

## Completion receipt

After approval and successful execution, the receipt lists the changed file, profile version, decision reference, validation outcome, native session reference, and any failed attempts. It can show provider-reported token counts, credits, or usage limits with an explicit `unavailable` value where the provider exposes no suitable measurement. Dollar costs are shown only when a valid billing rate or provider charge is available.

The business outcome is a reviewer-accepted workflow and its resulting edits. Number of messages, sessions, or tokens alone is not a success measure.
