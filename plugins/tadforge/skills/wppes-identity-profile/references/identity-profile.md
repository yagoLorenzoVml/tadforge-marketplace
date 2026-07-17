# Identity and Profile Review

## Review sequence

1. Define each identifier's issuing authority, format, stability, uniqueness domain, authentication state, and lifecycle.
2. Inventory identity namespaces and schema identity descriptors.
3. Trace identities from source through dataset and Profile.
4. Identify collision, shared-device, recycled-ID, household-versus-person, and anonymous-to-known stitching risks.
5. Inventory Profile-enabled schemas and datasets and estimate fragment growth.
6. Review merge policies, precedence, and edge cases using representative profiles.
7. Validate consent and deletion behavior across linked identities.

## Rules

- Namespaces are semantic contracts, not labels for every identifier-like field.
- A primary identity must be present and trustworthy for the records that declare it.
- Do not use namespace creation or merge policy changes to hide upstream quality defects.
- Separate person, household, device, membership, order, and other entity concepts.
- Profile enablement needs a named activation or personalization consumer.
- Test both desired stitching and dangerous over-stitching.

Report graph risks and merge outcomes with evidence; never expose raw personal data unnecessarily.
