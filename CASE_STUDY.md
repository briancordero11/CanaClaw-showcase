# Fictional Case Study: Agent Harnesses and a Reorganization at $100M ARR

Northstar Software is a fictional enterprise software company at **$100 million in annual recurring revenue (ARR)**. A 12-person planning group pilots Can.AI to coordinate agent work across finance, delivery operations, and engineering. Its Chief AI Officer or Senior-Level Engineer owns the technical setup; the CEO, CFO, and people leaders own organizational and budget decisions.

The executive question is whether to combine delivery operations and workflow automation under one operating model, redeploy six coordination roles, and fund the required technology. ARR describes the company's revenue scale. It is neither cash available to spend nor a forecast of value created by Can.AI.

All companies, roles, budgets, quantities, and outcomes in this case are fictional design examples.

## 0. Establish the agent anchor

Northstar selects **Codex or Claude as its agent anchor**, with the minimum required connectors and plugins installed. In Can.AI terminology, the anchor is the team's primary authenticated agent entry point and starting configuration.

The starter package records the selected product and version, eligible customer account, identity, billing route, organization policy, and a small connection test. The minimum setup for this pilot includes approved read-only finance and workforce-summary access, governed document storage, a spreadsheet/document output tool, and the configured OpenClaw decision route. Tools are enabled only where the chosen anchor and deployment support them.

The anchor does not automatically grant access to Dot, Claude Artifacts, Devin, or other platforms. Those experiences have their own capabilities, account requirements, and integration boundaries.

## 1. Purchase seats and download the installation package

The operations lead visits Can.AI's website and buys 12 named-user seats for the planning pilot. The organization portal supplies billing records, entitlement, installation-package downloads, and deployment instructions. Provider subscriptions, agent-platform charges, and usage remain separate customer costs.

IT installs Can.AI on an approved office computer. The local session manager coordinates authorized office work; any hosted agent harness or model service retains its own execution location. Local scheduled work requires the office computer to be available.

## 2. Starter intake and customization

The Chief AI Officer or Senior-Level Engineer captures the decision objective, current operating model, team responsibilities, source systems, data classifications, and approval owners. The intake asks what evidence the executives need before changing a reporting line or committing budget.

The data lake and data storage hold approved budget snapshots, aggregate workforce information, vendor commitments, workflow metrics, and draft artifacts. Each collection has a source date, owner, access scope, and retention rule. The planning pilot uses synthetic inputs and does not require unrestricted personnel records.

## 3. PowerTools setup: anchors, harnesses, and agents

The setup owner publishes a versioned PowerTools profile named `Executive Planning v1`.

| Configuration | Northstar's illustrative choice |
| --- | --- |
| Agent anchor | Codex or Claude, with minimum required connectors and plugins installed |
| Agent harnesses | Approved execution environments that manage agent sessions, context, tools, permissions, continuation, and cancellation |
| Agents in harnesses | Research and follow-up agent, budget analyst, engineering evaluator, and organization-design reviewer |
| Agent selection | Choose a role agent, its harness or working experience, and its evidence requirements for each task |
| Tool requirements and certifications | Required finance, workforce-summary, document, spreadsheet, and storage capabilities; applicable customer-required certificates, audit reports, and internal acceptance evidence |
| Data lake and storage | Versioned budget sources, aggregate role data, contract schedules, scenario models, and decision records |
| Triggers | Planning request, approved budget refresh, and scheduled scenario review |
| Decision policy | Chief AI Officer or Senior-Level Engineer prepares the evidence; CEO/CFO and designated people leaders approve the reorg and spending scope |
| Resource limits | Session concurrency, runtime duration, retries, context size, and supplier spending limits |
| OpenClaw and iMessage | Concise executive decision briefs linked to a governed evidence package |
| Recovery | Pause, cancel, supported continuation, and escalation when a required source or certification is missing |

**Tool requirements and certifications** is an evidence register, not a claim that Can.AI or every tool is certified. It records the required scheme or review, issuer, scope, validity, deployment applicability, and approval owner. Missing mandatory evidence prevents that tool from entering the pilot's approved configuration.

## 4. Agents within the harness plan

The case distinguishes the anchor, an agent harness, a working agent, and the artifact it produces. The requested examples fit into the plan as follows:

| Harness or working experience | Agent or output in this case | Intended contribution |
| --- | --- | --- |
| Dot | Ongoing research and follow-up agent in its hosted environment | Track open questions, collect permitted background evidence, and bring back changes that affect the decision |
| Claude workflow and Claude Artifacts | Budget-analysis agent producing a scenario document or interactive budget artifact | Make assumptions, calculations, and alternatives inspectable by the planning group |
| Cognition developer cowork experience, represented by Devin | Engineering evaluation agent in a Devin session | Assess migration effort, integration dependencies, and the feasibility of the proposed automation setup |
| Selected Codex/Claude anchor harness | Organization-design reviewer with a bounded evidence set | Challenge the proposal, identify missing assumptions, and assemble the executive brief |

Dot is documented as a cloud agent that can delegate background work. Claude Artifacts are documents, dashboards, or interactive tools produced in a Claude workflow; an artifact is not automatically an independent autonomous agent. Cognition documents Devin sessions that can coordinate managed Devins. These distinctions inform the proposed design; they do not establish existing Can.AI connectors or imply that all experiences run inside one local process. [Meet dots](https://learn.chatgpt.com/docs/dots), [Claude Artifacts](https://support.claude.com/en/articles/17153992-what-are-artifacts-and-how-do-i-use-them), [Cognition managed Devins](https://cognition.com/blog/devin-can-now-manage-devins)

Cognition, Emergences Labs, and Rowboat Labs remain proposed platform targets. Agent selection evaluates their actual role and supported connection separately. The [architecture](ARCHITECTURE.md#integration-design) explains those boundaries.

## 5. Run the planning workflow

An employee asks: "Compare the current operating model with a phased reorganization of delivery operations and workflow automation. Show recurring budget, transition cost, role changes, customer-service risk, and the approvals needed."

The local session manager assigns bounded work to the selected agents. They retrieve approved source snapshots, draft the budget model, test arithmetic and source consistency, and collect unresolved questions. Tools produce editable planning artifacts and suggested changes. No agent changes the live organization chart, payroll, hiring plan, or purchasing commitments as part of this analysis.

## 6. The $100M ARR reorganization and budget example

Northstar is evaluating a **$12M annual delivery-and-operations budget**, a subset of company spending. The proposal combines delivery operations and workflow automation under the Chief AI Officer and moves six coordination roles into workflow enablement and customer retention.

The six roles represent an illustrative $1.2M of payroll already included below. They remain employed and funded. Their reassignment is a reallocation, not a payroll saving.

| Budget item | Current annual plan | Reorganized annual run rate |
| --- | ---: | ---: |
| Payroll, including the six reassigned roles | $8.4M | $8.4M |
| Vendors and duplicated systems | $2.4M | $2.0M |
| Contractors | $1.2M | $0.8M |
| Can.AI, provider usage, storage, and operating support | $0 | $0.3M |
| **Recurring budget total** | **$12.0M** | **$11.5M** |

The proposed annual reduction in vendor and contractor expenses is $800K. After the $300K recurring technology-and-operations envelope, the net steady-state reduction is **$500K a year**. The $300K envelope includes multiple suppliers and operating costs; it is not a Can.AI price quote.

The plan also requires a separate **$300K one-time transition budget** for migration, training, and organizational change. Assume the first three months retain the current operating model, followed by nine months at the reorganized run rate:

```text
First-year current-model cost = $12.0M x 3/12 = $3.000M
First-year reorganized cost   = $11.5M x 9/12 = $8.625M
One-time transition cost                         $0.300M
First-year total                                 $11.925M
First-year reduction vs. $12.0M baseline          $0.075M ($75K)
```

If the old operating model remains for six months rather than three, first-year recurring savings fall to $250K; after the $300K transition cost, the first year costs $50K more than the baseline. The decision therefore depends on timing, vendor commitments, adoption, delivery capacity, and customer-retention risk. It is not justified by an assumed payroll reduction or a claim that agents created the company's ARR.

## 7. iMessage supports the executive decision

OpenClaw sends the executive a concise iMessage brief with three options: retain the current structure; conditionally approve the phased reorg and its budget envelopes; or run a smaller evidence-gathering pilot before authorizing the reorg. The full model and workforce analysis remain in governed storage.

The proposed recommendation is conditional approval of the phased plan, with a 90-day validation period before the organizational move. The CFO verifies expense assumptions and budget authority; the CEO approves the operating model; designated people leaders approve reporting lines, role transitions, and retraining. The Chief AI Officer or Senior-Level Engineer owns the technical rollout and evidence quality.

An iMessage response is routed to the correct session and recorded with the decision owners, budget version, conditions, and permitted next step. It can authorize preparation of the approved implementation plan. Organizational, personnel, and financial changes still require the responsible owners' normal approval and execution processes.

The configured iMessage path uses a customer-approved Mac Messages bridge. OpenClaw handles request and decision routing in the brief's DTC role. [OpenClaw iMessage setup](https://docs.openclaw.ai/channels/imessage/setup)

## 8. Close, measure, and repeat

The completed planning session stores the scenario model, source references, certification register, agent/harness assignments, executive decision, and outstanding conditions. The planning group measures correction effort, evidence completeness, decision turnaround, source freshness, and total cost of accepted work.

Financial results are evaluated separately after implementation: actual expenses versus the approved baseline, realized vendor reductions, transition spending, customer-service performance, and the experience of reassigned employees. A better decision brief is not itself proof of realized savings.

See the [sample executive brief](SAMPLE_OUTPUT.md) and [business model and enterprise token fit](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md).
