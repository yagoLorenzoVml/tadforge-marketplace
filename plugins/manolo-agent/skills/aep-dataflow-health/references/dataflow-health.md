# Dataflow Health

For each flow identify source, target dataset, schedule or streaming mode, last successful activity, current state, records received, accepted, failed, and skipped where available, freshness versus SLA, error samples or categories, and downstream consumers.

Prioritize incidents by business impact and blast radius, not error count alone. Check schema changes, credentials, source availability, mapping, required fields, identity quality, duplicate delivery, backfill behavior, and platform limits.

Report:

- Status and evidence window.
- Impacted resources and consumers.
- Most likely causes, separated from confirmed causes.
- Safe diagnostics and immediate containment.
- Recovery and replay plan with duplicate controls.
- Validation and monitoring criteria.

Never recommend blind replay into production. Establish idempotency, time bounds, reconciliation, and destination consequences first.
