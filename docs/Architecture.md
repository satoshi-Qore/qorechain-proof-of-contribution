# Architecture

## Overview

The Proof of Contribution architecture is proposed as a layered framework for recording, validating, and interpreting human contribution in decentralized ecosystems. It should not be treated as a simple points system. Its purpose is to preserve contribution history with enough context for future governance, research, community coordination, and reputation analysis.

## Proposed Layers

| Layer | Purpose |
|---|---|
| Contribution Event Layer | Defines what type of contribution is being recorded |
| Evidence Layer | Links contribution claims to supporting material |
| Attestation Layer | Records validation by reviewers, systems, communities, or protocols |
| Reputation Layer | Interprets verified contribution history over time |
| Governance Interface | Allows contribution records to inform ecosystem decisions |
| Privacy and Disclosure Layer | Controls public visibility and contributor consent |

## Contribution Event Layer

A contribution event is a structured record describing an action that may have ecosystem value. Examples include a merged pull request, documentation improvement, issue report, governance analysis, node operation record, educational article, translation, security disclosure, or onboarding support.

Each event should include:

- Contribution type
- Contributor identifier or pseudonymous address
- Evidence reference
- Timestamp or period
- Attestation status
- Limitations or review notes

## Evidence Layer

The evidence layer should avoid storing unnecessary personal data directly on-chain. Instead, it may store references, hashes, metadata, or attestations connected to public evidence.

Possible evidence types include:

- GitHub pull requests and issues
- Published documentation
- Governance votes or proposals
- Infrastructure uptime records
- Community education materials
- Security reports
- Review notes or moderator attestations

## Attestation Layer

Attestations indicate that a contribution has been reviewed, acknowledged, or validated. Attesters may include maintainers, governance participants, protocol modules, community reviewers, or automated verification systems.

A strong architecture should distinguish between:

- Self-claimed contribution
- Peer-attested contribution
- Maintainer-attested contribution
- Protocol-verified contribution
- Independently audited contribution

## Reputation Layer

The reputation layer should interpret contribution history without reducing it to a transferable token. Reputation should be contextual, evidence-aware, and resistant to purchase or transfer.

A contributor may have different reputation profiles across categories, such as documentation, infrastructure, security, governance, or education.

## Governance Interface

Contribution records may inform governance decisions, but they should not automatically replace voting, delegation, or deliberation. Possible governance uses include contributor grants, reviewer selection, role assignment, proposal context, and historical accountability.

## Design Constraint

The architecture must avoid converting contribution into a speculative asset. Its purpose is memory, verification, and reputation, not farming.