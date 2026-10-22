# Can.AI Showcase

**Can.AI, formerly CanaClaw, is an enterprise agent session manager designed to run on computers in a customer's office.** The journey starts with an **agent anchor: Codex or Claude, with minimum required connectors and plugins installed**, then Can.AI seat purchase and an installation package. A Chief AI Officer or Senior-Level Engineer leads starter intake, customization, and PowerTools setup for the team's work.

The product combines local editing and automation, a data lake and data storage for tool optimization, and OpenClaw routing through iMessage to support high-degree decision making. Cognition, Emergences Labs, and Rowboat Labs form the proposed platform integration layer. Pega delivery remains one example workflow.

This repository presents the intended customer experience and public product design. Features described here are proposed capabilities, not evidence of a released installer, live checkout, or production deployment. The repository retains its original `CanaClaw-showcase` URL for continuity.

## Customer journey

| Stage | Customer action | Intended Can.AI experience |
| --- | --- | --- |
| Agent anchor setup | Select Codex or Claude and install the minimum required connectors and plugins | Verified identity, permissions, billing route, and connection prerequisites |
| Buy | An organization purchases named-user seats on the website | An organization workspace, seat assignments, billing records, and download access |
| Install and intake | Download the installation package and complete starter intake | A working office installation and documented workflows, data sources, and desired outcomes |
| Customize | The Chief AI Officer or Senior-Level Engineer defines the PowerTools setup | Harnesses, role agents, tool requirements and certifications, data access, decision rules, and budgets |
| Agent selection | Choose agents, their harnesses or working experiences, and applicable platform connections | Individually validated assignments and a record of their access and execution boundaries |
| Organize data | Scope the data lake and data storage for tool optimization | Relevant context, reusable artifacts, and evidence for improving tool use |
| Activate | Test and publish the PowerTools profile | A repeatable setup employees can select for their work |
| Work | Employees edit files, request suggestions, and delegate approved workflows | Visible sessions with progress, changes, review points, and results |
| Decide | Receive a decision brief through iMessage via OpenClaw | High-degree decision making with evidence, options, tradeoffs, and a recorded human decision |
| Operate | IT monitors hosts, usage, failures, and seat assignments | Controlled updates, recoverable sessions, and measurable workflow outcomes |

## What Can.AI adds

- An access-setup-to-installation journey with starter intake and customization
- PowerTools profiles owned by a Chief AI Officer or Senior-Level Engineer
- Agent selection that distinguishes the anchor, execution harness, working agent, and artifact output
- A register of tool requirements, required certifications, and acceptance evidence
- A shared management view of separately authorized agent sessions
- A data lake and data storage layer for context retrieval and tool optimization
- Proposed platform connections to Cognition, Emergences Labs, and Rowboat Labs
- OpenClaw and iMessage coordination for high-degree decision making
- Visibility into completion, correction effort, provider consumption, and cost per accepted workflow

Here, **PowerTools** means Can.AI's proposed configuration bundles for agents and automations. **DTC** retains the product brief's shorthand for OpenClaw's messaging and decision-routing role; this showcase does not define a new protocol by that name.

**Agent anchor** is Can.AI's term for the starting Codex or Claude configuration. An **agent harness** manages execution, session context, tools, and permissions; the **agents in a harness** perform assigned roles. The [case study](CASE_STUDY.md#4-agents-within-the-harness-plan) illustrates Dot, Claude workflows with Artifacts, and Cognition's developer cowork experience represented by Devin, while distinguishing hosted execution and artifact output.

The [executive case study](CASE_STUDY.md#6-the-100m-arr-reorganization-and-budget-example) follows a fictional $100M ARR company evaluating a reorg and a $12M operating budget. Its staffing, spending, and transition assumptions are worked examples for review.

## Existing AI access

Customers bring suitable OpenAI or Anthropic access for their selected agent anchor and any separate access required by the selected platforms and harnesses. A Can.AI seat pays for Can.AI's management software; it does not include every third-party platform seat or inference allowance. Subscription sign-in and API credentials remain distinct connection paths. OpenAI documents these authentication routes separately. [OpenAI authentication](https://learn.chatgpt.com/docs/auth)

The named platforms are proposed integration targets, with capabilities and compatibility to be established during customization. See the [architecture](ARCHITECTURE.md#integration-design) for their distinct roles.

## Office execution and data boundaries

The local session manager and permitted computer actions run on the office computer. The data lake and storage may be local or customer-controlled remote services, as selected during intake. Connected AI services receive approved context; iMessage carries scoped decision briefs and responses. These locations are recorded during customization.

iMessage delivery requires a configured Mac Messages bridge, including when the office execution computer uses another operating system. [OpenClaw iMessage setup](https://docs.openclaw.ai/channels/imessage/setup)

## Explore the showcase

- [Architecture and responsibility boundaries](ARCHITECTURE.md)
- [Fictional customer journey and $100M ARR reorg case](CASE_STUDY.md)
- [Example executive budget and decision brief](SAMPLE_OUTPUT.md)
- [Business model and enterprise token fit](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md)
- [Public security design](SECURITY.md)

Independent portfolio work by Brian Cordero. Named products and organizations describe intended integrations or examples and do not imply endorsement. Copyright (c) 2026 Brian Cordero. All rights reserved.
