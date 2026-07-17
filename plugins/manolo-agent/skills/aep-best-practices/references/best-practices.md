# AEP Delivery Standards

## Core principles

1. Start with a measurable use case, not a platform object.
2. Design lineage end to end: source to XDM to dataset to Profile or lake to audience to destination.
3. Reuse governed components deliberately; do not create near-duplicate schemas, field groups, namespaces, or audiences.
4. Separate development, validation, and production through an explicit sandbox and promotion strategy.
5. Minimize data collection and activation to what the approved purpose requires.
6. Make identity and consent behavior explicit before enabling Profile or activation.
7. Attach ownership, naming, description, lifecycle state, and operational monitoring to every production asset.

## Mandatory design gates

Before implementation, confirm:

- Objective, KPI, audience or consumer, owner, market, legal basis, and retention need.
- Source contract, volume, cadence, latency, backfill, deduplication, and failure behavior.
- XDM class and field semantics, required fields, types, cardinality, and evolution plan.
- Identity namespaces, primary identity, authenticated versus anonymous behavior, and stitching risks.
- Dataset Profile enablement, merge policy, and expected profile-fragment growth.
- Audience evaluation method, eligibility logic, exclusions, suppression, and expected population.
- Destination contract, mapping, consent enforcement, schedule, and deletion behavior.
- Monitoring, reconciliation, rollback, runbook, and hypercare ownership.

## Anti-patterns

Flag these directly:

- Production-first experimentation.
- Generic or ambiguous field names and ungoverned custom field groups.
- Creating a namespace for an identifier that is not stable and unique in its domain.
- Enabling Profile by default without a profile use case or growth assessment.
- Treating a merge policy as a data-quality fix.
- Audience logic without consent, suppression, recency, or market boundaries.
- Activation without deterministic mappings and count reconciliation.
- Manual duplication between sandboxes with no promotion record.
- Assets with no owner, description, consumer, monitoring, or retirement criterion.

## Review output

For each finding provide severity, resource and sandbox, observed evidence, impact, recommended remediation, and any dependency or confirmation required.
