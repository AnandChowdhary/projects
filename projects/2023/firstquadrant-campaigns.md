---
title: Campaigns on FirstQuadrant
tags: projects
intro: AI-personalized outbound campaigns with sequence editing, audience qualification, deliverability, and pipeline tracking
date: 2023-09-01
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-campaigns/sequence-editor
img_type: png
stack: ["TypeScript", "React", "Next.js", "OpenAI", "SendGrid"]
---

Campaigns was the outbound engine: take a [qualified audience](/projects/2023/firstquadrant-prospecting), generate personalized emails in the sender's voice, send them through connected mailboxes, and hand replies into [Actions](/projects/2024/firstquadrant-actions) for human-reviewed follow-up. It was the bridge between top-of-funnel data and warm sales conversations.

The campaign overview was designed for scanability. Each campaign had a status, progress indicators, and counts for contacts that were completed, running, sequenced, or still pending. Starting a campaign was guarded by readiness checks: the workspace needed an active subscription, at least one sender, an audience, a variant, and at least one sequence step. Pausing a campaign could be soft, where already-started sequences kept running, or hard, where running sequences and scheduled drafts were stopped.

![Campaign list with active outbound programs and delivery status](/assets/firstquadrant-campaigns/campaigns.png)

Editing a campaign was a checklist rather than a blank canvas. The main setup sections were Senders, Audience, and Sequence, with advanced configuration for Pipelines, Product or service, and Sending schedule. That structure made it clear what had to be configured before the switch could go from draft to running.

The sequence editor was where the product felt most different from traditional mail merge. The yellow variables were not simple find-and-replace tokens. They were LLM instructions embedded directly in the template, like “insert a personal anecdote about their team, market, or recent launch.” Each variable could have its own length setting and example, so the system knew whether it should generate a two-word phrase, a short sentence, or a fuller contextual passage.

![Sequence editor with LLM-generated personalization variables](/assets/firstquadrant-campaigns/sequence-editor.png)
![Campaign audience and qualification filters](/assets/firstquadrant-campaigns/audience.png)

Audience management connected campaigns back to the CRM. Campaigns could pull from saved contact views and imports, then show every resulting sequence with its status. Opening an audience row showed the same rich contact context panel used elsewhere: contact details, company details, enrichment, custom properties, related deals, and activity history.

The generation model used the whole campaign envelope: sender identity, recipient and company context, qualification answers, custom properties, product/service details, and previous steps in the sequence. Follow-ups were aware of the earlier message instead of being separate templates stitched together by date.

Deliverability engineering was critical. We supported Google Workspace, Microsoft 365, Exchange, Zoho, and IMAP mailboxes, plus outbound-specific accounts. Campaigns could inherit the workspace sending schedule or override it with their own weekday windows and recipient-time-zone behavior. The same inheritance pattern applied to product details and pipelines: use workspace defaults when possible, override only when a campaign needed a specific offer, schedule, or conversion pipeline.

![Campaign sending schedule controls](/assets/firstquadrant-campaigns/schedule.png)
![Product and service context for generated outreach](/assets/firstquadrant-campaigns/product.png)
![Pipeline targeting for campaign conversion tracking](/assets/firstquadrant-campaigns/pipelines.png)

Pipeline targeting made campaign outcomes measurable. When someone replied positively, FirstQuadrant could create or associate deals in the selected pipeline and then surface conversion in analytics. The result was a loop: prospecting created the audience, campaigns generated the outreach, actions handled the replies, and analytics showed whether the work created pipeline.

We shipped Campaigns as a living system, not a one-off feature. Over time it grew language support, richer variables, mailbox management, HTML email handling, unsubscribe logic, campaign analytics, variants, autopilot, and deeper CRM attribution. For a while, the Monday changelog rhythm was almost part of the product itself.

## Additional product views

Campaigns depended on the surrounding infrastructure: connected mailboxes for sending, calendars for meeting detection, and workspace-level schedules that kept outbound inside sane delivery windows.

![Connected email accounts and sending health](/assets/firstquadrant-campaigns/mailboxes.png)
![Connected calendar accounts](/assets/firstquadrant-campaigns/calendars.png)
![Workspace sending schedule](/assets/firstquadrant-campaigns/sending-schedule.png)
