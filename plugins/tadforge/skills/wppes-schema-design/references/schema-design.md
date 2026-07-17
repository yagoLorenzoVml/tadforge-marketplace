# XDM Schema Design

## Procedure

1. Confirm the business event, entity, and consumers.
2. Inventory reusable standard and tenant field groups in the target sandbox.
3. Select the XDM class from semantics, not convenience.
4. Map every source field to an XDM path with type, requiredness, example, transformation, sensitivity, identity role, and owner.
5. Validate arrays, enums, cardinality, timestamps, currencies, locale, and reference identifiers.
6. Decide Profile enablement independently for schema and dataset, based on a documented use case.
7. Check compatibility with downstream audiences, Query Service, destinations, and existing ingestion.
8. Define evolution, backfill, validation, and rollback behavior.

## Rules

- Prefer standard XDM semantics when they accurately represent the concept.
- Extend under the tenant namespace only when required and document why.
- Do not overload one field with multiple meanings or encode structured data in strings.
- Event schemas require a valid event timestamp and stable event semantics.
- Record schemas must have deliberate identity and update semantics.
- Treat schema changes as contracts; assess existing datasets and consumers before mutation.

Return a mapping table and explicit decisions. Do not create or alter components without the change-safety confirmation process.
