---
title: Onboarding on Pabio.com
tags: projects
intro: Style quiz and onboarding flow for Pabio's personalized interior design and furniture rental service
date: 2021-12-22
work: ["Web", "Pabio"]
bg: "#ed7470"
style: cover
img_src: /assets/pabio-onboarding/cover
img_type: jpg
stack: ["TypeScript", "React", "Next.js", "Tailwind CSS"]
---

On the Pabio website, we designed a new onboarding flow to help users get started with the service and better qualify leads.

The flow starts with a style quiz, which asks users to select their preferred interior design styles from a set of images. The quiz is followed by a short form to collect contact information and a few more questions about the user's needs.

![Step 1](/assets/pabio-onboarding/1.jpg)
![Style description in step 1](/assets/pabio-onboarding/1-style.jpg)

The team at Cleverclip designed custom illustrations for the quiz and onboarding flow, and we implemented the flow in TypeScript, React, and Next.js, using Tailwind CSS for styling.

We ask customers which rooms they want to furnish, and show relevant questions based on their answers.

![Step 2](/assets/pabio-onboarding/2.jpg)
![Step 3](/assets/pabio-onboarding/3.jpg)
![Step 7](/assets/pabio-onboarding/7.jpg)
![Step 7](/assets/pabio-onboarding/8.jpg)

Pabio is available in Switzerland and Germany. We automatically detect the user's current location and preselect their region to personalize the experience. If they're based in a region we don't serve yet, we show a message and ask them to sign up for our newsletter.

![Step 13](/assets/pabio-onboarding/13.jpg)

We then ask them to upload their floor plan and any photos of their empty apartment to be able to generate photorealistic 3D renderings of their furnished apartment.

![Upload your floor plan](/assets/pabio-onboarding/floor-plan.jpg)
![Take some photos of your home office](/assets/pabio-onboarding/photos.jpg)

Finally, we ask them to select a date and time for a free consultation call with one of our interior designers. We integrate with Calendly to show available time slots and automatically create a meeting in their calendars.

![Step 14](/assets/pabio-onboarding/consulting-call.jpg)
![Step 14](/assets/pabio-onboarding/schedule-call.jpg)

After the call, we send them a summary of the call and a link to their personalized furniture proposal, which you can see on the [Pabio.com proposal](/projects/2021/pabio-proposal) page.
