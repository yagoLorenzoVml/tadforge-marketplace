---
name: wppes-brief-to-ajo
description: Build draft AEP or Adobe Journey Optimizer campaigns and journeys from briefs and email files in .ao/uploads. Use when a user supplies a brief plus HTML and images and asks to create, prepare, or validate campaign or journey email content.
---

# Brief to AJO

Use [`references/brief-to-ajo.md`](references/brief-to-ajo.md). Read the supplied brief, resolve or create its audiences with `audience-creation-flow`, create AJO content templates from each referenced GCS brief ZIP with `tadforge-create-template-from-brief`, then use `journey-create` for journey drafts. Create drafts only; never activate or publish a journey.
