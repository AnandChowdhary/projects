---
title: Actions on FirstQuadrant
tags: projects
intro: Human-in-the-loop command center where sales teams review, approve, and tune AI-generated next steps
date: 2024-05-20
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-actions/actions-overview
img_type: png
stack: ["TypeScript", "React", "Next.js", "OpenAI GPT-4o", "BullMQ"]
---

Actions was our answer to a core belief: fully autonomous AI sales is a bad idea — not because the AI cannot do it, but because people should not have to blindly trust it. The product needed a daily operating surface where the AI could do the expensive reasoning work and the human could stay in control of judgment, tone, and timing.

![Actions cockpit with reviewed AI tasks, contact context, and deal signals](/assets/firstquadrant-actions/actions-overview.png)

At its core, Actions was an AI-generated task inbox. Each row came from a real contact activity: an inbound email, a meeting signal, a stale deal, a campaign response, a note, or an imported lead that was ready for reasoning. Instead of forcing reps to dig through email threads and CRM views, FirstQuadrant translated the latest signal into a proposed next step: approve a reply, schedule a follow-up, research a buying committee, attach a source citation, or prepare a procurement summary.

The page itself was intentionally dense. The status selector kept the daily workflow simple: To do, Later, and Done. The table could be filtered by owner, label, contact, company, deal, campaign, sequence status, email verification, location, seniority, and last touchpoint. Selecting a row opened a read-only contact panel, so a reviewer could see the person, company, enrichment, emails, related deals, and custom properties without leaving the list.

The engine behind Actions was the Brain, our autonomous reasoning system powered by GPT-4o. Brain read conversation history, contact and company context, pipeline state, campaign context, workspace settings, and fine-tuning rules. When a new signal arrived, the plan was not treated as a static workflow. Brain re-evaluated the situation and proposed the next best action with the latest context.

The human controls were deliberately close to the row. You could approve, reject, snooze for a day/week/month, rerun AI reasoning, or sync the action back to the source system. When the system was still processing contacts, the header showed a live “processing contacts” control so teams understood that the list was being computed in the background rather than manually maintained.

![Fine-tuning rules that guide AI action generation](/assets/firstquadrant-actions/fine-tuning.png)

Fine-tuning was how we made the Brain controllable without turning it into brittle if-this-then-that automation. Teams could create typed rules for email received, notes, knowledge, nurturing, and general behavior. A rule could apply everywhere or be scoped to specific campaigns, imports, pipelines, or saved contact views. Email rules doubled as classification labels; knowledge rules answered recurring questions like pricing or security; general rules shaped tone and writing style.

Autopilot sat behind that trust model. For rules where the team was comfortable, FirstQuadrant could automatically approve generated emails and schedule them for sending. For everything else, the AI still did the draft and reasoning work, but the action stayed in the review queue until a person approved it.

We designed the system around a trust gradient: start in manual mode, learn from rejections and edits, scope behavior through fine-tuning, then gradually enable autopilot for the categories of work that had become predictable.

We also connected Actions to the rest of the CRM. Calendar events could mark meetings as scheduled, email replies could move contacts through campaigns, and deal context could surface directly inside the action row. The goal was not just “send this email,” but “move this relationship forward with the right amount of human review.”

![Pipeline analytics connecting AI actions to deal outcomes](/assets/firstquadrant-actions/pipeline-analytics.png)

That is why the analytics layer mattered. Pipeline analytics tracked created deals, won deals, conversion rate, won value, weighted value, and total value, with breakdowns by owner and company. Because actions were tied to contact activities, and contacts could be points of contact on deals, the product could draw a line from an AI-suggested reply to pipeline movement.

## Additional product views

The deal pipeline was the other half of the story: Actions handled the daily execution, while deals and analytics made the outcome measurable.

![Deals pipeline linked to action context](/assets/firstquadrant-actions/deals.png)
