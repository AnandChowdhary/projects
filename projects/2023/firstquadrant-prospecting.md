---
title: Prospecting & Qualification on FirstQuadrant
tags: projects
intro: AI-powered lead finding, enrichment, and qualification engine for hyper-targeted B2B outbound sales
date: 2023-06-01
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-prospecting/qualification-criteria
img_type: jpg
stack: ["TypeScript", "React", "Next.js", "Prisma", "Apollo.io"]
---

Before you can run [campaigns](/projects/2023/firstquadrant-campaigns) or handle [actions](/projects/2024/firstquadrant-actions), you need an audience — and not just any list, but one that's been enriched, filtered, and qualified so every contact is worth emailing.

The primary way to build an audience is through our Apollo.io integration. Apollo has over 100 million contacts, and we built a prospecting tool that lets you search through them without leaving FirstQuadrant. Filters include company headcount, HQ location, industry, revenue, funding rounds, technologies, and open positions on the company side, plus job title, management level, previous employers, and department on the contact side.

![AI prospecting filter with custom qualification questions](/assets/firstquadrant-prospecting/ai-prospecting-filter.jpg)

For teams with existing lists, we built CSV import supporting over 50 columns — everything from basic contact info to company funding data, social URLs, and tech stack. Each row goes through enrichment and shows a clear status: Successful, Skipped, or Failure.

We also built integration audiences — a Zapier connector and a Campaign API with public `fqa_pub_` keys, so leads can flow in programmatically from forms, webhooks, or CRMs.

![HubSpot and webhook integrations](/assets/firstquadrant-prospecting/integrations.jpg)

The most powerful feature was AI Qualification. Using LLMs, we'd analyze each contact against default criteria (company name known, website active, email verified) plus custom filter questions like "Does this company offer remote work?" For each question, the AI conducts web searches per contact to find the answer — computationally expensive, but the targeting precision was remarkable.

![Qualification criteria with filter questions](/assets/firstquadrant-prospecting/qualification-criteria.jpg)
![Qualification table with manual overwrite](/assets/firstquadrant-prospecting/qualification-table.jpg)

We later added audience segmentation — creating new audiences from segments of existing ones based on qualification results. This enabled campaign chaining: run a broad campaign, segment the non-responders who met some criteria, and hit them with more targeted messaging.

![Audience segmentation from existing campaigns](/assets/firstquadrant-prospecting/segment-audiences.jpg)
