# Fictional Case Study: Bringing Can.AI into an Enterprise Office

Northstar Delivery Services is a fictional 12-person enterprise implementation team. Its employees already have approved AI access, but each person configures agents differently. The team's Chief AI Officer or Senior-Level Engineer wants a repeatable installation package, starter intake, and customized PowerTools setup, with governed data and a clear path from agent work to high-degree decision making.

All organizations, people, quantities, tasks, and outcomes below are illustrative. This is the proposed Can.AI customer journey, not a completed customer deployment.

## 0. Codex/Claude plugin and access setup

Before purchase and rollout, Northstar prepares the selected Codex/Claude client or plugin connection and confirms that its existing provider access covers the intended work. The setup owner records user identities, organization policy, the billing route, required permissions, and a small connection test.

This access step establishes prerequisites for Can.AI. Separate credentials or contracts may be needed for the platform integrations selected later; an OpenAI or Anthropic subscription does not include access to every platform in the architecture.

## 1. Discover, evaluate, and purchase seats

The operations lead visits Can.AI's website and reviews the product, installation requirements, customization process, and billing split. Northstar chooses 12 named-user Can.AI seats. Its Chief AI Officer or Senior-Level Engineer owns the rollout and decision policy.

Checkout creates an organization workspace and entitlement. The customer receives a seat-assignment screen, invoice, and installer-download instructions. The Can.AI invoice covers session management and the selected support package. Northstar continues to pay its AI provider directly for the applicable seats, credits, or API consumption.

Before proceeding, Northstar checks that each intended connection has the required provider access. Twelve Can.AI seats do not turn one employee's provider subscription into an organization-wide account.

## 2. Installation package and starter intake

IT downloads the installation package from the organization portal and installs it on an approved office computer. Starter intake captures the team's recurring work, applications, data sources, storage locations, expected outputs, and the people responsible for consequential decisions.

The office computer becomes the execution host. It must remain powered on and connected for its scheduled work to run. A powered-off machine is shown as unavailable; work waits for it instead of silently moving to an unapproved cloud machine. Initial activation, license renewal, update checks, and hosted model calls have their own disclosed network requirements.

The commercial portal manages seats and package access. Intake determines which working state stays on the office computer and which collections belong in the customer's data lake and data storage. Those storage choices are separate from the portal's commercial records.

## 3. Customization with PowerTools setup

The Chief AI Officer or Senior-Level Engineer uses the intake results to create a versioned **PowerTools profile** named `Delivery Office v1`. This customization defines agent roles, tools, prompts, data access, workflow triggers, spending limits, and the decisions that must return to a person.

The installation package, starter intake, and PowerTools setup form one customization journey.

| Configuration | Northstar's illustrative choice |
| --- | --- |
| Agent roles | Intake analyst, editing assistant, test reviewer, and workflow coordinator |
| Data lake and storage | Approved discovery collection, project outputs, retrieval index, and scoped operating evidence |
| Tool access | Explicitly configured document, spreadsheet, repository, and supported desktop tools |
| Integration selection | Evaluate Cognition, Emergences Labs, and Rowboat Labs separately for the tasks they can support |
| Triggers | Employee request, approved file arrival, and scheduled end-of-day review |
| High-degree decision policy | Present evidence and tradeoffs to the Chief AI Officer or Senior-Level Engineer for consequential choices |
| Resource limits | Job concurrency, runtime duration, retry count, context size, and provider spend thresholds |
| OpenClaw and iMessage | Scoped decision briefs and responses through the configured Mac Messages bridge |
| Recovery | Pause, cancel, resume where supported, and escalation after a failed retry |

The setup owner tests the profile with synthetic data, checks generated edits and decision delivery, and publishes it to the 12 assigned users. Later changes are versioned and tested before use.

## 4. Validate integrations and optimize tool context

Cognition, Emergences Labs, and Rowboat Labs are the planned platform layer. Northstar validates each selected connection's available capabilities, credentials, licensing, execution location, and data boundaries. These names are integration targets rather than evidence that Can.AI already supports all three. Their distinct roles are described in the [architecture](ARCHITECTURE.md#integration-design).

The data lake and data storage provide permission-scoped source material, reusable artifacts, and operating evidence. The team retrieves only relevant context for a task and compares tool performance using accepted outputs, corrections, retries, and cost. Optimization uses reviewed evidence; it does not mean automatically training on every stored record.

For unattended work, the setup owner selects an organization-approved automation identity and connection. Shared hardware and shared storage preserve separate user and session access. See the [provider-access and commercial assumptions](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md#provider-access-and-commercial-boundaries).

## 5. Employees use the configured system

An employee opens Can.AI, selects the delivery profile, and starts a session: "Review these discovery notes, suggest improvements to the requirements workbook, and draft a test checklist."

The local session manager shows the requester, office computer, selected integration, profile version, source collection, progress, and pending decisions. The agent retrieves approved material from storage, produces suggested edits, and prepares a reviewable change summary. An employee can accept, revise, or reject suggestions. Configured execution tools apply authorized edits on the office computer and store approved results in the designated collection.

In this example, Pega requirements are one output type. The same management journey could support other engineering or office workflows with separately configured tools and templates.

## 6. iMessage supports high-degree decision making

Northstar uses OpenClaw in the brief's **DTC role**: sending requests, routing them to the appropriate session, delivering progress, and carrying decisions back to that session. The term is product shorthand here, not a claim that DTC is a standard OpenClaw protocol.

The Chief AI Officer or Senior-Level Engineer receives an iMessage decision brief: should the team accept the requirements package, commission a targeted second review, or hold the work until a policy ambiguity is resolved? The brief includes relevant evidence, uncertainty, options, consequences, and a link or reference to the governed decision record.

This is high-degree decision making: selecting the course of action rather than reviewing every small edit. OpenClaw routes the request and scoped response to the correct session. A named person remains accountable, and execution follows the recorded decision and tool permissions.

Northstar configures a customer-approved Mac signed into Messages as the iMessage bridge, using the documented OpenClaw setup. The office session manager can run elsewhere while communicating with that bridge. [OpenClaw iMessage setup](https://docs.openclaw.ai/channels/imessage/setup)

For provider integration, the design uses the appropriate supported route. OpenClaw documents native Codex app-server integration and a separate ACP path for external agent runtimes. ACP does not itself supply a universal account login or unrestricted shared access. [OpenClaw Codex harness](https://docs.openclaw.ai/plugins/codex-harness), [ACP agents](https://docs.openclaw.ai/tools/acp-agents)

## 7. Close, measure, and repeat

After the decision and review, the session stores approved artifacts, the decision record, and a completion summary in governed storage. The setup owner distinguishes completed, failed, cancelled, and awaiting-decision work, then inspects provider usage and retrieval or storage costs where reported. A new employee receives a seat and the tested profile rather than rebuilding the setup.

Northstar evaluates time from plugin/access setup through installation and first accepted work, employee adoption, completion, correction effort, decision turnaround, recovery, and total cost per accepted workflow. No time savings or ROI are claimed until measured.

The business hypothesis is that reusable engineering setup and reliable daily operation create enough value to justify Can.AI's fee in addition to the customer's existing provider spend. See [business model and enterprise token fit](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md) and the [example session report](SAMPLE_OUTPUT.md).
