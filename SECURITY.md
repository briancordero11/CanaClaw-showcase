# Can.AI Public Security Design

This repository contains public product-design documentation and fictional examples. The controls below are implementation requirements for the proposed office-installed session manager, not certifications or claims that a production system has already passed validation.

## Identity and access

- Distinguish Can.AI seat ownership, installation-package access, Codex or Claude agent-anchor credentials, platform authentication, and decision authority.
- Treat the agent anchor as the customer's starting environment with minimum required connectors/plugins installed; treat the harness as the session executor that manages execution, effective permissions, and context.
- Keep role agents inside the selected harness within their assigned responsibilities; role names do not create identities, grant tool access, or replace human decision authority.
- Preserve each user's provider and session boundaries on a shared office host.
- Store credentials in an approved credential store; exclude them from exported profiles, messages, and logs.
- Give the Chief AI Officer or Senior-Level Engineer controlled access to starter intake, customization, and PowerTools setup without distributing their provider identity to other users.
- During Agent selection, validate candidate Cognition, Emergences Labs, and Rowboat Labs connections individually, including their data access and execution location.

## Computer actions and decisions

- Define data-lake collections, storage locations, tools, triggers, execution identities, and resource limits in versioned PowerTools profiles.
- Present proposed edits for review where the workflow requires it.
- Keep high-degree decision making accountable to a named person; bind action approvals to that identity, session, scope, and expiry.
- Authenticate and correlate iMessage decisions with the original request; message content alone does not expand tool access.
- Record action completion so retries and reconnects do not blindly repeat external changes.
- Provide visible pause, stop, failure, and host-unavailable states.

## Organization and budget decisions

Automation may gather evidence, model budget allocations, draft organization proposals, and record approvals. Executive organization changes and budget commitments require the designated CEO/CFO authority and applicable HR authorization. An agent, harness, or iMessage reply cannot independently authorize personnel changes, contractual commitments, or spending outside the sender's delegated authority.

Keep the Northstar planning example's redeployed roles separate from cash savings. Preserve the approved assumptions, scope, accountable human owners, and decision record before any downstream system change.

## Tool requirements and certifications

Starter intake and customization include a customer-defined register for required tools and assurance evidence. For each requirement, record the supplier and service, deployment and data scope, required certificate or audit-report type, source document, coverage period or expiry, reviewer, and acceptance status. Link actual evidence and mark missing, expired, or out-of-scope material explicitly.

The register records requirements and review results; it does not assert that Can.AI has obtained certification or that a supplier's certification covers every connected tool, host, or deployment. Agent selection and PowerTools changes trigger a review of affected requirements.

## On-premises and outbound data

The office computer executes permitted local tools and retains configured working state. Data-lake storage, connected AI services, and iMessage have separate locations and access rules. Starter intake and customization identify the destinations, information sent, provider settings, and any portal telemetry. On-premises installation alone does not establish offline operation, data residency, or a compliance certification.

## Data lake and tool optimization

Keep source provenance, collection-level permissions, retention, deletion, and backup rules with the stored data. Scope retrieval to the current task and identity. Use reviewed operating evidence to improve tool selection; do not treat access to a data lake as permission to train models, expose all records, or widen tool privileges.

## iMessage and decision delivery

The proposed setup includes a customer-approved Mac Messages bridge. Keep decision briefs concise, limit recipients, minimize sensitive content, and preserve a fuller decision record in governed storage. A delivery receipt is distinct from approval, and bridge failure must leave a decision pending rather than execute it.

## Operations

The intended deployment process includes verified installation packages, tested PowerTools customizations, controlled updates, session isolation, storage retention, recovery tests, and review of each third-party integration. The Chief AI Officer or Senior-Level Engineer verifies effective permissions across plugins, connected platforms, local tools, storage, and the iMessage bridge.

## Reporting

Use GitHub's private vulnerability-reporting feature if it is enabled. Avoid posting sensitive findings or credentials in public issues.
