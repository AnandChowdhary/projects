---
title: FirstQuadrant.ai
tags: projects
intro: The public site, docs, changelog, and platform settings around FirstQuadrant's sales product
date: 2024-02-21
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-website/homepage
img_type: png
stack: ["TypeScript", "React", "Next.js", "Tailwind CSS", "MDX"]
---

The FirstQuadrant website had one hard job: explain a fairly complex sales product before visitors bounced. The positioning changed as the product got clearer. We went from "All-in-one AI sales platform" at YC launch, to "AI sales execution platform," and eventually to "Maximize B2B sales with human-centered AI." That last line matched what we were actually building: AI that helps humans do better sales work, centered on the [Actions](/projects/2024/firstquadrant-actions) cockpit and Brain.

![Homepage showing FirstQuadrant's AI sales platform positioning](/assets/firstquadrant-website/homepage.png)

The final homepage led with the simplest promise we could make, then used motion and product screenshots to show what the platform actually did. The hero carried the YC and Product Hunt signals, a demo video, and an animated screenshot stack. A screenshot module let visitors switch between AI Conversations, AI Actions, AI Enrichment, and AI Campaigns, which mapped directly to the product surfaces we had built.

Below the hero, the site framed FirstQuadrant around three motions: Convert, Nurture, and Grow. Convert covered pipeline and deal work. Nurture covered reactivation and ongoing relationships. Grow covered top-of-funnel campaigns. That structure helped because the product was a loop: find contacts, enrich and qualify them, generate campaigns, review actions, and measure pipeline outcomes.

The interactive sections used normal sales scenarios: canceled meetings, positive replies, postponed conversations, competitor objections, and nurturing. The point was simple: FirstQuadrant read the conversation, understood the relationship, planned the next step, and kept following up.

Our YC Launch page leaned into personality: "This is the startup's philosopher stone that turns lead into gold." Founders who signed up within 48 hours got priority waitlist access.

The changelog became one of my favorite parts. We published weekly updates every Monday for over six months, including bug fixes. The consistency became its own kind of marketing.

We also built a documentation site powered by Mintlify, an API reference, and a free [Deliverability Guide](https://deliverabilityguide.com) about email infrastructure. The site was the public home for positioning, docs, changelog, launch announcements, developer guidance, and trust-building.

![App integrations catalog](/assets/firstquadrant-website/apps.png)
![API key list with last-usage history](/assets/firstquadrant-website/api-keys.png)
![Contacts CSV export](/assets/firstquadrant-website/data-export.png)

The settings screenshots show the product infrastructure behind the public story. Apps gave teams one place to manage integrations: HubSpot, Zapier, Vector, Cal.com, Segment, RB2B, Slack Connect, Perplexity, and other import or sync sources. API keys supported server-to-server workflows and showed last-usage history. Behind the UI, the API model also supported scopes, expiration, IP ranges, and app ownership. Data export gave customers a simple contacts CSV backup path for reporting and portability.

Those details mattered because FirstQuadrant sat inside a customer's revenue stack. It had to send mail, sync calendars, ingest product and form events, enrich properties, write back to CRMs, expose APIs, and still feel like one product.

The site supported dark and light themes, professional email validation, locale detection, animated product storytelling, and a performance-focused frontend. Built with Next.js App Router, Tailwind CSS, and TypeScript, it got the same attention to polish and operational detail as the app itself.

## Additional product views

The admin surfaces rounded out the product: workspace settings for operational control, members for team collaboration, and properties for structured CRM data that AI could enrich and use for segmentation.

![Workspace general settings](/assets/firstquadrant-website/general-settings.png)
![Workspace member management](/assets/firstquadrant-website/members.png)
![Custom CRM properties](/assets/firstquadrant-website/properties.png)
![Full homepage capture](/assets/firstquadrant-website/homepage-full.png)

[**Visit FirstQuadrant →**](https://firstquadrant.ai)
