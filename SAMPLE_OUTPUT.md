# Can.AI Example: Executive Reorganization and Budget Decision

This fictional output accompanies the [Northstar case study](CASE_STUDY.md). Northstar Software is modeled at **$100M ARR**, with a **$12M annual delivery-and-operations budget** under review. The 12-seat Can.AI planning pilot supports the decision. All identifiers, budgets, staffing values, and outcomes are invented examples.

## Planning request

> Compare the current structure with a phased reorganization that combines delivery operations and workflow automation. Show budget, transition cost, role changes, customer impact, and the executive decision required.

## Anchor, harnesses, and agent selection

The Chief AI Officer or Senior-Level Engineer defines `Executive Planning v1`. The **agent anchor is Codex or Claude, with minimum required connectors and plugins installed**. PowerTools records each agent's harness, authorized data, requirements, and expected output.

| Agent selection | Harness or working experience | Planned output |
| --- | --- | --- |
| Research and follow-up agent | Dot in its hosted environment, subject to an approved connection | Source changes, open questions, and follow-up evidence |
| Budget-analysis agent | Claude workflow with Claude Artifacts as the reviewable output surface | Scenario model and executive budget artifact |
| Engineering evaluation agent | Cognition developer cowork experience represented by a Devin session | Migration estimate, dependencies, and implementation risks |
| Organization-design reviewer | The approved Codex/Claude anchor harness | Challenge review and decision brief |

These are proposed assignments. Claude Artifacts is the artifact surface in this plan, not an independently certified agent or a claim that it runs locally inside Can.AI. See the [case-study explanation](CASE_STUDY.md#4-agents-within-the-harness-plan).

## Session summary

| Field | Example value |
| --- | --- |
| Organization | Northstar Software |
| Session | `demo-reorg-001` |
| Office computer | `office-demo-01` |
| Requester | Executive planning group |
| Technical setup owner | Chief AI Officer or Senior-Level Engineer |
| Organizational and budget owners | CEO, CFO, and designated people leaders |
| PowerTools profile | `Executive Planning v1` |
| Tool requirements and certifications | Read-only budget and workforce-summary retrieval, scenario calculations, governed document output, and required customer assurance evidence |
| Source collection | Fictional `demo/executive-planning` data-lake collection |
| Output collection | Fictional `demo/reorg-decision` storage collection |
| State | Awaiting executive decision |
| Delivery | iMessage through OpenClaw and a configured Mac Messages bridge |

The tool-evidence register records requirements, applicable certificates or audit reports, scope, validity, and acceptance owner. This example claims no certification has been obtained.

## High-degree decision brief delivered through iMessage

**Decision reference:** `demo-reorg-001 / budget-v1`  
**Company context:** $100M ARR; ARR is a revenue run rate, not spendable cash.  
**Decision requested:** Conditionally approve a phased delivery-and-automation reorg, a $300K one-time transition envelope, and a $300K annual technology-and-operations envelope?  
**Organizational effect:** Combine delivery operations and workflow automation under the Chief AI Officer; redeploy six coordination roles into workflow enablement and customer retention.  
**Staffing assumption:** $1.2M of payroll moves with those six roles and remains within the existing $8.4M payroll budget. No payroll saving or reduction in employment is assumed.  
**Financial case:** $800K gross annual vendor/contractor reduction, less $300K new recurring operating cost, gives $500K net annual run-rate reduction. With three months at the current model, nine at the new model, and $300K transition cost, first-year modeled reduction is $75K.  
**Primary risks:** Delayed contract reductions, disruption to delivery or retention, retraining effort, and insufficient evidence of automation performance.  
**Recommendation:** Conditional approval with a 90-day validation period and explicit finance, executive, and people-team gates.  
**Available decisions:** Retain current structure; conditionally approve phased plan; request a smaller pilot and more evidence.  
**Authority:** CEO/CFO and applicable people leaders approve organizational and spending decisions; the technical setup owner supplies the analysis.  
**Response window:** Two business days in this illustrative profile; a changed budget version or expired request requires renewed review.

The concise message references the governed evidence package. Individual employee information and detailed workforce analysis remain in restricted storage.

## Supporting budget artifact

| Budget item | Current annual | Proposed steady-state annual |
| --- | ---: | ---: |
| Payroll | $8.4M | $8.4M |
| Vendors and duplicated systems | $2.4M | $2.0M |
| Contractors | $1.2M | $0.8M |
| Can.AI, provider usage, storage, and operations | $0 | $0.3M |
| **Recurring total** | **$12.0M** | **$11.5M** |

```text
Gross annual expense reduction = $0.4M + $0.4M = $0.8M
Net recurring reduction        = $0.8M - $0.3M = $0.5M
First-year operating cost      = ($12.0M x 3/12) + ($11.5M x 9/12)
                               = $11.625M
First-year cost incl. transition = $11.625M + $0.300M = $11.925M
First-year reduction            = $12.000M - $11.925M = $0.075M
```

The recurring $300K platform envelope covers multiple suppliers, infrastructure, and operating effort. It is not a Can.AI quote. The separate $300K transition envelope is one-time. If the old model remains for six months rather than three, the first year is $50K more expensive than the unchanged baseline. Results depend on the stated assumptions being realized.

## Proposed implementation gates

- CFO reconciles the model with approved budgets, vendor contract dates, and accounting treatment.
- CEO and people leaders approve the new reporting structure, role transitions, and employee support plan.
- Chief AI Officer or Senior-Level Engineer validates the anchor, selected harnesses and agents, required tool evidence, and representative workflow results.
- The planning group confirms service-level and customer-retention measures before the reorg stage begins.
- Material changes to scope, timing, cost, or staffing return for a fresh decision.

## Completion receipt

The receipt records the source snapshot, anchor and harness identities, agent selection, tool requirements and certification evidence, budget version, decision owners, approvals, conditions, and permitted next step. OpenClaw routes the iMessage decision to the correct session; it does not turn a message into unrestricted authority to update payroll, move employees, or commit funds.

The output is a reviewable executive decision package. Accepted analysis, actual implementation results, and realized financial outcomes are measured separately.
