# Can.AI Public Security Design

This repository contains public product-design documentation and fictional examples. The controls below are implementation requirements for the proposed office-installed session manager, not certifications or claims that a production system has already passed validation.

## Identity and access

- Distinguish Can.AI seat ownership, administrator privileges, provider authentication, host enrollment, and approval authority.
- Preserve each user's provider and session boundaries on a shared office host.
- Store credentials in an approved credential store; exclude them from exported profiles, messages, and logs.
- Give the senior engineer controlled access to profile configuration without distributing their provider identity to other users.

## Computer actions and decisions

- Define allowed workspaces, tools, triggers, execution identities, and resource limits in versioned PowerTools profiles.
- Present proposed edits for review where the workflow requires it.
- Bind approvals to the authorized reviewer, action, session, scope, and expiry.
- Treat document content and channel messages as input, not as permission to expand tool access.
- Record action completion so retries and reconnects do not blindly repeat external changes.
- Provide visible pause, stop, failure, and host-unavailable states.

## On-premises and outbound data

The office host executes local tools and retains configured working state. Hosted inference and messaging still transmit selected data to their respective services. Deployment review must identify those destinations, the information sent, applicable provider settings, and any portal telemetry. On-premises installation alone does not establish offline operation, data residency, or a compliance certification.

## Operations

The intended deployment process includes verified installation packages, controlled updates, host and session isolation, retention settings, recovery tests, and a review of each third-party integration. The administrator must verify effective permissions in the installed runtime as well as in Can.AI's panel.

## Reporting

Use GitHub's private vulnerability-reporting feature if it is enabled. Avoid posting sensitive findings or credentials in public issues.
