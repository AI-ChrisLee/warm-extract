# Warm Extract: install in 60 seconds

The first part of an Execution Squad, and the one that ends "I do not know anyone." It runs
your whole warm week: it turns the names already in your phone into one ranked list, writes
the honest twenty-minute ask for each one so a meeting gets booked today, drafts every
follow-up on the morning it comes due, and after each call it pulls that person's own words
into `squad/draft-offer.md`, the first draft of your offer. Twenty minutes a day, all week.

## What to bring

Your copy of the Outreach Sheet from the lesson, and five names. That is the whole intake.
The five are the four minute test: real people you could text tonight, first names, no
research. If you stall on the fifth, the one you are slightly embarrassed to write is the
right one, because embarrassment means the relationship is real. Nothing to prepare, nothing
to clean up. Phone and email exports are optional and only get mined if your list runs short.

## Run it

Open Claude Code in your business folder and say: **"Build my warm list."** (Downloaded this
folder on its own? Drop the whole thing into `.claude/skills/`, then quit and reopen Claude
Code.)

After that, four sentences run the week:

- **"Who is due today"** every morning. It reads the dates and drafts the follow-ups that are
  owed, honest and specific, never "just checking in."
- **"[Name] said yes, Thursday 2pm"** the moment somebody answers. The meeting lands on the row.
- **"I talked with [name]"** and then dump the call, messy: fragments, lowercase, no order. That
  is the format. Do not clean it up.
- **"Build that"** when a call gives you something obvious to show. One slice, built the same day,
  their name on it.

Stopped halfway, or closed the laptop? Say **"continue Warm Extract"** in a new window. It
reads what is on disk and picks up at the first thing missing.

## The sheet connector, and what paste mode costs you

The Outreach Sheet lives in your own Google Drive, and connecting it is clicks, not config:
Settings in the Claude desktop app, the Connectors list, Connect on Google Drive. Connect the
Google Sheets connector too if your app lists one, since that is the one that opens a named tab
like Warm. Connected, the run reads your rows itself and hands you cells to paste back.

Not connected, and the run still goes: you paste the Warm tab instead, header row included, all
seven columns, every time it needs to look. It costs you that paste on every beat and nothing
else. The run tells you which mode you are in before you spend anything on it. There is no MCP
server to wire here; the sheet is a desktop connector, which is why this folder ships no
`mcp.json.example`.

## What you get

One ranked list at `squad/warm-list.md` with an ask drafted under every warm name, your buyers'
own sentences saved verbatim at `squad/warm-notes.md`, and `squad/draft-offer.md`, one block per
call: their problem in their words, two or three service ideas scored, and one of them named as
where you start. And a meeting on the calendar today, which is the thing the week is graded on.

It never sends anything and it never prices anything. Every message goes out by your hand, and
the first number gets decided in the next part.

## What comes next

The part that reads these calls and forges them into one offer document with one answer on it. It
arrives one episode at a time. Subscribe (the link under every episode) and each new part lands
in your inbox the day its episode goes live.
