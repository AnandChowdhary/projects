---
title: FirstQuadrant.ai
tags: projects
intro: Marketing website, documentation, changelog, and product infrastructure for FirstQuadrant's AI sales platform
date: 2024-02-21
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-website/homepage
img_type: png
stack: ["TypeScript", "React", "Next.js", "Tailwind CSS", "MDX"]
---

The marketing website for FirstQuadrant had to explain a complex AI sales platform in five seconds. The positioning evolved over time — from "All-in-one AI sales platform" at YC launch, to "AI sales execution platform," to the final "Maximize B2B sales with human-centered AI." That last framing reflected our actual product philosophy: AI that assists humans rather than replacing them, built around the [Actions](/projects/2024/firstquadrant-actions) cockpit and the Brain.

![Homepage showing FirstQuadrant's AI sales platform positioning](/assets/firstquadrant-website/homepage.png)

The final homepage led with the simplest possible promise, then used motion and product screenshots to make the breadth legible. The hero carried the YC and Product Hunt signals, a demo video, and an animated screenshot stack. The screenshot module let visitors switch between AI Conversations, AI Actions, AI Enrichment, and AI Campaigns, which mapped directly to the product surfaces we had built.

Below the hero, the site introduced FirstQuadrant as a sales execution platform with three product motions: Convert, Nurture, and Grow. Convert covered pipeline and deal work, Nurture covered reactivation and ongoing relationships, and Grow covered top-of-funnel campaigns. That structure was useful because the product was not one feature. It was a loop: find contacts, enrich and qualify them, generate campaigns, review actions, and measure pipeline outcomes.

The interactive sections explained context-aware decision-making using real sales scenarios: canceled meetings, positive replies, postponed conversations, competitor objections, and nurturing. Rather than describe the AI as magic, the copy emphasized that it read the conversation, understood the relationship, planned the next step, and kept following up.

Our YC Launch page leaned into personality: "This is the startup's philosopher stone — that turns lead into gold." Priority waitlist access for founders who signed up within 48 hours.

The changelog became one of my favorite parts — weekly updates every Monday for over six months, including bug fixes. Full transparency. The consistency of it became its own marketing.

We also built a comprehensive documentation site powered by Mintlify, an API reference, and a free [Deliverability Guide](https://deliverabilityguide.com) about email infrastructure best practices. The website was therefore not just a brochure. It was the public interface for positioning, docs, changelog, launch announcements, developer guidance, and trust-building.

![App integrations catalog](/assets/firstquadrant-website/apps.png)
![API key list with last-usage history](/assets/firstquadrant-website/api-keys.png)
![Contacts CSV export](/assets/firstquadrant-website/data-export.png)

The settings screenshots show the product infrastructure behind that public story. Apps gave teams a single place to manage integrations: HubSpot, Zapier, Vector, Cal.com, Segment, RB2B, Slack Connect, Perplexity, and other import or sync sources. API keys supported server-to-server workflows and showed last-usage history, while the API model supported scopes, expiration, IP ranges, and app ownership behind the scenes. Data export gave customers a simple contacts CSV backup path for reporting and portability.

Those details mattered because FirstQuadrant sat inside the customer's revenue stack. It had to send mail, sync calendars, ingest product and form events, enrich properties, write back to CRMs, expose APIs, and still feel like one coherent product.

The site supported dark and light themes, professional email validation, locale detection, motion-heavy product storytelling, and a performance-focused frontend. Built with Next.js App Router, Tailwind CSS, and TypeScript, it shared the same care for polish and operational detail as the rest of FirstQuadrant.

## Additional product views

The admin surfaces rounded out the platform story: workspace settings for operational control, members for team collaboration, and properties for structured CRM data that AI could enrich and use for segmentation.

![Workspace general settings](/assets/firstquadrant-website/general-settings.png)
![Workspace member management](/assets/firstquadrant-website/members.png)
![Custom CRM properties](/assets/firstquadrant-website/properties.png)
![Full homepage capture](/assets/firstquadrant-website/homepage-full.png)

[**Visit FirstQuadrant →**](https://firstquadrant.ai)
