# Can.AI Example Session and Output

This fictional example accompanies the [Northstar customer journey](CASE_STUDY.md). It illustrates the proposed experience, not output from a released Can.AI product. All identifiers and usage quantities are synthetic.

## Employee request

> Review the approved claims-discovery notes, suggest edits to the requirements workbook, and draft an intake test checklist. Show the changes before applying them.

## Starter intake and customization

The Chief AI Officer or Senior-Level Engineer defines `Delivery Office v1` during installation-package intake and PowerTools setup. Codex/Claude plugin and access prerequisites are recorded first. The planned integration layer includes Cognition, Emergences Labs, and Rowboat Labs, with only validated connections enabled for the pilot.

## Session panel

| Field | Example value |
| --- | --- |
| Organization | Northstar Delivery Services |
| Session | `demo-intake-001` |
| Office host | `office-demo-01` |
| Requester | Assigned delivery analyst |
| Setup and decision owner | Chief AI Officer or Senior-Level Engineer |
| PowerTools profile | `Delivery Office v1` |
| Agent role | Editing assistant |
| Integration route | A validated pilot connection with its customer-authorized identity and billing route |
| Data lake source | Fictional `demo/claims-discovery` collection |
| Data storage output | Fictional `demo/claims-output` collection |
| Optimization evidence | Relevant source references, tool results, corrections, and usage where available |
| Scope | Read the selected collection; propose edits in the designated output location |
| State | Awaiting decision |
| Delivery channel | iMessage through OpenClaw and a configured Mac Messages bridge |

The user can inspect suggested changes, request revisions, or cancel. Desktop actions are available only through tools explicitly configured and verified on this host.

## High-degree decision brief delivered through iMessage

**Session:** `demo-intake-001`  
**Decision:** Accept the requirements package, request a targeted second review, or hold for clarification?  
**Affected artifact:** `demo/claims-output/claims-requirements.xlsx`  
**Evidence:** The draft covers required-field validation; four policy questions remain unresolved.  
**Tradeoff:** Accepting now advances planning; a second review adds cost; holding avoids committing to uncertain policy.  
**Recommendation:** Request a focused review of the unresolved policy questions before treating the package as an approved baseline.  
**Execution boundary:** The chosen review workflow and output collection; no production-system update.  
**Decision owner:** Chief AI Officer or Senior-Level Engineer.  
**Available decisions:** Accept baseline, request second review, or hold.  
**Expiry:** Fifteen minutes in this illustrative profile; expired requests require a fresh decision.

OpenClaw routes the iMessage brief and response to the correct session. The local manager verifies the decision owner's identity and approved scope before continuing the selected workflow. High-degree decision making describes the choice being supported; the named person owns the decision.

## Deliverable excerpt

### Claims-intake workflow

Suggested stages: capture submission, validate policy details, request missing documents, triage, and confirm intake completion.

### Proposed acceptance criteria

- Evaluate required fields against the selected claim type.
- Show missing items in a reviewable checklist.
- Draft follow-up communication for review before any external send.
- Record the decision owner, selected course of action, and approval state with the artifact version.

### Unresolved questions

- Which claim types require supervisor review?
- Which system is authoritative for policy information?
- What retention period applies to incomplete submissions?
- Which decision summaries may be sent through iMessage, and which details must remain in governed storage?

## Completion receipt

After the selected workflow completes, the receipt lists the stored artifact, source collection, profile version, decision owner and reference, validation outcome, session reference where available, and failed attempts. Tool-optimization evidence is retained within its collection permissions and retention rules. The receipt can show reported token counts, credits, retrieval and storage charges, or usage limits, with an explicit `unavailable` value where measurement is missing. Dollar costs require a valid billing rate or provider charge.

The business outcome is accepted work plus an accountable decision and its resulting action. Track decision turnaround and correction effort alongside workflow cost; message, session, and token counts alone do not establish success.
