---
title: Actions on FirstQuadrant
tags: projects
intro: Human-in-the-loop AI inbox where sales teams review, approve, and refine AI-generated outreach actions
date: 2024-05-20
work: ["Web", "FirstQuadrant"]
bg: "#1a1a2e"
style: cover
img_src: /assets/firstquadrant-actions/inbox-dark
img_type: jpg
stack: ["TypeScript", "React", "Next.js", "OpenAI GPT-4o", "BullMQ"]
---

Actions was our answer to a core belief: fully autonomous AI sales is a bad idea — not because the AI can't do it, but because people shouldn't have to blindly trust it. This was the cockpit where AI did the heavy lifting and humans stayed in control.

![The full Actions inbox — conversation thread, contact panel, and command palette](/assets/firstquadrant-actions/inbox-dark.jpg)

At its core, Actions is a smart inbox organized into views: Todo (items needing review), Replies (sent responses), Follow-ups (scheduled emails), Snoozed (deferred to tomorrow, weekend, or next week), Scheduled, Sent, and Completed. Keyboard navigation, multi-select for bulk approvals, and a context panel showing the full conversation thread and contact details.

![Todo queue with contacts, companies, and sentiment tags](/assets/firstquadrant-actions/todo-queue.jpg)
![Todo list with action types and color-coded classifications](/assets/firstquadrant-actions/todo-list.jpg)

The engine behind Actions was the Brain — our autonomous reasoning system powered by GPT-4o. Brain ingests the entire conversation history and decides what to do next: draft a reply for positive emails, answer questions from campaign context, reschedule follow-ups around out-of-office dates, unsubscribe negative contacts, or flag ambiguous cases for human review. Every action includes the AI's reasoning, so you always know *why* it made a decision.

![Brain flagging a manual action with reasoning](/assets/firstquadrant-actions/manual-action.jpg)
![Brain scheduling a follow-up with contextual reasoning](/assets/firstquadrant-actions/brain-followup.jpg)

The approval flow lets you approve, edit, or reject any AI-generated action. Rejections include feedback that feeds into "Feedback memory" per campaign — corrections the Brain references for all future actions.

![Providing feedback to the Brain on a follow-up](/assets/firstquadrant-actions/brain-feedback.jpg)
![Snooze options — tomorrow, this weekend, next week](/assets/firstquadrant-actions/snooze-options.jpg)

We designed a deliberate trust gradient: start in manual mode (approve everything), move to sampling (autopilot on X% of contacts), then full autopilot where Brain handles everything except truly uncertain cases.

![Autopilot settings with sequence sampling at 50%](/assets/firstquadrant-actions/autopilot-sampling.jpg)

We also built full conversation management with HTML email rendering, calendar integration that auto-detects scheduled meetings (feeding conversion signals back to [prospecting](/projects/2023/firstquadrant-prospecting) and [campaigns](/projects/2023/firstquadrant-campaigns)), and notifications via in-app bell and Slack Connect channels.

![Full conversation thread with approval flow](/assets/firstquadrant-actions/conversation-thread.jpg)
![In-app notifications for qualification and campaign events](/assets/firstquadrant-actions/notifications.jpg)
