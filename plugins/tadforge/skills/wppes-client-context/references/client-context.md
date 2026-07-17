# IKEA Client Context

## Confirmed baseline

- Client: IKEA.
- Platform focus: Adobe Experience Platform.
- Live platform information must be obtained from the plugin-provided `aep` MCP server.
- No specific sandbox, market, schema, dataset, namespace, merge policy, audience, source, destination, SLA, owner, or governance rule is confirmed by this document.

## Evidence hierarchy

Use sources in this order:

1. Current MCP results from the explicitly selected sandbox.
2. Approved documentation or requirements supplied by the user.
3. This skill's general retail-domain hypotheses, clearly labelled as assumptions.
4. General AEP best practice, clearly labelled as a recommendation.

If sources conflict, report the conflict instead of choosing silently. Live configuration proves what exists, but it does not automatically prove that the configuration is intended or compliant.

## Plausible domain concepts, not implemented facts

The following concepts can help frame discovery but must not be presented as existing fields or resources:

- Customer and household profiles.
- IKEA Family or another membership relationship.
- Product, range, category, room, and style affinity.
- Store, market, language, and fulfilment preferences.
- Web, app, store, contact-centre, and campaign interactions.
- Basket, order, delivery, return, planning, and appointment events.
- Marketing consent, channel permissions, and privacy requests.

Before using any concept in a design, identify its actual XDM path, source, identity, freshness, consent basis, owner, and quality controls.

## Discovery checklist

For account-specific work, establish:

- Organization, sandbox, environment type, region, and business owner.
- Business objective, KPI, market, legal basis, and intended activation.
- Schemas, field groups, datasets, sources, dataflows, and ingestion cadence.
- Identity namespaces, primary identities, identity graph behavior, and merge policies.
- Profile and segmentation enablement.
- Audiences, destinations, mappings, schedules, and activation state.
- Data usage labels, policies, consent fields, retention, and deletion processes.
- Naming, tagging, lifecycle, promotion, incident, and ownership conventions.

Do not invent missing values. Record them as discovery gaps with an owner and next action when known.
