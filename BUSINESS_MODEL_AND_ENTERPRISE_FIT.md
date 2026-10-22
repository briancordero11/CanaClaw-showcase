# Can.AI: Business Model and Enterprise Token Fit

Can.AI, formerly CanaClaw, is proposed as a licensed agent session manager installed on computers in a customer's office. Customers purchase seats through a website, download the software, connect their existing eligible AI accounts, and have a senior engineer configure repeatable automation through an admin panel.

The commercial proposition is to turn AI access the enterprise already pays for into useful, supervised work on its own computers. Can.AI sells deployment, configuration, session management, workflow controls, and support. Model access remains a separate customer relationship with the provider.

This document describes a proposed business model and validation plan. Packages, prices, capabilities, and outcomes below are design hypotheses unless explicitly identified as sourced provider behavior.

## 1. The purchase-to-value journey

| Stage | Customer action | Proposed Can.AI contribution |
| --- | --- | --- |
| Evaluate | A department sponsor selects an initial workflow and identifies the senior engineer who will operate it. | Explain provider prerequisites, supported environments, expected permissions, and what the pilot will measure. |
| Purchase | An organization buys named-user seats through the website and appoints an administrator. | Create the organization, seat entitlements, billing record, and installer access. |
| Install | IT downloads and installs the manager on an approved office computer. | Register the host, check runtime prerequisites, and verify connectivity and recovery behavior. |
| Connect | Each user or authorized enterprise identity connects eligible OpenAI, Anthropic, or other supported access. | Guide supported authentication and report connection health without selling pooled provider credentials. |
| Configure | A senior engineer opens the admin panel and defines the exact agent setup. | Provide PowerTools configuration for skills, tools, workspaces, schedules, budgets, routing, and approval rules. |
| Operate | Employees start or continue sessions, request edits, inspect suggestions, and approve delegated work. | Make session state, proposed changes, decisions, exceptions, and results understandable. |
| Expand | The sponsor evaluates accepted work, operating costs, and support effort. | Help reuse proven configurations across additional seats, workflows, or office hosts. |

OpenClaw supplies the proposed routing and decision-coordination layer around connected runtimes. In this product description, “DTC” is the product brief's shorthand for the messaging and decision-routing role, not the name of a standardized protocol. Can.AI supplies the customer experience and operating configuration. Provider integrations must be verified for the selected runtime and authentication route before a customer is promised compatibility.

## 2. Who would buy it

The initial target is an enterprise department with repetitive computer-based work, existing AI access, an identifiable technical owner, and a reason to coordinate sessions or tools beyond a single assistant interface.

| Role | Buying interest |
| --- | --- |
| Department sponsor | More accepted work per employee, faster turnaround, and fewer repetitive handoffs. |
| Senior engineer or automation lead | Repeatable setup, session visibility, reliable recovery, and controlled access to local tools. |
| IT and security | Clear host ownership, identity boundaries, update management, and understandable data flows. |
| Procurement or finance | Predictable software licensing and visibility into the separate provider bill. |
| Employee | Useful editing and automation suggestions with a clear way to inspect, approve, stop, or resume work. |

Candidate workflows include document revisions, spreadsheet preparation, recurring reporting, engineering support, and Pega delivery work. Pega is one possible workflow pack rather than the definition of the platform.

Poor fits include teams already satisfied by one provider's native tools, organizations without someone to operate the office host, and workloads that require fully disconnected inference while relying on cloud models. A computer installed on premises does not imply that model requests remain on premises; the selected provider connection determines where inference occurs.

## 3. Proposed revenue model

| Revenue component | Proposed charging basis | What it pays for |
| --- | --- | --- |
| Core software | Recurring named-user seat subscription, with an organization minimum if needed. | Session manager, admin configuration, workflow execution controls, updates, and standard support. |
| Deployment service | One-time scoped onboarding fee. | Host setup, provider connection checks, initial PowerTools configuration, and acceptance testing. |
| Enterprise operations | Contracted platform or deployment fee tied to a clearly defined scope. | Additional host management, organizational controls, support response commitments, and deployment assistance. |
| Workflow services | Optional fixed-scope implementation engagement. | Building and validating a department-specific workflow pack. |

Define a seat as an authorized human user, not an unlimited number of concurrent agents. Host counts, simultaneous runs, service identities, support coverage, and any unattended usage should be explicit in the contract. Avoid charging twice for the same entitlement through overlapping seat and host fees.

Start with a limited paid pilot and a measurable acceptance criterion. Expand only when the customer can reproduce useful work and operate the configuration at an acceptable cost. No public list price or proven willingness to pay is asserted here.

## 4. Separate the Can.AI bill from the model bill

### Provider access and commercial boundaries

An existing AI subscription is a prerequisite only when its supported runtime and permitted authentication method cover the intended use. A subscription is not a universal API credential, a shared enterprise token pool, or permission to bypass provider limits.

OpenAI documents ChatGPT sign-in for subscription access and API-key sign-in for usage-based access, and recommends API keys as the default for automation. The applicable workspace and data controls depend on that route. Can.AI should preserve that distinction during onboarding and validate unattended workflows separately. [OpenAI authentication documentation](https://learn.chatgpt.com/docs/auth)

OpenAI also distinguishes API token pricing from subscription usage. Included subscription tasks should not be estimated by multiplying API token rates. The admin panel should label the active billing mode instead of presenting one misleading combined token balance. [OpenAI pricing documentation](https://learn.chatgpt.com/docs/pricing)

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
   + rollout and configuration cost amortization
   + host and operating costs
   + review, correction, and exception-handling labor)
  / number of accepted workflows
```

All attempted runs belong in the numerator, including attempts that never become accepted work. A provider subscription already purchased for the comparison baseline may have zero incremental cash cost, but it still has capacity constraints and belongs in a full ownership-cost view. A newly required subscription is an additional cost. Show both incremental and fully allocated economics when they tell different stories.

### Token-efficient operation

The proposed admin setup should let engineers test a smaller or faster model on bounded tasks and escalate difficult work only when the quality test requires it. Reuse approved workflow templates, retrieve relevant context instead of repeatedly sending whole workspaces, and apply caching only where the provider supports it and measured economics justify it. These are optimization hypotheses to validate, not promised savings.

Keep parallel sessions purposeful: duplicate agents, long idle loops, and unbounded retries can consume budget without increasing accepted output. Configure concurrency, retry, time, and context limits, along with spend alerts and pause thresholds where usage reporting permits enforcement. Surface reporting delays and estimates rather than promise an exact provider-billing ceiling from incomplete telemetry.

## 6. Illustrative break-even calculation

The following numbers are invented modeling assumptions, not Can.AI prices, provider price quotes, customer results, or a forecast. The example isolates incremental economics for one month and assumes existing office hardware has no incremental cost.

| Assumption | Illustrative value |
| --- | ---: |
| Can.AI seats | 20 |
| Assumed monthly software charge per seat | $50 |
| Monthly software total | $1,000 |
| Amortized setup and additional administration | $400/month |
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

The relevant comparison is the customer's current work process **and** its existing provider-native assistant. Can.AI must earn the additional software and administration cost through deployment consistency, cross-session coordination, useful workflow configuration, or measurable operating improvements.

| Pilot question | Evidence to collect |
| --- | --- |
| Does setup reach useful work quickly? | Time from seat purchase to a working host, verified provider login, and first accepted workflow. |
| Is there sustained adoption? | Weekly active licensed users, repeated workflow use, and reasons for abandoned sessions. |
| Does it improve outcomes? | Acceptance rate, correction time, turnaround time, and comparison with the same task performed manually and in the native assistant. |
| Is token use economically useful? | Cost per accepted workflow, retry rate, context growth, model mix, and subscription-capacity interruptions. |
| Can the customer operate it? | Engineer time per host, configuration changes, failed runs, recovery time, and support tickets. |
| Will the buyer renew? | A paid continuation or expansion decision backed by observed value and operating cost. |

Agree pilot targets with the customer before running the comparison. Use equivalent tasks, quality criteria, approved inputs, and human review rules across methods. Report unsuccessful workflows and support effort alongside successful demonstrations.

The core hypothesis is that enterprises will pay for a dependable way to configure and operate agent work on office computers using their existing AI relationships. Product-market fit remains to be demonstrated through repeatable accepted work, sustainable support costs, and paid renewal.

## Source scope

Provider documentation was reviewed on October 22, 2026. The linked sources establish specific authentication, billing, and distribution boundaries; they do not endorse Can.AI or establish compatibility for an implementation that has not been tested.
