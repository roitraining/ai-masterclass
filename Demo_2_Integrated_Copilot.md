# Reframing a Proposal Section and Verifying the Changes

_This prompt has Copilot reframe sections of a proposal inside Word, then shows three ways to check what it changed: asking Copilot itself, Track Changes, and Version History._

> Copilot is fast at rewriting. You select a paragraph, run a prompt, and a nicer-sounding paragraph appears. The hard part isn't getting the rewrite, it's knowing what the rewrite actually did. So let's start the way most people do: no safety nets, just ask and accept. The only setup is saving the document first, so there's a copy of the original to come back to later.

## Step 1: The Edit Nobody Can See

[Proposal_Harborview_Data_Migration](https://github.com/roitraining/ai-masterclass/blob/main/assets/Proposal_Harborview_Data_Migration.docx)

_! Version History only works on files saved to OneDrive or SharePoint with AutoSave turned on, so upload the document there first if you opened it from your desktop._

Open the proposal in Word, make sure Track Changes is off, and save the document (`Ctrl+S`). Then select the Executive Summary paragraph, open the Copilot chat pane, and paste in the below prompt.

```
Rewrite the selected Executive Summary so that it leads with the business outcomes Harborview will get, such as minimal disruption and internal capability, before mentioning the technical transition from legacy systems. Keep it to four sentences or fewer and do not add any new claims.
```

> Take a look at what came back. It reads well, but what actually changed? There's no markup, so the only way to know is to hold the old version in your head and compare, and nobody does that. Did it keep "without unplanned service disruption"? Did it add anything? You don't know, and neither does anyone else who opens this document later.
>
> Let's fix the visibility problem. Turn on Track Changes, and this time we'll also be more specific about what we want. Pay attention to the last line of the prompt, because it's there for a reason.

## Step 2: Turning On Track Changes and Getting Specific

Turn on Track Changes (**Review > Track Changes**), select the "Our standard approach" paragraph under the phase table, and paste in the below prompt.

```
Rewrite the selected paragraph for a non-technical executive audience, such as Harborview's CFO or COO, who cares about business risk and disruption rather than migration terminology.

Replace jargon such as "wave-based" and "big-bang cutover" with plain business language. Keep it to three sentences or fewer. Do not add new claims, and do not change any commitments, facts, or numbers.
```

> Much better, and now there's a record. But look closely at how Word shows it. Track Changes doesn't mark the individual words that changed, it tends to strike through the whole sentence or paragraph and show the new one in its place. So you're still reading both versions with your eyes to figure out what's different. On a three-sentence paragraph that's fine. On a forty-page proposal with dozens of edited paragraphs, it isn't.
>
> This is where Copilot can earn its name as a collaborator. You've already asked it to do the writing, so ask it to help with the checking too. One caveat: it's grading its own homework here, so treat what it gives back as a starting point and not the final answer.

## Step 3: Asking Copilot to Audit Its Own Edit

```
Compare the tracked changes in the "Our standard approach" paragraph. In a table, list the original wording, the new wording, and whether the meaning is unchanged, softened, strengthened, or lost. Flag anything in the new version that was not in the original, such as words like "eliminate," "guarantee," or "seamless."
```

> That table is useful, especially for spotting a commitment that got quietly softened, like "rollback criteria in every wave" becoming "safeguards." But if we don't fully trust Copilot to grade its own changes, and Track Changes isn't detailed enough on its own, we need a check that doesn't depend on either one.
>
> That's Version History. It has been saving versions in the background this whole time, including the Executive Summary edit from Step 1 that had no markup at all. Notice the pattern across all four steps: Copilot does the drafting and helps with the review, but you're the one who sets the guardrails, turns on the tools that keep a record, and makes the final call. That's what a co-pilot is supposed to be.

## Step 4: Checking Version History

Go to **File > Info > Version History** (or click the file name in the title bar), open the version you saved at the start of Step 1, and choose **Compare** to see a marked-up comparison against the current document. Scroll through it and you can see exactly which words changed in both paragraphs, including the Executive Summary edit that was never tracked. Anything that doesn't hold up, you can fix by hand or use **Restore** to go back to the original version.
