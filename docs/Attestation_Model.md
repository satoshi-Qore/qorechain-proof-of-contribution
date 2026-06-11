# Attestation Model

## Overview

The attestation model defines how contribution claims are reviewed and validated. In a Proof of Contribution framework, an attestation is not simply a like, badge, or reward marker. It is a structured statement that a contribution was observed, reviewed, accepted, or verified under specific conditions.

## Attestation Types

| Type | Description | Example |
|---|---|---|
| Self-attestation | Contributor records their own contribution claim | A user submits a documentation proof link |
| Peer attestation | Another community member acknowledges the contribution | A reviewer confirms a helpful guide |
| Maintainer attestation | A repository or project maintainer validates the work | A merged pull request |
| Protocol attestation | A protocol module records verifiable activity | On-chain governance vote |
| External attestation | An independent party confirms the contribution | Audit report or third-party review |

## Evidence Requirements

Attestations should include enough context to prevent ambiguous claims. A useful attestation may include:

- Contributor identifier
- Contribution category
- Evidence link or content hash
- Attester identity or role
- Review timestamp
- Scope of validation
- Limitations or dispute status

## Attestation Strength

Not all attestations have equal weight. A self-attested claim may be useful as a record but should not carry the same credibility as a maintainer-verified contribution or protocol-confirmed event.

Suggested strength levels:

| Level | Meaning |
|---|---|
| Claimed | Submitted by contributor, not yet reviewed |
| Observed | A contribution exists and can be inspected |
| Reviewed | A reviewer has examined the contribution |
| Accepted | A maintainer or governance process accepted it |
| Verified | The contribution is supported by strong public or protocol evidence |

## Anti-Abuse Considerations

The attestation model should address:

- Duplicate submissions
- Low-effort contribution spam
- Circular attestations between coordinated accounts
- Reviewer bias
- Fake or misleading evidence
- Link rot and disappearing proof
- Overreliance on social engagement metrics

## Dispute Handling

A complete model should include mechanisms for correction, dispute, expiration, or downgrade. Contribution records should not become permanent reputational errors when evidence changes or claims are challenged.

## Research Position

Attestation should be treated as a trust-minimized evidence process, not as automatic endorsement. The system should preserve contribution context while allowing future reviewers to evaluate the reliability of the claim.