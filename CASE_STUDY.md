# Fictional Case Study: Northstar Claims Intake

This fictional scenario illustrates the intended workflow without using customer or employer information.

## Situation

Northstar Insurance receives claims through email, phone calls, and a web form. Intake specialists manually reconcile incomplete information before a claim can be assigned for review. Business rules are spread across policy documents and team notes.

## Goal

Create a reviewable implementation package for a consolidated claims-intake case workflow.

## Inputs

- A fictional intake-policy document
- Workshop notes from fictional stakeholders
- A sample claims form containing synthetic data
- A list of assumed downstream systems

## CanaClaw workflow

1. Identify candidate actors, stages, data objects, and policy rules.
2. Separate explicit requirements from assumptions.
3. Produce clarification questions for missing or conflicting details.
4. Draft a case structure and prioritized user stories.
5. Require a reviewer to accept or revise the package before export.

## Result

The output package gives an implementation team a consistent starting point while preserving the distinction between source-backed requirements, inferred recommendations, and unresolved questions.

## Product decisions demonstrated

- Every assumption is labeled instead of presented as a fact.
- External actions remain outside the showcase workflow.
- Review checkpoints are part of the design, not an afterthought.
- Outputs are structured for both human reading and machine processing.
