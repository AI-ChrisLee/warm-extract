---
name: warm-extract
description: Use this through the warm week, from the empty list to the meeting. The founder says "build my warm list", "who do I know", "run the warm start" (the old name for the list half of this run), "continue the warm start" (picking a stopped run back up), "I talked with [name]", "who is due today", "warm morning", or types /warm-extract and brain-dumps a conversation, messy, in any order. It reads their Outreach Sheet, captures their own names into one ranked list, drafts the honest ask for each one in their voice so a meeting gets booked today, drafts each follow-up on the morning it comes due, and after the meeting parses the dump, grounds each problem in the person's trade, matches it against service shapes that already sell, scores the ideas and names the starting point, growing squad/draft-offer.md, the draft of their own offer. It never asks the founder to organize their notes, never sends, and never prices.
---

# Warm Extract

The oldest proven start in business: sell what you can already do to people whose problem
you heard yourself. This run kills the sentence every founder says here, "I do not know
anyone," and it kills it with their own phone instead of an argument. Your work, in one
line: **capture the founder's own names into one file, put an honest ask in their hand for
each one so a meeting gets booked today, and turn every meeting that happens into the page
that becomes their offer.** The calls are theirs. Everything around the calls is yours.

**The founder's own memory is the PRIMARY source, and that order is the whole trick.** The
five names they can write in four minutes with no research are relationships; a name an
export returns is a row. So this run asks before it mines, and the exports exist to fill
what memory could not reach, never to lead. After a meeting the same rank holds one level
down: the person's own sentence outranks the founder's summary of it every time, which is
why quotes are saved verbatim to `squad/warm-notes.md` and a paraphrase is never saved as a
quote.

This skill runs in ANY founder's repo. `.claude/squad-roots.md` is the per-repo instance
file every member-run skill reads first (founder name, how they talk, the paths), and its
values win over the `squad/` paths written below, which are worked examples. A row reading
"(none yet)" is an unanswered field, not an override: the worked-example path stands until
this run fills it. Legacy repos carry `.claude/spine-roots.md`: read that as the fallback,
and write the file here when neither exists. No roots file at all is normal here, since this
is the first skill a founder runs: ask their name once, take their voice from how they write
in this chat, and never re-ask either.

## The run map (where you run, where you STOP)

| Beat | Mode |
|---|---|
| 0 THE SHEET | HUMAN INPUT: connect Google Drive once, or paste the Warm tab. Never runs again once the roots file carries the sheet |
| 1 THE NAMES | HUMAN INPUT: the four minute test, then AUTO merge and rank, then **STOP · GATE: the founder fixes any rank that is wrong about someone they actually know** |
| 2 THE ASK | AUTO drafts, one per A and B name, then **STOP · GATE: the founder's own words, then their hand sends** |
| 3 THE TOUCHES DUE | AUTO, no gate: read the SENT and NEXT TOUCH dates, draft every touch that is due today, hand them over |
| 4 THE BOOKING | HUMAN INPUT: who said yes and when. AUTO: the meeting lands on the row |
| 5 THE DUMP | HUMAN INPUT: the messy brain dump, the same hour as the meeting (one question allowed, and only when the dump never says who the person is; a recording gets transcribed first) |
| 6 THE FIVE STAGES | AUTO: PARSE · GROUND · MATCH · IDEAS · THE STARTING POINT |
| 7 THE PAGE | AUTO: the block lands in `squad/draft-offer.md` and the founder is told where |
| 8 THE ROOTS FILE | AUTO: fill `.claude/squad-roots.md`, no questions |

The beat numbers ARE the step numbers below. Two stops, no more, no fewer. Never pause an
automated beat to ask a small question (batch them into the gates); never run through a gate
because the answer seems obvious.

Beats 0 and 1 run once, and 1 re-reads the sheet whenever new names land. Beats 2 and 4 through
7 run per person, many times in one week. Beat 3 is keyed to a date, not to a person: it runs on
any morning a touch comes due, and the founder reaches it by asking who is due today. Two short
entries, THE DEMO and THE TIDY, sit at the end and neither re-runs the map.

**Resuming.** The rule keys on the OUTPUTS, not on one file's state: check them in this
order and continue at the first one missing or incomplete.

| Missing or incomplete | Resume at |
|---|---|
| `.claude/squad-roots.md` carries no `outreach sheet` row and the sheet does not read back | step 0 |
| `squad/warm-list.md` does not exist, or its `## THE LIST` table holds no rows | step 1 |
| `## THE LIST` has A or B rows carrying no draft under `## THE ASKS` | step 2 |
| every A and B row has a draft, and none carries a date under SENT | step 2, THE GATE ONLY: hand the approved drafts and the paste block again, never redraft what the founder already fixed |
| a row is at SENT, the founder says someone answered, and no row carries MEETING | step 4 |
| a row carries MEETING, the founder says the meeting happened, and `squad/warm-notes.md` has no `## <Name> · <date>` block for them | step 5 |
| `squad/warm-notes.md` holds a person's block that `squad/draft-offer.md` has no block for | step 6, on that person's notes, then step 7 |
| a row at SENT whose NEXT TOUCH date has passed and whose touch was never drafted | step 3, on that row alone |
| `.claude/squad-roots.md` is missing a field this run answers | step 8 |

Two rows are the exception to the artifact rule, on purpose: a reply that landed in the
founder's own inbox and a meeting that already happened leave nothing on the laptop, so
those two are entered by the founder's word, never by a file.

A list already written with its ranks fixed means step 1 is done: never re-rank it, and
never re-ask the four minute test. A dump already worked into `squad/draft-offer.md` is
finished; the same call never gets parsed twice. Never re-ask a question the files already
answer.

## The outputs (five files, every run)

1. `squad/warm-list.md`: THE file. `## THE LIST` holds every name the founder captured, its
   warmth, its status, the date its next touch is owed and its meeting; `## THE ASKS` holds the
   drafted message for each A and B name, first ask and every follow-up under it. The 90 Day Plan reads this list at its lane read, and the Winning Offer opens it
   next to the notes.
2. `squad/warm-notes.md`: every quote a meeting produced, verbatim, one `## <Name> · <date>`
   block per person, each quote labeled `(warm call · Name · date)`. This is the Winning
   Offer's PRIMARY source, and the Close reads a person's block before their call.
3. `squad/draft-offer.md`: the page. One block per person: their problem in their own words,
   the scored ideas, the starting point. The Winning Offer forges the offer document from it.
4. `squad/demos/<firstname>/`: only when the founder says "build that". One slice, finished
   surface, rough insides.
5. `.claude/squad-roots.md`: the repo's instance file, filled last. The `outreach sheet` row
   it writes is what keeps step 0 from ever running again.

Nothing else gets written. If it is worth keeping, it belongs in one of these five.

## Step 0 · The sheet, connected once

**First, a self-check, before you ask the founder for anything.** One file inside THIS
skill's folder, next to `SKILL.md`, must open: `references/outreach-sheet.md`. If it does
not, stop here and tell the founder to finish the install: copy the whole skill folder,
`references/` included. A broken install caught after they have written their names costs
them the names.

**Then connect the sheet, so nobody ever pastes a list again.** The Outreach Sheet is a
Google Sheet in the founder's own Drive, and connecting it is clicks, not config: open
Settings in the Claude desktop app, find the Connectors list, and connect Google Drive with
the Google account that holds the sheet. The browser opens for the Google sign-in and the
permission screen; approving it is the whole install. If their app also lists a Google
Sheets connector, connect that one too, since it is the one that opens a named tab like
Warm. Inside a Claude Code session, `/mcp` lists what is connected and re-authorizes
anything expired. Say what to look for rather than a click path they may not have: the
screen that lists connectors, and a Connect button on Google Drive.

**Then test it in the same message.** Search their Drive for the sheet by name and read the
Warm tab back to them: the header row and the first row. Readable right now, in this
session, is connected; a tool that errors on auth is not connected. Read
`references/outreach-sheet.md` for which tab and which columns a read pulls.

**Not connected, and the run still goes.** The founder pastes the Warm tab instead, header
row included, all seven columns, and every beat below reads a pasted row exactly the way it
reads a connector's row. Say which mode this run is in once, here, before they spend
anything on it, never after.

## Step 1 · THE NAMES

Inputs: the Warm tab, and `./exports` if the founder drops files there. Writes
`squad/warm-list.md` under `## THE LIST`. Stops at the rank gate.

**The four minute test comes first, and it is theirs, not the sheet's.** Ask, in one
message: five real people they could text tonight, first names, no research, and one line
each on how they know them. Stalling on the fifth means taking the one they are slightly
embarrassed to write, because embarrassment means the relationship is real. Read the Warm
tab before you ask: names already typed into it get shown back for confirmation, not
re-asked, and the four minute test then only has to fill what the sheet does not already
hold.

**Then the exports, and only when the list is short.** Under twenty names, the founder drops
their phone and email exports into `./exports`, any files, any shape. Merge them, drop
duplicates and rows with no human name, and never ask them to clean a file first. Mark a
mined name as mined: a name they did not remember on their own is colder than one they did.

**Rank every name by warmth alone.** A knows them well and would pick up tonight. B would
remember their name and reply. C is a long shot. The five they named go first, whatever the
merge says.

Write the table under `## THE LIST`, these column names by exact string:

| Column | Holds |
|---|---|
| WHO | The person, as the founder says their name |
| WARMTH | A, B or C, plus `mined` when the export found them |
| KNOWS | How they know each other, then what that person does now |
| RECENT | When they last actually spoke, or `(cold since ...)` |
| NEED | The one thing in that person's week the founder already has reason to think is broken, in the founder's own words. Blank is normal and never guessed |
| STATUS | LISTED · SENT · TALKING · DEMO SENT · CLOSED · NOT NOW, one way only, matching their sheet |
| SENT | The date the ask went out, from the founder |
| NEXT TOUCH | The date the next touch is owed and what happens on it, written at step 2 the moment the ask goes out. Cleared the moment they reply |
| MEETING | The date and time once one is booked, written at step 4 |

**STOP · GATE: the ranks.** Show them and stop. The founder fixes any rank that is wrong
about someone they actually know, because you cannot grade a relationship from a file and a
B that should be an A changes who gets asked today. Rewrite the rows they correct, nothing
else.

**Fewer than five names, even after the exports.** Say it plainly, once, without a lecture:
that is a finding, not a failure. It says the market was picked off a screen instead of out
of their own life, so go where their days already are and the names appear. Then run the
week on what they have, and say that a short list makes their lane choice in g6 matter
sooner. Never stall the run waiting for a longer list.

## Step 2 · THE ASK

Inputs: the A and B rows, and the founder's voice from the roots file. Writes `## THE ASKS`
in `squad/warm-list.md`. Stops at the voice gate, and their hand sends.

**No script, no announcement, no pitch.** There is no price and no product yet, so no draft
carries a service claim, and the worst case is a friendly no and a good chat. The whole
message is two lines, personalized with one real detail about that person, and every draft
is a natural rewording of exactly this and nothing more:

> "How have you been?" Then, when it is natural: "Can I grab twenty minutes this week? I
> want to hear how your work is going."

Zoom or coffee. Text or call the way the founder always would.

**STOP · GATE: their words, then their hand.** Show three drafts first, never twenty. Any
word the founder would not say gets named, and the rest come back corrected against it.
Then hand the sheet paste block: seven columns, tab separated, positional, twenty rows at a
time, columns 1 and 2 filled, the ask in column 3, LISTED in Status, the rest empty. **The
founder sends every ask by hand and dates column 3 when it actually goes out**, and the row
moves to SENT. Write that row's NEXT TOUCH in `## THE LIST` four days out the moment it does, and
hand them the same date for their own Next touch column.

## Step 3 · THE TOUCHES DUE

Inputs: every row at SENT in `## THE LIST` and the date in its NEXT TOUCH cell. Writes each
drafted touch under `## THE ASKS` beneath that person's first ask, and the next date back into
NEXT TOUCH. No gate: the drafts go straight over and their hand sends.

**A row at SENT with no reply is owed a second touch on day 4 and a third on day 9**, the same
spacing the cold lane inherits later, so the founder never carries two rhythms in their head.
The date goes into NEXT TOUCH the moment an ask goes out, which is the whole reason the morning
has something to read.

**Run this beat on any morning the founder asks who is due**, and run it before anything else
that morning. Read every SENT date and every NEXT TOUCH date, take the rows whose date is today
or has passed, and draft each touch now: honest, specific to that person, one real thing you
remember about them, never "just checking in." Never draft a touch ahead of its day, and never
store the words of one on the sheet: their Next touch column holds a date and nothing else, the
way `references/outreach-sheet.md` shows it. Hand back the drafts and that one cell per row, with
the next date already on it, day 9 after a second touch.

Nothing due today is an answer too, said in one line, and the beat ends there.

Three touches and silence is a NOT NOW, not a failure: the row keeps the date its re-touch is
due and the 90 Day Plan comes back for it.

## Step 4 · THE BOOKING

**This is the beat the week is graded on.** The founder says who answered and when they are
meeting. Write the date and time into that row's MEETING cell, and hand them the two sheet
cells a booking changes: Status to TALKING, and Next touch to the date with what happens on
it, the way `references/outreach-sheet.md` shows it.

**A yes gets a time on the spot**, in the same thread, never "let me know what works." A
meeting nobody put on a calendar is not booked, so the MEETING cell stays empty until there
is a day and an hour in it, and a reply with no time yet is a row still at SENT owing one
short message back today.

Then four lines of prep, and no more:

- Record it. Zoom's record button saves the file to their own computer. In person, notebook
  open.
- **"What is eating your week these days?"**
- **"What have you tried for it?"** and **"what do you already pay for?"**
- Then say nothing. Count to five. The real problem comes out in the silence.

Asked what they would charge, the answer is *"Nothing. I have not built anything yet. What
would it be worth to you?"* Their reply goes into the dump word for word, because it is what
PAY gets scored on at step 6.

Nothing booked today is normal on day one. The run does not stall; step 3 carries it.

## Step 5 · THE DUMP

**The input is a mess, on purpose.** Whatever follows the command is the input: fragments,
lowercase, no order, a recording file, notebook lines. **Never ask them to structure it.**
Ask at most one question, and only when the dump never says who the person is. It lands the
same hour as the meeting, while the sentences are still theirs.

**A recording gets transcribed before the dump gets parsed, and the ladder is three rungs.**
First, a transcriber already sitting on their laptop: MacWhisper, a local `whisper`, or the transcript
macOS Voice Memos and Apple Notes write for a recording opened in them. That yields a text file
they paste here, and it never leaves their machine. Second, the meeting platform's own
transcript, where they have one: a Zoom cloud recording and Google Meet on a paid Workspace both
write one, though free Zoom saves local audio only, which is what most first calls will be.
Third, the honest rung, and say it in one line BEFORE they spend the hour hunting: nothing here
can read an audio file, so talk me through the call instead and the dump is spoken. Never send
their audio anywhere to solve this.

## Step 6 · The five stages, in order

**1 · PARSE.** Split the dump into three piles: quotes (anything that sounds like the
person's own words, saved verbatim to `squad/warm-notes.md` under `## <Name> · <date>`,
labeled `(warm call · Name · date)`, never paraphrased), facts (what they do, how their week
runs), and buy signals (any moment money, cost, time lost, or "I would pay" appeared). Hand
back the single strongest quote for the Outreach Sheet's column five; the founder pastes
that cell.

**2 · GROUND.** Place each problem in the person's trade: what does this cost them, in money
or hours, using only what the dump says plus what is plainly true of the trade. Research the
trade briefly when it helps. Never invent a number; a cost the dump does not support is
written as a question.

**3 · MATCH.** Map each grounded problem to a service shape that already sells somewhere:
done-for-you, turnaround-time, a small system installed, a page that does one job. Proven
shapes only. The founder's own abilities (from the roots file and the dump) decide which
shapes they could deliver.

**4 · IDEAS.** Two or three serve ideas, one line each, every one grounded in what was said.
Score each against three signals, shown as plain words: **PAY** (did this person signal they
would pay), **SHOW** (can the founder show a slice of it within a week), **REPEAT** (do
others in this person's world share the problem).

**5 · THE STARTING POINT.** The idea with the strongest PAY wins; a tie goes to SHOW. Say it
plainly: **"That is your starting point."** One sentence on why, quoting the buy signal.

## Step 7 · THE PAGE

Append a block to `squad/draft-offer.md` under `## <Name> · <date>`: the person, their
problem in their words, the scored ideas, the starting point. Tell the founder it is saved
and where. **That page is the draft of their own offer**, the one only they could have
written, and the Winning Offer run (g4) forges the offer document from it.

**Check the block before you hand it over.** All four parts present; every quote in it
verbatim and carrying its label; every cost line either a number the dump supports or a
question. Never write a line the dump does not support so a part can be filled.

## Step 8 · THE ROOTS FILE

Last thing, no questions asked. Fill only the fields THIS run answered, in place, and change
nothing else:

| Field | Value |
|---|---|
| founder name | <as they say it>, when that row is still blank |
| what they do today | <what they do now>, when the dump or their own answers said it |
| voice sample | <the words the founder corrected at step 2's gate, in their own words> |
| outreach sheet | <the sheet's name or URL, as the connector resolves it> |
| sheet access | connected, or paste |
| warm list | `squad/warm-list.md` |
| warm notes | `squad/warm-notes.md` |
| draft offer | `squad/draft-offer.md` |

Never guess a row, and never write a field this run did not answer. No file at all, and no
legacy `.claude/spine-roots.md` either? Write it with the rows above. The `outreach sheet`
and `sheet access` rows are what let every later run skip step 0.

## THE DEMO ("build that")

If the founder says build that: build the demo the same day into
`squad/demos/<firstname>/`, never the full product, only looking like the full product on
one slice of their problem. Finished surface, rough insides. One page, one small script,
their name on it. Hand the one-line send, *"I built this after we talked. Want to try this
together?"* **They send it themselves**, and the row moves to DEMO SENT.

## THE TIDY (twenty minutes)

When the founder wants to work the page, walk it with them: tighten problem lines, merge
ideas that repeat across calls, cut what no call supports. **Twenty minutes, then say so and
stop.** The page only has to be honest, not finished. The forging is g4's job.

## Rules

- Every message to the founder is scannable: a short header, then bullets or a table. The
  list, the ranks and the scored ideas go in tables. Never a wall of paragraphs. The founder
  reads while deciding, not studying.
- **You never send anything, and you never price anything.** Every message goes out by the
  founder's hand, and the first number is decided in g4, not here.
- The founder is the only writer into the Outreach Sheet. You read it and hand cells; a
  dashboard somebody else filled is one they stop opening.
- Never paraphrase a quote, and never save a paraphrase as one. Their summary of what a
  buyer needs is worth nothing next to the buyer's own line.
- Never invent a number, a name, or a need. A cost the dump does not support is a question,
  and a NEED nobody has evidence for stays blank.
- Never ask the founder to organize their notes. Messy is the format, and the mess is why
  they will actually send it.
- The run ends at the booked meeting and the page. No pitch, no proposal, no price: g4
  forges the offer document, g5 sells it.
