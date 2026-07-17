# AEP Housekeeping

Assess schemas, field groups, datasets, namespaces, dataflows, audiences, destinations, and other visible resources for:

- Duplicate purpose or semantics.
- No recent activity or consumer.
- Broken, disabled, or stale execution.
- Missing owner, description, naming, tags, or lifecycle state.
- Orphaned upstream or downstream dependencies.
- Non-production assets in production sandboxes.
- Profile enablement without a current use case.

An asset is not safe to delete merely because no recent activity is visible. Build a dependency map, identify the owner, define an observation or quarantine period, capture an export or recovery route where possible, and validate downstream behavior. Prefer disable, deprecate, or stop-ingestion stages before irreversible deletion.

Output candidates with evidence, confidence, dependencies, risk, proposed action, and required approval.
