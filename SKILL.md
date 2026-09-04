---
name: warm-extract
description: Use this after every warm call, one person at a time. The founder says "I talked with [name]", "/warm-extract", pastes a transcript or gives the path to one (.txt, .md, .srt, .vtt), or says "self-interview" when there is nobody to call. It saves the transcript and writes one notes.md per person under squad/clients/ (their words verbatim, the problem, the cost, what they pay now, the idea, the model, the next step), and when a call hands over an offer it writes the draft into squad/business.md and stops for the one number the founder will say. It never sends, never prices, and never asks the founder to organise their notes.
---

# Warm Extract

**Text in, one folder per person out: the call's words saved verbatim, the idea and the model named, and the draft offer written the day a call hands one over.** The founder's part: paste the transcript, and type one number when a call passes the gate.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is read first (founder name, voice sample, `clients`); its values win over the `squad/` paths below, which are worked examples. A row reading "(none yet)" is an unanswered field, not an override.

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 0 THE TEXT | HUMAN INPUT: the transcript, pasted or by path. One question, only when the text never says who the person is. On "self-interview": the script's 8 questions, asked one at a time |
| 1 THE FOLDER | AUTO: `transcript.md` and `notes.md`, one pass |
| 2 THE GATE | AUTO check. Passed: `## THE DRAFT` written, then **STOP · GATE: the founder types the number they will say**. Failed: one line, no stop |

Runs once per person, 1 to 5 people. Never pause beat 1 to ask a small question; never run through the gate.

**No resume.** `notes.md` present means that person is done; a folder without it was never extracted. A transcript a folder already holds is never parsed twice.

## The outputs (4 files at most, every run)

1. `squad/clients/<first-last>/transcript.md`: the text as it arrived, always.
2. `squad/clients/<first-last>/notes.md`: the 7 sections, one pass.
3. `squad/business.md`, `## THE DRAFT`: only when the gate passes.
4. `.claude/squad-roots.md`: the `clients` row, written once.

No scores, no service shapes, no starting point, no sheet cell. Nothing else gets written.

## Step 0 · THE TEXT

**Self-check first.** `references/recording.md` inside this skill's folder, next to `SKILL.md`, must open. If it does not, stop and tell the founder to finish the install: copy the whole skill folder, `references/` included.

Reads: whatever follows the trigger. A paste, or a path to a `.txt`, `.md`, `.srt` or `.vtt` file. The person's name and the call's date come from the text or from the founder's line ("I talked with Jordan on Tuesday"); a date nobody said is today's.

- A recording path (`.m4a`, `.mp3`, `.mp4`) is not read. Answer with one line from `references/recording.md` naming the transcriber for their laptop, and wait. No install, no connector, nothing uploaded.
- The founder's own account from memory is the floor. Take it as it comes, in any order, and label every quote `(founder's recollection · Name · date)`.
- Language is read, never asked. Quotes stay in the language they were said in; the notes and the draft are written in the language of the roots file's voice sample.
- One question, only when nothing says who the person is: "Who was this with?" Never ask the founder to organise anything.

**Self-interview.** Nobody to call is the trigger. Read `squad/warm-script.md` (missing: say to run `/warm-script` first, and stop). Ask its 8 questions one at a time, in the past tense, about who the founder was before they learned what they know now: "What was the hardest part about your work back then?", "Tell me about the last time that happened", and on through the cost, the spend and "Who else had this?". Wait for each answer. Then the exit question: **"Who is standing where you stood, today, that you could reach?"** The chat is the transcript, the folder is `squad/clients/self/`, and every quote is labeled `(self-interview · Name · date)`. A name from the exit question gets its own folder when the real call happens, not before.

## Step 1 · THE FOLDER

Writes `squad/clients/<first-last>/`: the name as the founder says it, lowercased and hyphenated (a first name alone is the folder name; `self` for the self-interview). `transcript.md` holds the text as it arrived. `notes.md` opens with `# Name · what they do · date` and holds these 7 headings, by exact string, in this order, written in one pass:

| Heading | Holds |
|---|---|
| `## QUOTES` | Every line the person said that carries a problem, a cost, a spend, an ask or a next step, verbatim, each labeled `(warm call · Name · date)`. A one-line gloss under a quote in another language. A paraphrase is never saved as a quote |
| `## THE PROBLEM` | One line per problem, 3 at most, each pointing at the quote that carries it |
| `## THE COST` | A number the text supports (money or hours, and how often), or the question that would get it |
| `## WHAT THEY PAY NOW` | A fact line ("$400 a month on a VA"), or "unknown". Never a price |
| `## THE IDEA` | One line: what the founder would deliver to this person for this problem |
| `## THE MODEL` | One line: agency, consulting or software, and why in 6 words |
| `## THE NEXT STEP` | The date they agreed to, or "none" |

Then add the `clients` row (`squad/clients/`) to `.claude/squad-roots.md` when it is not there yet.

Says: **Saved: `squad/clients/<first-last>/notes.md`**, then the 7 sections as written. One closing line: copy the strongest quote into the Outreach Sheet's column 5 by hand.

## Step 2 · THE GATE

Two things, both read off the text: **a named person asked for a named thing**, and **the next step has a date**. "I would totally pay for that" with no date fails. "Send me something" with no date fails.

Both true, on a recorded transcript: write `## THE DRAFT` into `squad/business.md`.

| Line | Holds |
|---|---|
| who | the person and what they do |
| the problem | in their words, the quote |
| the deliverable | the named thing they asked for |
| what they pay now | the fact line from `notes.md`, or "unknown" |
| price | `unpriced`, or "the price they said: $X" when they volunteered one, never the offer's price |
| the model | agency, consulting or software |
| the next step | the date |
| the quotes | the 3 strongest, labeled |

Then STOP on one line: **"G6 needs a number. The first rung is the $997 pilot (G5, Quick explain). Type the number you will say, or open G5 first."** Write the number they typed into the price line, and say: open G6 and sell it to this person.

A `squad/business.md` already stamped `confirmed <date>` is not touched: say the offer is confirmed and this person goes to G6 on it. An earlier `## THE DRAFT` for a different person is shown, and replaced on the founder's yes.

Either part false, or a recollection or self folder: write nothing to `business.md`. Say which part is missing in one line, how many folders exist (1 to 5), and that G5 forges the offer from the folders.

## Rules

- Never send anything.
- Never price anything. The founder types the one number at the gate; no other number is ever written as a price.
- Never invent a number, a name or a need. A cost the text does not support is a question; a need nobody said stays out.
- Never paraphrase a quote, and never save a paraphrase as one. Verbatim, labeled, dated.
- Never ask the founder to organise their notes. Messy is the format.
- Every message is scannable: a short header, then bullets or a table.
