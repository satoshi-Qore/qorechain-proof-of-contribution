# Verification Framework

## Overview

The Verification Framework defines how contribution claims may be evaluated within a Proof of Contribution research model. It is intended to clarify the relationship between submitted evidence, reviewer judgment, attestation strength, dispute handling, and long-term contribution records.

This document does not describe an implemented protocol. It is a conceptual framework for future specification work and should be evaluated as research guidance rather than a production design.

## Purpose

A Proof of Contribution system requires more than a list of activities. It must define how a contribution claim becomes credible, what evidence is required, who can review it, how disagreements are handled, and how records remain useful without becoming misleading.

The verification framework aims to:

- distinguish submitted claims from verified contribution records;
- classify evidence quality;
- define review outcomes;
- prevent activity volume from being mistaken for contribution value;
- support correction, dispute, and revision;
- preserve context for future reputation and governance analysis.

## Verification Flow

A contribution claim may move through several stages:

| Stage | Description | Expected Output |
|---|---|---|
| Submission | A contributor submits a contribution claim with supporting evidence | Draft contribution record |
| Evidence Review | Reviewers inspect links, artifacts, timestamps, and claimed scope | Evidence quality assessment |
| Context Review | Reviewers evaluate relevance, originality, and ecosystem usefulness | Contribution context note |
| Attestation | A reviewer, maintainer, or protocol source issues an attestation | Attested contribution record |
| Status Assignment | The claim receives a verification status | Claimed, observed, reviewed, accepted, verified, disputed, or rejected |
| Archival Record | The final or current status is preserved with evidence and limitations | Contribution memory entry |

## Evidence Categories

Different contribution types require different evidence. A merged pull request, a governance vote, a translated article, and a support interaction cannot be reviewed using the same standard.

| Evidence Type | Example | Strength | Limitations |
|---|---|---|---|
| Repository evidence | Pull request, issue, commit, review comment | High when public and traceable | May not show broader impact |
| Governance evidence | Proposal, vote, forum comment, decision record | Medium to high | May require context to interpret |
| Infrastructure evidence | Node logs, monitoring screenshots, configuration notes | Medium | May expose sensitive information |
| Educational evidence | Guide, tutorial, video, article, glossary | Medium | Quality may require human review |
| Community support evidence | Help thread, answer, onboarding note | Low to medium | Often fragmented or hard to verify |
| Social evidence | Post, reply, share, campaign activity | Low | Easily gamed and often low-context |
| Third-party evidence | Maintainer confirmation, audit report, external review | Medium to high | Depends on reviewer credibility |

## Evidence Quality Levels

| Level | Meaning | Example |
|---|---|---|
| Weak | Evidence exists but is incomplete, ambiguous, or difficult to verify | Screenshot without source link |
| Basic | Evidence confirms that an action occurred | Public post or visible comment |
| Contextual | Evidence shows action plus purpose, scope, and relevance | Issue with clear problem statement and discussion |
| Maintainer-confirmed | A maintainer or responsible reviewer accepted the contribution | Merged pull request or accepted documentation fix |
| Protocol-verifiable | Evidence can be independently verified through protocol or system data | On-chain vote or signed attestation |

Evidence quality should not be interpreted as contribution value by itself. A high-quality proof may document a small contribution, while a lower-quality proof may still represent meaningful work that requires additional review.

## Verification Statuses

| Status | Meaning | Use Case |
|---|---|---|
| Claimed | Submitted by the contributor but not yet reviewed | Initial record keeping |
| Observed | Evidence confirms the activity exists | Public link or artifact is visible |
| Reviewed | A reviewer has inspected the claim and evidence | Human review completed |
| Accepted | A responsible maintainer, reviewer, or community process accepted the work | Merged PR, accepted issue, approved guide |
| Verified | Strong evidence supports the claim with clear scope and review context | High-confidence contribution record |
| Disputed | The claim is challenged or evidence is insufficient/conflicting | Requires review or correction |
| Rejected | The claim is false, duplicated, misleading, or out of scope | Should not count as accepted contribution |
| Archived | The record is retained for history but no longer treated as active evidence | Older or superseded contribution record |

## Reviewer Roles

Verification depends on reviewer context. A single reviewer type should not be treated as universally authoritative.

| Reviewer Type | Suitable Review Scope | Limitation |
|---|---|---|
| Contributor self-review | Initial claim description and evidence submission | Not independent |
| Peer reviewer | Community usefulness, clarity, basic validation | May lack domain expertise |
| Maintainer reviewer | Repository, documentation, or project-level acceptance | May be limited to one domain |
| Governance reviewer | Proposal and decision context | May be politically influenced |
| Technical reviewer | Security, infrastructure, or protocol accuracy | May not assess community value |
| External reviewer | Independent research or audit context | May lack ecosystem-specific knowledge |

## Verification Criteria

A claim should be evaluated using multiple criteria rather than a single score.

| Criterion | Guiding Question |
|---|---|
| Existence | Did the contribution actually occur? |
| Attribution | Is the contributor reasonably linked to the work? |
| Originality | Is the contribution original or meaningfully adapted? |
| Relevance | Does the work relate to the ecosystem or research scope? |
| Usefulness | Did the contribution help users, maintainers, governance, infrastructure, or knowledge preservation? |
| Evidence quality | Are the sources public, durable, and reviewable? |
| Review independence | Was the claim reviewed by someone with sufficient context and limited conflict of interest? |
| Abuse risk | Could the claim be spam, duplicated, automated, or coordinated for artificial reputation? |

## Contribution Weighting Principles

This framework does not define a universal numerical score. However, it suggests principles for future systems that may need to interpret contribution significance.

- Quality should be separated from quantity.
- Contribution categories should remain distinct.
- Public visibility should not be treated as the same as usefulness.
- Repeated low-effort actions should not outweigh fewer high-context contributions.
- Reviewer notes should remain visible where possible.
- Reputation should reflect context, not permanent hierarchy.

## Dispute and Revision Process

A credible verification system should allow records to change when evidence changes.

Possible dispute flow:

1. A record is challenged by a contributor, reviewer, maintainer, or affected party.
2. The disputed reason is recorded.
3. Evidence is re-examined.
4. Reviewers may request clarification or additional proof.
5. The record may be confirmed, downgraded, corrected, rejected, or archived.
6. The revision history remains visible where appropriate.

Disputes should not be treated only as negative events. They are part of maintaining accurate ecosystem memory.

## Privacy and Safety Considerations

Contribution verification can expose sensitive information. A verification framework should avoid requiring unnecessary personal data.

Important safeguards include:

- avoiding private keys, seed phrases, IP addresses, and sensitive logs;
- allowing pseudonymous contribution records;
- supporting redaction for screenshots and infrastructure evidence;
- separating public contribution summaries from private review material;
- limiting identity requirements to cases where they are genuinely needed;
- preserving contributor agency over public-facing identity.

## Abuse Resistance Considerations

Verification must account for manipulation attempts, including:

- duplicate contribution submissions;
- copied or AI-generated low-quality content;
- fake social engagement;
- circular peer attestations;
- reviewer favoritism;
- reputation farming through repetitive tasks;
- false claims based on deleted or unverifiable evidence.

These risks should be addressed in a dedicated abuse resistance model, but they should already influence verification design.

## Example Verification Matrix

| Contribution Example | Evidence Needed | Likely Status if Valid | Notes |
|---|---|---|---|
| Merged documentation pull request | PR link, merge status, changed files | Accepted or Verified | Strong repository evidence |
| Meaningful issue report | Issue link, maintainer response, outcome | Reviewed or Accepted | Stronger if issue leads to improvement |
| Community guide | Public guide link, originality check, usefulness review | Reviewed | Requires human quality review |
| Light node operation note | Public note, redacted logs or screenshots, context | Observed or Reviewed | Avoid exposing sensitive server data |
| Governance participation | Proposal link, vote or comment, discussion context | Observed or Reviewed | Vote alone may not show contribution quality |
| Social media engagement | Public link or screenshot | Observed | Low evidence strength for contribution value |

## Open Research Questions

- What evidence standards should apply to each contribution category?
- How can verification remain fair to non-code contributors?
- How should systems treat pseudonymous contributors with strong evidence?
- What level of reviewer independence is required for high-impact claims?
- How should unverifiable but historically important contributions be archived?
- Can contribution verification remain useful without becoming a leaderboard?
- How can AI-assisted review be used without introducing false confidence?

## Conclusion

The Verification Framework is the central bridge between contribution claims and credible contribution memory. It should not reward activity automatically or turn contribution into a simple score. Its role is to preserve evidence, review context, limitations, and dispute history so that future reputation and governance systems can interpret contribution records responsibly.

Further work should refine contribution-specific evidence standards, reviewer role definitions, privacy safeguards, and abuse resistance mechanisms before any implementation is considered.
