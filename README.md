# Can.AI Showcase

**Can.AI, formerly CanaClaw, is an enterprise agent session manager designed to run on computers in a customer's office.** Companies purchase Can.AI seats through a website, install the software on approved office computers, connect their existing licensed AI access, and have a senior engineer configure the agents and automations employees will use.

The product combines local editing and automation with OpenClaw session orchestration, messaging, and decision routing. Pega delivery is one example workflow; the broader product is the operating layer for configured agents across office work.

This repository presents the intended customer experience and public product design. Features described here are proposed capabilities, not evidence of a released installer, live checkout, or production deployment. The repository retains its original `CanaClaw-showcase` URL for continuity.

## Customer journey

| Stage | Customer action | Intended Can.AI experience |
| --- | --- | --- |
| Buy | An organization purchases named-user seats on the website | An organization workspace, seat assignments, billing records, and download access |
| Install | IT downloads the installer and enrolls an approved office computer | A local session manager connected to that organization's entitlement |
| Connect | Authorized users or administrators connect supported OpenAI or Anthropic access | A connection check showing the runtime, account, billing route, and available capabilities |
| Configure | A senior engineer signs in to the admin panel | Versioned agent roles, workspaces, tools, triggers, model routes, approvals, and budgets |
| Activate | The engineer tests and publishes a PowerTools profile | A repeatable automation setup employees can select without reconfiguring the runtime |
| Work | Employees edit files, request suggestions, and delegate approved workflows | Visible sessions with progress, changes, review points, and results |
| Decide | An authorized reviewer receives a decision request through the panel or a configured OpenClaw channel | A decision attached to the correct session, followed by execution within its permissions |
| Operate | IT monitors hosts, usage, failures, and seat assignments | Controlled updates, recoverable sessions, and measurable workflow outcomes |

## What Can.AI adds

- A purchase-to-install path for enterprise teams
- Engineer-defined PowerTools profiles for repeatable work
- A shared management view of separately authorized agent sessions
- Local tools for editing and automation where the installed runtime supports them
- OpenClaw coordination for task delivery, session routing, and approval requests
- Visibility into completion, correction effort, provider consumption, and cost per accepted workflow

Here, **PowerTools** means Can.AI's proposed configuration bundles for agents and automations. **DTC** retains the product brief's shorthand for OpenClaw's messaging and decision-routing role; this showcase does not define a new protocol by that name.

## Existing AI access

Customers bring suitable OpenAI or Anthropic access. A Can.AI seat pays for Can.AI's management software; it does not include a provider seat or inference allowance. Supported subscription sign-in and API credentials are distinct connection paths. The installer must verify the selected runtime's actual authentication, organization policy, usage limits, and permitted integration. OpenAI documents subscription and API-key authentication separately. [OpenAI authentication](https://learn.chatgpt.com/docs/auth)

## Office execution and data boundaries

The agent session manager and permitted computer actions run on the enrolled office host. Hosted models still receive the approved context needed for inference. Messaging channels can also transmit task summaries or results. An on-premises installation therefore does not by itself mean offline inference or that all data stays inside the office. The proposed setup makes those destinations visible to the administrator.

## Explore the showcase

- [Architecture and responsibility boundaries](ARCHITECTURE.md)
- [Fictional customer journey: purchase through daily operation](CASE_STUDY.md)
- [Example session, decision request, and output](SAMPLE_OUTPUT.md)
- [Business model and enterprise token fit](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md)
- [Public security design](SECURITY.md)

Independent portfolio work by Brian Cordero. References to OpenAI, Anthropic, OpenClaw, and Pega describe intended integrations or examples and do not imply endorsement. Copyright (c) 2026 Brian Cordero. All rights reserved.
