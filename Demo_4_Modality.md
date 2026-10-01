# From Proposal to Interactive Experience

**THIS IS A DEMONSTRATION BY THE INSTRUCTOR AND NOT MEANT AS A FOLLOW-ALONG, YOU MAY NOT HAVE SOME OF THESE FEATURES ENABLED IN YOUR COPILOT ENVIRONMENT**

_This prompt turns the same written proposal into three different formats: a visual roadmap slide, a clickable web walkthrough, and a working app you can use live with a client._

> Lets turn a proposal you've already worked with into something visual instead. Attach the Harborview proposal and ask for a slide instead of a paragraph, and notice how much of the table's structure (the phases, the durations) survives the jump into something a client could actually look at.

## Step 1: The Visual Roadmap

Begin by creating a new blank presentation in PowerPoint and then selecting Copilot.

Then paste in the below prompt.

Attach: [Proposal_Harborview_Data_Migration](https://github.com/roitraining/ai-masterclass/blob/main/assets/Proposal_Harborview_Data_Migration.docx)
Attach: [Slide Template]()

```
Create one 16:9 PowerPoint slide using the attached example image as the exact design template and the attached proposal as the only content source.

Use content only from "Our Approach & Methodology” Do not add or infer any information. Match the example’s layout, colours, typography, spacing, shapes, icons, footer, and one-line text formatting. Replace the example content while preserving its visual structure. Add the proposal source to the speaker notes.

You may modify the bar length and colours to match the content needed.
```

> A slide is still something you have to click through one at a time, or print out. Let's ask for the same content in a format that lives on its own: a webpage you can click through, right inside the chat. This runs through a feature called Copilot Pages, so keep an eye on whether it renders as something you can actually click rather than just a block of code, that part isn't fully guaranteed every time.

## Step 2: The Interactive Click-Through

_! The preview will only work if your Microsoft Admin has enabled that feature_

```
Using the attached proposal document for Harborview Retail Group, build an interactive web page using only plain HTML, CSS and Javascript that walks through the "Our Approach & Methodology" phases one at a time.

Show one phase per screen: the phase name, its duration, and a short description. Include a "Next" button to move forward through the phases in order, and a "Back" button to return to the previous one. Show a simple progress indicator (for example, "Phase 2 of 6") so it's clear how far through the roadmap the viewer is.

Keep the design clean and professional, consistent with something a partner could click through live in front of a client. Render this as an interactive preview I can click through directly, rather than just showing me the code.
```
