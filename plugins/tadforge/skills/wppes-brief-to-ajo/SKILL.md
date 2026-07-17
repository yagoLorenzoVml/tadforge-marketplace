---
name: wppes-brief-to-ajo
description: Build draft AEP or Adobe Journey Optimizer campaigns and journeys from briefs and email files in .ao/uploads. Use when a user supplies a brief plus HTML and images and asks to create, prepare, or validate campaign or journey email content.
---

# Brief to AJO

Use [`references/brief-to-ajo.md`](references/brief-to-ajo.md). Read source files from `.ao/uploads`, upload each referenced image separately with `tadforge-upload-email-image`, then create email content with `tadforge-create-content-template`. Use the existing AEP tools for audiences, campaigns, journeys, and campaign duplication. Create drafts only; never activate or publish a campaign or journey.
