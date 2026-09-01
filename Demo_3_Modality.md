# From Proposal to Interactive Experience

**THIS IS A DEMONSTRATION BY THE INSTRUCTOR AND NOT MEANT AS A FOLLOW-ALONG, YOU MAY NOT HAVE SOME OF THESE FEATURES ENABLED IN YOUR COPILOT ENVIRONMENT**

_This prompt turns the same written proposal into three different formats: a visual roadmap slide, a clickable web walkthrough, and a working app you can use live with a client._

> Lets turn a proposal you've already worked with into something visual instead. Attach the Harborview proposal and ask for a slide instead of a paragraph, and notice how much of the table's structure (the phases, the durations) survives the jump into something a client could actually look at.

## Step 1: The Visual Roadmap

Attach: [Proposal_Harborview_Data_Migration](https://github.com/roitraining/ai-masterclass/blob/main/assets/Proposal_Harborview_Data_Migration.docx)

Begin by selecting the PowerPoint agent by typing this into the chat box.

```
@PowerPoint 
```

Then paste in the below prompt.

```
Using the attached proposal document for Harborview Retail Group, create a single slide that turns the "Our Approach & Methodology" phase table into a visual project roadmap.

Show each phase as a distinct step along a horizontal timeline. For each step, include the phase name, its duration, and a short one-line description, using icons or simple visual elements rather than a text table. Keep wording minimal, this should read as a leadership-ready graphic a partner could put in front of a client, not a wall of text.

Title the slide "Harborview Retail Group: Data Migration & Systems Modernization Roadmap." Use a clean, professional style consistent with an advisory/consulting deck.
```

> A slide is still something you have to click through one at a time, or print out. Let's ask for the same content in a format that lives on its own: a webpage you can click through, right inside the chat. This runs through a feature called Copilot Pages, so keep an eye on whether it renders as something you can actually click rather than just a block of code, that part isn't fully guaranteed every time.

## Step 2: The Interactive Click-Through

_! The preview will only work if your Microsoft Admin has enabled that feature_

```
Using the attached proposal document for Harborview Retail Group, build an interactive web page using only plain HTML, CSS and Javascript that walks through the "Our Approach & Methodology" phases one at a time.

Show one phase per screen: the phase name, its duration, and a short description. Include a "Next" button to move forward through the phases in order, and a "Back" button to return to the previous one. Show a simple progress indicator (for example, "Phase 2 of 6") so it's clear how far through the roadmap the viewer is.

Keep the design clean and professional, consistent with something a partner could click through live in front of a client. Render this as an interactive preview I can click through directly, rather than just showing me the code.
```

> One last jump: instead of just displaying the proposal's numbers, let's build something that lets you play with them. This one leaves Copilot Chat entirely and goes into Power Apps, since something with working logic like this still needs that environment. Notice the prompt doesn't ask for a document at all, it asks for a table and a rule, and Copilot builds the working app around them. If the toggle doesn't update the totals correctly on the first try, that's normal, just ask it to fix the formulas and it usually gets there on the second pass.

## Step 3: The Fee & Scope App

```
Create an app called "Harborview Engagement Fee & Scope Configurator" to help a partner explore fee and timeline scenarios for a proposed engagement.

Create a table called "Engagement Phases" with these records:

Phase Name | Duration (weeks) | Low Fee Estimate | High Fee Estimate | Included
Discovery & Assessment | 3 | 75000 | 90000 | Yes
Design & Planning | 4 | 105000 | 130000 | Yes
Build & Test | 5 | 280000 | 390000 | Yes
Pilot Migration | 2 | 110000 | 155000 | Yes
Full Migration & Cutover | 3 | 170000 | 230000 | Yes
Stabilization & Knowledge Transfer | 2 | 110000 | 155000 | Yes

Build a single screen app where each phase is shown as a row with a toggle for "Included." When a phase is toggled on or off, update three summary values at the top of the screen in real time:

- Total Estimated Duration (sum of Duration in weeks for included
  phases only)
- Total Estimated Fee, Low End (sum of Low Fee Estimate for included
  phases only)
- Total Estimated Fee, High End (sum of High Fee Estimate for included
  phases only)

Format the fee totals as currency and the duration as "X weeks." Keep the design clean and simple, this will be used live by a partner in a client conversation to show how scoping decisions affect fees and timeline.
```
