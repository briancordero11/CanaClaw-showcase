# Can.AI: Business Model and Enterprise Token Fit

Can.AI, formerly CanaClaw, is proposed as a licensed agent session manager installed on premises. The journey begins with Codex/Claude plugin and access setup, followed by website seat purchase, portal downloads, an installation package, and starter intake/customization led by a Chief AI Officer or Senior-Level Engineer.

The commercial proposition is to turn AI access the enterprise already pays for into useful, supervised work on its own computers. Can.AI sells deployment, starter customization, session management, workflow controls, and support. A proposed data lake and data-storage layer supplies approved context for tool optimization, while iMessage is the primary intended channel for decision requests. Model access remains a separate customer relationship with the provider.

This document describes a proposed business model and validation plan. Packages, prices, capabilities, and outcomes below are design hypotheses unless explicitly identified as sourced provider behavior.

## 1. The purchase-to-value journey

| Stage | Customer action | Proposed Can.AI contribution |
| --- | --- | --- |
| Codex/Claude plugin and access setup | Authorized users establish eligible provider access and the supported plugin/runtime connection. | Explain prerequisites and verify the connection path before seat purchase; this step does not assume a universal login or unverified plugin compatibility. |
| Website purchase | An organization buys named-user seats and identifies its Chief AI Officer or Senior-Level Engineer as setup owner. | Create the organization, seat entitlements, billing record, and customer-portal access. |
| Portal downloads | The setup owner obtains the installation package and deployment instructions. | Present the package, host requirements, entitlement, and release information in one place. |
| Installation package | IT installs the downloaded package on an approved on-premises computer. | Check installation prerequisites, selected provider access, connectivity, and recovery behavior. |
| Starter intake/customization | The Chief AI Officer or Senior-Level Engineer defines the exact agent setup through the starter experience. | Configure PowerTools, approved data-lake sources and storage, tool scope, schedules, budgets, routing, and approval rules. |
| Operate | Employees start or continue sessions, request edits, inspect suggestions, and delegate configured work. | Use authorized context from the data layer to support tools while showing progress, proposed changes, exceptions, and results. |
| High-degree decision making | The designated human decision owner reviews a scoped request delivered primarily through iMessage. | Use OpenClaw to coordinate delivery and return the decision to the correct session; effective user and tool permissions still govern execution. |
| Expand | The sponsor evaluates accepted work, operating costs, and support effort. | Help reuse proven configurations across additional seats, workflows, or on-premises hosts. |

OpenClaw supplies the proposed routing and decision-coordination layer around connected runtimes, with iMessage as the primary intended decision channel. In this product description, “DTC” is the product brief's shorthand for the messaging and decision-routing role, not the name of a standardized protocol. “High-degree decision making” describes the business function and intended outcome; it is not a login, role identity, or permission grant. The customer assigns the actual human decision owner and scope.

Can.AI supplies the starter experience and operating configuration. Cognition, Emergences Labs, and Rowboat Labs are candidate agent/platform integration targets to evaluate through the local session manager. Their inclusion records product direction, not verified compatibility, existing connectors, available APIs, or interchangeable local runtimes. Every selected integration and the iMessage path require runtime, authentication, platform, and permission validation before being promised to a customer. See the [architecture](ARCHITECTURE.md) for the iMessage bridge prerequisite and data placement.

## 2. Who would buy it

The initial target is an enterprise department with repetitive computer-based work, existing AI access, an identifiable technical owner, and a reason to coordinate sessions or tools beyond a single assistant interface.

| Role | Buying interest |
| --- | --- |
| Department sponsor | More accepted work per employee, faster turnaround, and fewer repetitive handoffs. |
| Chief AI Officer or Senior-Level Engineer | Repeatable starter customization, session visibility, reliable recovery, and controlled access to data and tools. |
| IT and security | Clear host ownership, identity boundaries, update management, and understandable data flows. |
| Procurement or finance | Predictable software licensing and visibility into the separate provider bill. |
| Employee | Useful editing and automation suggestions with a clear way to inspect, stop, or resume work. |
| Designated decision owner | Scoped iMessage decision requests, the supporting context, and a record of the resulting business decision. |

Candidate workflows include document revisions, spreadsheet preparation, recurring reporting, engineering support, and Pega delivery work. Pega is one possible workflow pack rather than the definition of the platform.

Poor fits include teams already satisfied by one provider's native tools, organizations without someone to operate the on-premises host, and workloads that require fully disconnected inference while relying on cloud models. A computer installed on premises does not imply that model requests remain on premises; the selected provider connection determines where inference occurs.

## 3. Proposed revenue model

| Revenue component | Proposed charging basis | What it pays for |
| --- | --- | --- |
| Core software | Recurring named-user seat subscription, with an organization minimum if needed. | Session manager, starter configuration, workflow execution controls, updates, and standard support. |
| Deployment service | One-time scoped onboarding fee. | Host setup, provider connection checks, PowerTools customization, approved data-source setup, and acceptance testing. |
| Enterprise operations | Contracted platform or deployment fee tied to a clearly defined scope. | Host management, data-storage operations, iMessage routing support, organizational controls, and support response commitments. |
| Workflow services | Optional fixed-scope implementation engagement. | Building and validating a department-specific workflow pack. |

Define a seat as an authorized human user, not an unlimited number of concurrent agents. Host counts, simultaneous runs, storage and retrieval allowances, decision-channel support, service identities, and unattended usage should be explicit in the contract. Avoid charging twice for the same entitlement through overlapping seat and host fees. A proposed data-lake service must state which storage, indexing, retrieval, and transfer costs are included and which remain customer costs.

Start with a limited paid pilot and a measurable acceptance criterion. Expand only when the customer can reproduce useful work and operate the configuration at an acceptable cost. No public list price or proven willingness to pay is asserted here.

## 4. Separate the Can.AI bill from the model bill

### Provider access and commercial boundaries

An existing AI subscription is a prerequisite only when its supported runtime and permitted authentication method cover the intended use. A subscription is not a universal API credential, a shared enterprise token pool, or permission to bypass provider limits.

OpenAI documents ChatGPT sign-in for subscription access and API-key sign-in for usage-based access, and recommends API keys as the default for automation. The applicable workspace and data controls depend on that route. Can.AI should preserve that distinction during onboarding and validate unattended workflows separately. [OpenAI authentication documentation](https://learn.chatgpt.com/docs/auth)

OpenAI also distinguishes API token pricing from subscription usage. Included subscription tasks should not be estimated by multiplying API token rates. The starter configuration and usage view should label the active billing mode instead of presenting one misleading combined token balance. [OpenAI pricing documentation](https://learn.chatgpt.com/docs/pricing)

For Claude Code distribution, Anthropic currently requires its binary to remain unmodified and its built-in authentication methods to remain available. Each end user authenticates with their own eligible credentials, with usage billed under their own provider agreement; the documented terms prohibit paying for, reselling, or intermediating that usage on the end user's behalf. This supports a proposed software-management fee separate from provider usage, subject to those conditions. [Claude Code legal and compliance documentation](https://code.claude.com/docs/en/legal-and-compliance)

Operationally, the proposed model is:

- The customer pays Can.AI for seats and contracted services.
- The customer maintains the required provider subscriptions or approved API arrangements.
- Can.AI uses supported integration paths and preserves user and enterprise identity boundaries.
- Provider quotas, concurrency restrictions, authentication failures, and usage charges remain visible to the operator.
- Credentials are not pooled between unrelated employees to stretch consumer-plan limits.

## 5. What “token market fit” means

Here, token market fit means that the model consumption required for a workflow produces enough accepted enterprise value to justify its total operating cost. It does not mean a cryptocurrency, a token exchange, or resale of provider capacity.

The useful unit is **cost per accepted workflow**, not tokens generated, agents launched, or messages sent. A workflow counts as accepted only when it meets a customer-defined quality standard after review.

For API-backed execution:

```text
Model cost = sum across every attempted run of:
  (uncached input tokens / 1,000,000) x input rate per million
  + (cached input tokens / 1,000,000) x cached-input rate per million
  + (output tokens / 1,000,000) x output rate per million
  + separately billed tools or services
```

The equation uses dollars per million tokens. Convert any differently quoted rates before calculating. Count retries, failed runs, and fallback-model attempts. Do not count the same input tokens in both cached and uncached categories. Record measured usage where available and label estimates when the provider does not expose complete usage.

For subscription-backed execution, model cost follows the purchased plan, credits or overages, and actual provider rules. Track capacity limits, throttling, wait time, and any incremental paid usage; do not invent a cash token rate for included subscription capacity.

For either route:

```text
Cost per accepted workflow =
  (allocated Can.AI fees
   + attributable provider costs
   + rollout and starter-customization cost amortization
   + host and operating costs
   + data storage, indexing, retrieval, and transfer costs
   + iMessage routing and decision-channel operating costs
   + review, correction, and exception-handling labor)
  / number of accepted workflows
```

All attempted runs belong in the numerator, including attempts that never become accepted work. A provider subscription already purchased for the comparison baseline may have zero incremental cash cost, but it still has capacity constraints and belongs in a full ownership-cost view. A newly required subscription is an additional cost. Show both incremental and fully allocated economics when they tell different stories.

### Token-efficient operation

The proposed starter customization should let the setup owner test a smaller or faster model on bounded tasks and escalate difficult work only when the quality test requires it. Reuse approved PowerTools templates and retrieve relevant context from the authorized data lake and storage layer for tool optimization. Measure retrieval relevance, freshness, and cost instead of assuming that storing more data improves results. Apply caching only where the provider supports it and measured economics justify it. These are optimization hypotheses to validate, not promised savings.

Keep parallel sessions purposeful: duplicate agents, long idle loops, and unbounded retries can consume budget without increasing accepted output. Configure concurrency, retry, time, and context limits, along with spend alerts and pause thresholds where usage reporting permits enforcement. Surface reporting delays and estimates rather than promise an exact provider-billing ceiling from incomplete telemetry.

## 6. Illustrative break-even calculation

The following numbers are invented modeling assumptions, not Can.AI prices, provider price quotes, customer results, or a forecast. The example isolates incremental economics for one month and assumes existing on-premises hardware has no incremental cost. It also assumes no incremental data-storage, retrieval, transfer, or iMessage operating charges; a real deployment must include any such costs before using this result.

| Assumption | Illustrative value |
| --- | ---: |
| Can.AI seats | 20 |
| Assumed monthly software charge per seat | $50 |
| Monthly software total | $1,000 |
| Amortized starter customization and additional operations | $400/month |
| Manual work per accepted workflow | 30 minutes |
| Human review and correction with Can.AI | 10 minutes |
| Loaded labor cost | $60/hour |
| Accepted workflows in the month | 120 |
| Average API input across all attempts per accepted workflow | 100,000 tokens |
| Average API output across all attempts per accepted workflow | 20,000 tokens |
| Assumed input and output rates | $4 and $10 per million tokens |

At those invented rates, model cost is $0.60 per accepted workflow: $0.40 of input plus $0.20 of output. The token averages include failed attempts and retries; any separately billed tools or extra subscription charges would need to be added.

```text
Manual baseline = 120 x 0.5 hours x $60 = $3,600
Assisted labor = 120 x (10/60) hours x $60 = $1,200
Model cost = 120 x $0.60 = $72
Software and amortized setup = $1,000 + $400 = $1,400
Total assisted cost = $1,200 + $72 + $1,400 = $2,672
Illustrative monthly difference = $3,600 - $2,672 = $928
```

The variable saving is $30 minus $10 of human work minus $0.60 of model use, or $19.40 per accepted workflow. Covering $1,400 of fixed monthly cost therefore requires 73 accepted workflows when rounded up. The conclusion changes with actual acceptance rates, review time, provider charges, hardware costs, and operating effort. Time released is capacity value; it is not automatically a realized payroll saving.

## 7. Prove the incremental value

The relevant comparison is the customer's current work process **and** its existing provider-native assistant. Can.AI must earn its additional software and operating cost through deployment consistency, reusable starter customization, cross-session coordination, effective data retrieval, and decision routing. High-degree decision making should be assessed through the quality and timeliness of accepted decisions, not the number of iMessage notifications delivered.

| Pilot question | Evidence to collect |
| --- | --- |
| Does setup reach useful work quickly? | Time from Codex/Claude plugin and access setup through purchase, installation, starter customization, and the first accepted workflow. |
| Is there sustained adoption? | Weekly active licensed users, repeated workflow use, and reasons for abandoned sessions. |
| Does it improve outcomes? | Acceptance rate, correction time, turnaround time, and comparison with the same task performed manually and in the native assistant. |
| Is token use economically useful? | Cost per accepted workflow, retry rate, retrieved-context relevance and cost, model mix, and subscription-capacity interruptions. |
| Does decision routing help? | iMessage delivery reliability, time awaiting a human decision, decision quality, and whether the authorized outcome reaches the correct session. |
| Can the customer operate it? | Setup-owner time per host, PowerTools changes, data maintenance, failed runs, recovery time, and support tickets. |
| Will the buyer renew? | A paid continuation or expansion decision backed by observed value and operating cost. |

Agree pilot targets with the customer before running the comparison. Use equivalent tasks, quality criteria, approved inputs, and human review rules across methods. Report unsuccessful workflows and support effort alongside successful demonstrations.

The core hypothesis is that enterprises will pay for a dependable way to configure and operate agent work on on-premises computers using their existing AI relationships. Product-market fit remains to be demonstrated through repeatable accepted work, sustainable support costs, and paid renewal.

## Source scope

Provider documentation was reviewed on October 22, 2026. The linked sources establish specific authentication, billing, and distribution boundaries; they do not endorse Can.AI or establish compatibility for an implementation that has not been tested.
