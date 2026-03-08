---
title: Campaigns on FirstQuadrant
tags: projects
intro: AI-generated personalized email sequences with deliverability infrastructure for fully autonomous B2B outbound
date: 2023-08-01
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-campaigns/sequence-timeline
img_type: jpg
stack: ["TypeScript", "React", "Next.js", "OpenAI", "SendGrid"]
---

Campaigns is the outbound engine — taking a [qualified audience](/projects/2023/firstquadrant-prospecting), writing personalized emails in the user's voice, and sending them on autopilot. It bridges prospecting and [actions](/projects/2023/firstquadrant-actions): turning cold prospects into warm conversations.

Setting up a campaign is a multi-step flow. You pick an audience, configure qualification criteria, define enrichments (custom fields like "company mission" or "latest product launch" that AI researches per prospect), add context about your offering, write the email sequence, and select mailboxes.

![Multilingual content settings with enrichments and creativity slider](/assets/firstquadrant-campaigns/multilingual.jpg)

The email generation uses a few-shot approach: users write three sample emails to "train" the AI on their voice, and the system generates personalized outreach using full context — sender info, recipient details, company enrichments, and custom data. Follow-ups are contextually aware of previous emails in the sequence, the AI computes optimal follow-up timing, and the last follow-up casually mentions it's the final one.

![Campaign sequence timeline with scheduled follow-ups](/assets/firstquadrant-campaigns/sequence-timeline.jpg)

Deliverability engineering was critical. We support Google Workspace, Microsoft 365, Exchange, Zoho, and IMAP mailboxes with bulk CSV import. Smart ramp-up gradually increases sending volume with configurable randomness. Each mailbox gets a reputation score weighted toward recent days.

![Connect mailbox — all supported providers](/assets/firstquadrant-campaigns/mailbox-connect.jpg)
![Mailbox ramp-up schedule preview](/assets/firstquadrant-campaigns/rampup-schedule.jpg)
![Mailbox dashboard with warming scores](/assets/firstquadrant-campaigns/mailbox-dashboard.jpg)

We guide users to set up separate outbound domains and recommend six mailboxes per sender across two domains, with integration into warming providers like MailReach and Instantly.

![Mailbox selection per campaign](/assets/firstquadrant-campaigns/mailbox-selection.jpg)
![Bulk import mailboxes via CSV](/assets/firstquadrant-campaigns/bulk-import-mailboxes.jpg)

Campaigns support eight languages (English US/UK, Dutch, French, German, Romanian, Hindi, Swiss German), multiple goal types (link clicks, calendar events, manual), and Autopilot with sampling — test full autonomy on X% of contacts before going all-in. We shipped updates every Monday for over six months.
