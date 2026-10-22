# Can.AI Public Security Design

This repository contains public product-design documentation and fictional examples. The controls below are implementation requirements for the proposed office-installed session manager, not certifications or claims that a production system has already passed validation.

## Identity and access

- Distinguish Can.AI seat ownership, installation-package access, Codex/Claude plugin credentials, platform authentication, and decision authority.
- Preserve each user's provider and session boundaries on a shared office host.
- Store credentials in an approved credential store; exclude them from exported profiles, messages, and logs.
- Give the Chief AI Officer or Senior-Level Engineer controlled access to starter intake, customization, and PowerTools setup without distributing their provider identity to other users.
- Validate Cognition, Emergences Labs, and Rowboat Labs connections individually, including their data access and execution location.

## Computer actions and decisions

- Define data-lake collections, storage locations, tools, triggers, execution identities, and resource limits in versioned PowerTools profiles.
- Present proposed edits for review where the workflow requires it.
- Keep high-degree decision making accountable to a named person; bind action approvals to that identity, session, scope, and expiry.
- Authenticate and correlate iMessage decisions with the original request; message content alone does not expand tool access.
- Record action completion so retries and reconnects do not blindly repeat external changes.
- Provide visible pause, stop, failure, and host-unavailable states.

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
