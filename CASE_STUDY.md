# Fictional Case Study: Bringing Can.AI into an Enterprise Office

Northstar Delivery Services is a fictional 12-person enterprise implementation team. Its employees already have approved AI access, but each person configures agents differently. A senior engineer repeatedly reconnects tools, recovers unfinished work, and explains which automations staff may run. The team wants one managed setup on an office computer, with clear ownership of every session and decision.

All organizations, people, quantities, tasks, and outcomes below are illustrative. This is the proposed Can.AI customer journey, not a completed customer deployment.

## 1. Discover, evaluate, and purchase seats

The operations lead visits Can.AI's website and reviews the product, host requirements, supported provider connections, and billing split. Northstar chooses 12 named-user Can.AI seats and designates one senior engineer as the initial administrator.

Checkout creates an organization workspace and entitlement. The customer receives a seat-assignment screen, invoice, and installer-download instructions. The Can.AI invoice covers session management and the selected support package. Northstar continues to pay its AI provider directly for the applicable seats, credits, or API consumption.

Before proceeding, Northstar checks that each intended connection has the required provider access. Twelve Can.AI seats do not turn one employee's provider subscription into an organization-wide account.

## 2. Download, install, and enroll an office computer

IT downloads the Can.AI installer from the customer portal and installs it on an approved office workstation. The proposed enrollment flow checks the supported operating environment, registers the host to Northstar, and establishes its local workspace and session store.

The office computer becomes the execution host. It must remain powered on and connected for its scheduled work to run. A powered-off machine is shown as unavailable; work waits for it instead of silently moving to an unapproved cloud machine. Initial activation, license renewal, update checks, and hosted model calls have their own disclosed network requirements.

The commercial portal manages seats and entitlements. Working files and local session state live on the configured office host; the published deployment design separately identifies any metadata sent to the portal.

## 3. Connect existing provider access

The setup wizard detects supported installed runtimes and asks an authorized user to complete the relevant provider sign-in or enterprise API configuration. It then verifies a small test session and shows the connected identity, runtime, available model route, billing method, and relevant limits.

For unattended organization workflows, the engineer selects an organization-approved automation credential and access pattern. User sessions retain their own identity boundaries. A shared physical host does not make provider accounts, credentials, or session contents interchangeable.

The setup must select a connection supported by both the runtime and the customer's provider terms; it cannot assume every consumer subscription permits every integration. See the [provider-access and commercial assumptions](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md#provider-access-and-commercial-boundaries).

## 4. Senior engineer configures the admin panel

The engineer signs in to Can.AI's admin panel and creates a versioned **PowerTools profile** named `Delivery Office v1`. PowerTools is the proposed Can.AI setup for agents, tools, and automation rules.

| Configuration | Northstar's illustrative choice |
| --- | --- |
| Agent roles | Intake analyst, editing assistant, test reviewer, and workflow coordinator |
| Workspace scope | Read approved discovery folders; write only to the project's working-output folder |
| Tool access | Explicitly configured document, spreadsheet, repository, and supported desktop tools |
| Provider routes | An approved default agent runtime, plus a separately authorized alternative for selected tasks |
| Triggers | Employee request, approved file arrival, and scheduled end-of-day review |
| Human review | Suggestions may be drafted; sending messages, committing changes, or modifying a business system follows the configured approval rule |
| Resource limits | Job concurrency, runtime duration, retry count, context size, and provider spend thresholds |
| OpenClaw channels | An approved messaging channel connected to named requesters and reviewers |
| Recovery | Pause, cancel, resume where supported, and escalation after a failed retry |

The engineer tests the profile with synthetic files, checks the generated edits and routing, and publishes it to the 12 assigned users. A later profile change is tested and versioned so a running session is not unexpectedly given broader powers.

## 5. Employees use the configured system

An employee opens Can.AI, selects the delivery profile, and starts a session: "Review these discovery notes, suggest improvements to the requirements workbook, and draft a test checklist."

The session manager shows the requester, execution host, provider route, profile version, progress, and pending decisions. The agent reads only the approved materials, produces suggested edits, and prepares a reviewable change summary. An employee can accept, revise, or reject the suggestions. Supported tools can apply authorized edits on the office computer.

In this example, Pega requirements are one output type. The same management journey could support other engineering or office workflows with separately configured tools and templates.

## 6. OpenClaw routes tasks and decision requests

Northstar uses OpenClaw in the brief's **DTC role**: sending requests, routing them to the appropriate session, delivering progress, and carrying decisions back to that session. The term is product shorthand here, not a claim that DTC is a standard OpenClaw protocol.

A supervisor requests a progress report through a configured channel. OpenClaw routes the request to the authorized session on the office host. When the agent proposes an action requiring review, the supervisor receives a concise decision request with its scope, affected files or system, proposed changes, and expiry. Only the authorized reviewer can approve it.

The decision is recorded against that action and session. The execution tool still enforces its own permissions. OpenClaw transports and coordinates the decision; neither a chat message nor a model suggestion independently grants administrative authority.

For provider integration, the design uses the appropriate supported route. OpenClaw documents native Codex app-server integration and a separate ACP path for external agent runtimes. ACP does not itself supply a universal account login or unrestricted shared access. [OpenClaw Codex harness](https://docs.openclaw.ai/plugins/codex-harness), [ACP agents](https://docs.openclaw.ai/tools/acp-agents)

## 7. Close, measure, and repeat

After review, the session produces edited working files, a decision log, and a completion summary. The administrator can distinguish completed, failed, cancelled, and awaiting-review work, then inspect provider usage where reported. A new employee receives a seat and the tested profile rather than rebuilding the automation setup manually.

Northstar evaluates the pilot against the same workflow performed with its existing tools: time to first accepted result, employee adoption, successful completion, reviewer effort, recovery effort, and total cost per accepted workflow. No time savings or ROI are claimed until measured.

The business hypothesis is that reusable engineering setup and reliable daily operation create enough value to justify Can.AI's fee in addition to the customer's existing provider spend. See [business model and enterprise token fit](BUSINESS_MODEL_AND_ENTERPRISE_FIT.md) and the [example session report](SAMPLE_OUTPUT.md).
