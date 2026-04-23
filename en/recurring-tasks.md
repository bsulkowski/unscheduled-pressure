# Recurring Tasks — an UP tool

A simple system for tracking activities that need to happen regularly, but on no fixed schedule.

## What it's for

Some tasks don't have deadlines. They just need to happen *roughly* every so often — cleaning the washing machine filter, replacing a toothbrush, checking the fire extinguisher. Easy to forget, hard to schedule precisely, and not worth the mental overhead of putting them in a calendar.

This tool collects them in one place and keeps track of when each one was last done.

## How it works

Maintain a table with three pieces of information for each activity:

- **What** — a short description of the task
- **How often** — a rough frequency, chosen from a set of predefined intervals
- **Last done** — the date it was most recently completed

When the lower bound of the chosen interval has passed since the last completion, the item is gently flagged — not as overdue or failed, but as a nudge: *you wanted to do this roughly this often, and the time has come around again.*

## Frequency intervals

Rather than picking an exact frequency (every 3 weeks? every 28 days?), activities are assigned to one of a small number of intervals. The default set is:

- **a few days**
- **10-20 days**
- **1–2 months**
- **3–4 months**
- **6–8 months**
- **1 year**

The point of intervals — rather than exact values — is to remove a non-decision. Whether something happens every 3 or 4 months is rarely meaningful. The interval captures the intent without demanding false precision.

The default intervals can be adjusted to suit your needs.

## When the nudge appears

A task is flagged once the lower bound of its interval has passed since it was last completed. For a task set to *1–2 months*, the nudge appears after one month. Nothing is flagged early. The signal comes from the configuration you set and the actual passage of time — not from the tool itself.

## Implementation

This tool has no required technology. Use whatever fits your workflow:

- A Trello board with cards and labels
- A spreadsheet (Excel, Google Sheets, Numbers)
- A plain text file or markdown table
- A notebook and pencil

The structure is the method. The medium is up to you.

## UP compatibility

This tool follows the UP principle of reflecting existing pressure without adding its own:

- No enforced rhythm — the tool does not expect regular check-ins
- No punishment for absence — come back after a week away and the data is exactly as you left it
- No false urgency — flagging begins only after the threshold the user has set
- User-owned configuration — frequencies are chosen and freely adjustable by the user
