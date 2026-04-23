# Scale-Free Planner — an UP tool

A long-range planning tool where the level of detail is determined by distance in time, not by the planner.

## What it's for

Most planning tools operate at a single level of granularity — a weekly planner, a project board, a quarterly roadmap. Switching between them means maintaining multiple systems and manually keeping them in sync.

The Scale-Free Planner works across all horizons at once. Near-term slots are narrow and concrete; distant slots are wide and approximate. The structure reflects how planning actually works: you know what you're doing this week, you have a rough sense of next quarter, and beyond that you're working with intentions rather than commitments.

## How it works

Tasks and plans are assigned to time slots. The slots are quantised — a fixed set of intervals — but their width grows with distance from the present. The default set of slots, from the most distant to the most immediate, is:

- **4 years** — aligned to a fixed grid (2001–2004, 2005–2008, …), dividing a lifetime into 25 equal intervals; the final year of each period is always divisible by 4
- **2 years**
- **1 year**
- **Half a year**
- **Quarter**
- **Month**
- **Half a month** — the division of a month into two halves is conventional; the recommended approach is to follow the week boundaries below
- **Week** — months do not divide neatly into equal weeks; it is more practical at this level to work with whole weeks on a fixed cycle (e.g. Monday–Sunday), assigning each week to the month that contains the majority of its days

The default slots can be adjusted to suit your needs.

## The key principle: slots divide, they don't shift

As time passes, slots are never relabelled or reshuffled. Instead, they divide. When a distant slot draws close enough, it splits into the narrower slots that now fit inside it. A task sitting in "next quarter" stays there as the quarter approaches — and when the time comes to plan that quarter in detail, the slot is divided and the task is placed more precisely within it.

This means the system never needs to be rebuilt from scratch. Persistent plans accumulate and refine over time rather than expiring and being replaced.

## Ripening

A slot is considered ripe for division when less than half of its length remains before it begins. For a three-month quarter, that means the slot ripens around six weeks before it starts. Ripening is a signal — not an obligation. It prompts the user to look at what is in that slot and decide how to distribute it among the narrower intervals it will divide into.

The decision of when and how to divide is always the user's. The tool surfaces the moment; the user makes the call.

## Shared planning

The scale-free structure works naturally for planning between two or more people. A shared board gives everyone visibility of the same horizon, from the concrete near-term to the approximate long-term. Because slots divide gradually rather than resetting periodically, there is no fixed moment when everyone must sit down and replan together — the system accommodates asynchronous contribution and refinement.

## Implementation

This tool has no required technology. Use whatever fits your workflow:

- A Trello board with one list per slot
- A spreadsheet with columns or sections per interval
- A physical board with labelled columns
- A plain document reviewed and updated periodically

The structure is the method. The medium is up to you.

## UP compatibility

This tool follows the UP principle of reflecting existing pressure without adding its own:

- No enforced rhythm — there is no required planning cadence; the user engages when a slot ripens or when it feels right
- No punishment for absence — the structure persists unchanged; returning after time away requires no rebuilding
- No false urgency — ripening is a soft signal based on elapsed time, not a deadline imposed by the tool
- Detail emerges from reality — granularity is determined by proximity in time, not by a schema the tool imposes

→ [Example plan](example-plans.md#scale-free-planner)