---
title: Prospecting & Qualification on FirstQuadrant
tags: projects
intro: AI-powered contact ingestion, enrichment, and qualification for targeted B2B outbound workflows
date: 2023-06-01
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-prospecting/contacts
img_type: png
stack: ["TypeScript", "React", "Next.js", "Prisma", "Apollo.io"]
---

Before you can run [campaigns](/projects/2023/firstquadrant-campaigns) or handle [actions](/projects/2024/firstquadrant-actions), you need an audience. Not just a CSV of names, but contacts and companies that have been enriched, filtered, qualified, and connected to the rest of the CRM so the AI can reason about them.

The first version of prospecting centered on Apollo.io. Apollo had the breadth of B2B data we needed, and we built a workflow to search, filter, and qualify prospects without leaving FirstQuadrant. Over time, the product generalized into a broader imports system: CSV files, API/webhook intake, app integrations, saved views, visitor identification, and product signals could all become audiences.

That shift mattered because FirstQuadrant only became useful once a contact was explicitly in the workspace. Imported contacts could be enriched, appear in the CRM, be added to campaigns, receive AI reasoning, and eventually produce actions. Prospecting was the data gate for the rest of the product.

![Qualified contacts table with rich profile data](/assets/firstquadrant-prospecting/contacts.png)

The contact list became the operating database for that audience. It supported saved views, filters, import-specific views, counts, custom properties, and auto-refresh while enrichment was still running. Selecting a contact opened a context panel with the person, email addresses, social handles, employments, company information, related contacts, deals, and enriched properties. It was built for repeated sales work: scanning, segmenting, and opening context without losing your place.

For teams with existing lists, CSV import did a lot of heavy lifting. The uploader parsed CSV files, suggested field mappings from common header names, previewed sample values, validated rows, and supported contact, employment, and company fields. That meant a rough export from another tool could still become structured CRM data.

We also built integration audiences through app imports and API keys with `fqa_pub_` previews, so leads could flow in from forms, webhooks, website visitor tools, product analytics, or CRMs. Imports could run immediately or on a recurring schedule, which made them useful for both one-time lead lists and continuous sources like product signups.

![Import sources and enrichment workflows](/assets/firstquadrant-prospecting/imports.png)
![Import detail with row-level processing status](/assets/firstquadrant-prospecting/import-detail.png)

The most powerful feature was AI qualification. Every import could run standard checks such as company website availability, verified work email, professional email domain, and duplicate-contact exclusion. On top of that, users could add qualifying questions. Some questions used existing properties; others used web search. The row detail panel showed the answer, whether it qualified, the AI's reasoning, and source citations.

Qualification was also connected to cost and control. Web-search questions were more expensive than existing-property questions, and the import form made credit usage visible before starting. If criteria changed, the system could ask whether to re-qualify existing rows or only apply the new rules to future rows. Individual rows could also be qualified manually or re-run.

After qualification, teams could choose to run AI reasoning for qualified contacts. That step created the bridge into Actions: FirstQuadrant would decide what to do next, then create suggested emails or tasks for review.

We later added audience segmentation and richer account views. A broad campaign could generate engagement, qualification could identify the best-fit subset, and the team could turn that subset into a more targeted follow-up audience. The data model supported both individual contacts and account-level context, so prospecting could evolve into account-based sales motion instead of stopping at lead capture.

## Additional product views

Company pages completed the picture. They gave teams an account-level view of enrichment, custom properties, related contacts, deals, and activity history.

![Company account list with enrichment signals](/assets/firstquadrant-prospecting/companies.png)
![Company detail page with contacts, deals, and research context](/assets/firstquadrant-prospecting/company-detail.png)
