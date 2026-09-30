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
