# The Outreach Sheet, the Warm tab

Serves step 0 (connect it, read it), step 1 (the names already in it), step 2 (the paste
block that puts new rows in it), step 3 (the Next touch dates the morning reads) and step 4
(the two cells a booked meeting changes).

The sheet the founder copies in G3 lives at
`https://docs.google.com/spreadsheets/d/11m-EFAMSuovafeCQmiypa-oUey2VtO5s-5P4u0oAqjA/copy`.

It carries four tabs: START HERE, Warm, Cold and Weekly. Every row from this skill lands in
the Warm tab.

This file is the checked-in copy of the Warm tab's schema. The skill, the lesson and every
skill downstream (the winning offer, the 90 day plan) name these columns; when the sheet
changes, this file changes with it in the same edit, and anything that disagrees with this
file is the thing that is wrong.

Column order is load-bearing: the step 2 paste block is tab separated and positional, so a
reordered sheet lands data in the wrong cells.

| # | Column | Filled by | What goes in it |
|---|---|---|---|
| 1 | Who they are | the squad | The person |
| 2 | How you know them | the squad (grey on the sheet) | The relationship, then what they do now, in the founder's words |
| 3 | First message sent | the squad drafts, the founder dates | The drafted first message; the date goes in when it actually goes out |
| 4 | Reply | the founder | What came back, and when |
| 5 | What they said on the call | the founder, after the call | A real quote. Empty until they say it |
| 6 | Status | the founder | LISTED · SENT · TALKING · DEMO SENT · CLOSED · NOT NOW, one way only |
| 7 | Next touch | the founder (blue on the sheet) | The date the next follow-up is owed |

Follow-ups get drafted on the morning they are due, never stored on the sheet; Next
touch holds only the date one is owed.

To the right of column 7 the sheet carries THE COUNT: contacted, replies, follow-ups due,
closed. It is computed off the rows. Nothing writes into it by hand.

## Row one, the example row that ships in the sheet

It sits inside the counted range, so THE COUNT reads it like any other row. The lesson has
the founder read it for the shape and then delete it before the first real row lands.

| Column | Value |
|---|---|
| Who they are | (example) Jordan Park |
| How you know them | Old coworker, design team 2023. Runs a small detailing shop with his brother |
| First message sent | Aug 31, voice note asking how the shop is running. No pitch |
| Reply | Sep 1, long reply, complained about no-shows |
| What they said on the call | "People text me at eleven at night and I lose half of them by morning" |
| Status | TALKING |
| Next touch | Sep 4, send the demo with his name on it |

## Who reads it, who writes it

**The squad reads this sheet and never writes into it.** Reading is what step 0 connects:
Google Drive finds the file by name, and a Google Sheets connector, where the founder's app
offers one, is what opens a named tab like Warm. Writing stays the founder's hand, because a
dashboard somebody else filled is one they stop opening.

What a read pulls, every time: every row that is not at LISTED or CLOSED, columns 1, 3, 4
and 6, Who they are, First message sent, Reply and Status. Column 1 is what ties a row to a
person, and the date in column 3 is what says which follow-up is owed today, so neither can
be dropped. Column 5 outranks every other column the moment it has anything in it, because
it is the only cell on the sheet carrying the buyer's own words.

**Unconnected, the founder pastes instead**, header row included, all seven columns, and
every beat treats a pasted row exactly the way it treats a connector's row. The paste is
positional: a row pasted without column 1 cannot be tied to a person and gets asked for
again.

The squad's own copy of the list is `squad/warm-list.md`, and that copy, not this sheet, is
what every later skill reads.
