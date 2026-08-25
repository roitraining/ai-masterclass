# Client Meeting Prep Brief

_This prompt prepares a one-page brief for a client meeting by summarizing news, organizing past notes, and analyzing stakeholder profiles._

> You've probably typed something exactly like this before: quick, to the point, gets it over with. Try it, and take a look at what comes back. It reads fine, but it's generic. It could be about almost any client, because there's nothing in the prompt that's actually about this meeting. That's the real issue: not that the AI did a bad job, just that we haven't given it anything to work with yet.

## Step 1: The Generic First Try

```
Write me a brief for my meeting with Starbucks.
```

> Here's something most of us are guilty of: months of meeting notes in half-sentences, abbreviations, question marks everywhere. Before asking AI to write anything client-facing, it's worth having it clean up your own notes first.
> 
> Paste these in along with the instructions below, and notice what we're telling it: flag anything uncertain instead of guessing at what we meant. That one line is doing a lot of work. Without it, the AI might just smooth over the question marks and hand you back something that sounds confident but isn't actually accurate.

## Step 2: Cleaning Up Old Notes

[Past Meeting Notes](https://github.com/roitraining/ai-masterclass/blob/main/assets/Past_Meeting_Notes.docx)

```
I'm going to attache raw, unstructured meeting notes covering several past interactions with a client contact. Reorganize them into a clean summary using these headers: Date/Occasion, Topic Discussed, Client Concerns Raised, Commitments We Made, Open Action Items.

Keep every distinct fact. Don't drop anything. Don't add anything that isn't in the notes. If something in the notes is itself uncertain (marked with a question mark or "I think"), flag it as uncertain rather than resolving it yourself.
```

> Now let's bring in some real information. This part isn't fictional: you're asking the AI to go find actual, current news about a real company. Make sure you ask for sources along with the headlines, because that's what we're going to dig into over the next few steps.

## Step 3: Researching Real News

```
Use the Internet and find recent news from the last 30 days about Starbucks that would be relevant to an advisory conversation with their leadership team. For each item give me: the headline, a one-sentence summary, the source name, and a link. Prioritize primary sources (company statements, named reporters at established outlets) over aggregators.
```

> Just because a claim has a source attached to it doesn't mean the claim is right or the source is relevant. You always need to verify it yourself. One more thing worth checking: when was this actually published? AI search can surface an older article in a way that makes it feel brand new. Quick date check before you call anything "recent."
> Now try pulling in some context from a client contact's LinkedIn. Paste in a profile link and ask for a summary, then just watch what happens. Chances are, it won't work. LinkedIn doesn't let AI tools access profiles without permission, so this isn't the AI letting you down; it's a wall LinkedIn put up on purpose.

## Step 4: The LinkedIn Wall

```
I am give you a LinkedIn profile. Summarize this person's background and recent activity so I can reference it in our meeting.

LinkedIn profile: https://www.linkedin.com/in/anthony-sok/
```

> So if it can't go get the page itself, just show it the page instead. A screenshot works because the AI can read images directly, no fetching required. 

## Step 5: Prompt (with the screenshot attached)

```
I've attached a screenshot of a LinkedIn profile. Summarize this person's professional background and tenure, note anything relevant from their recent activity, and suggest one talking point I could use to open our meeting.
```

> Okay, now we bring it all together. The cleaned-up notes, the verified news, the LinkedIn context, all into one brief. Pay attention to the last line of the prompt: "if something isn't covered here, say so instead of guessing." That single sentence is doing more work than it looks like. You'll see exactly why in a second.

## Step 6: Putting It All Together

```
You are a senior advisory partner preparing for a client meeting in two hours. Using only the information provided below, produce a one-page meeting prep brief with these sections:

1. Recent Developments (from the verified news)
2. Relationship Context (from the cleaned meeting notes)
3. Stakeholder Notes (from the LinkedIn context)
4. Likely Priorities
5. Three Opening Questions
6. One Point of View We Can Lead With

Keep it to one page. Professional but conversational tone. If something relevant isn't covered in the material referenced, say so explicitly rather than inferring or guessing.
```
