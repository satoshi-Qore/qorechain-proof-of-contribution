# Reputation Layer

## Overview

The reputation layer interprets verified contribution history over time. In a Proof of Contribution framework, reputation should not be designed as a transferable asset or speculative score. It should function as contextual memory about a contributor's history, reliability, and area of contribution.

## Design Goals

- Preserve long-term contribution history
- Distinguish contribution quality from activity volume
- Support category-specific reputation
- Resist purchase, transfer, and artificial farming
- Provide context for governance and ecosystem coordination
- Protect contributor privacy and pseudonymity where possible

## Contextual Reputation

A contributor may be strong in one area and inexperienced in another. For example, a person may have high documentation reputation but no validator operation history. A useful reputation layer should therefore avoid a single universal score.

Suggested categories:

- Documentation
- Protocol research
- Infrastructure operation
- Governance participation
- Security review
- Education and onboarding
- Translation and localization
- Community moderation
- Developer tooling

## Non-Transferability

Contribution reputation should be linked to contributor history rather than transferable ownership. If reputation can be sold, delegated without context, or moved as a financial asset, it becomes less useful as a signal of human contribution.

Non-transferability may be implemented through:

- Soulbound-style credentials
- Pseudonymous contributor profiles
- Attestation-linked identifiers
- Governance-controlled role assignment
- Reputation records without token transfer rights

## Reputation Decay and Recency

A protocol may need to distinguish old contribution history from recent activity. Reputation decay should be studied carefully because older contributions may remain valuable as ecosystem memory, while recent activity may better represent current availability.

Possible approaches:

- No decay for historical records
- Category-specific recency weighting
- Separate lifetime and recent contribution views
- Manual review for high-impact roles

## Risks

| Risk | Description |
|---|---|
| Score reductionism | Complex contribution becomes oversimplified into a number |
| Reputation farming | Users optimize for visible metrics rather than useful work |
| Social centralization | A small group controls recognition and validation |
| Privacy exposure | Contributors reveal more identity history than intended |
| Governance capture | Artificial contribution history influences decision-making |

## Research Position

The reputation layer should be evidence-aware, contextual, non-transferable, and transparent about its limits. It should help communities remember contribution history without turning reputation into a market object.