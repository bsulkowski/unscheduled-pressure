# Pace Planner — an UP tool

A tool for tracking open-ended activities that have no deadlines — only a desired pace.

## What it's for

Some activities matter but never become urgent. Learning a language, exercising, playing games, reading for pleasure — these compete for the same limited resource: free time. And the less free time there is, the more worthwhile it is to spend it intentionally.

At the same time, any system that turns leisure into obligation defeats its own purpose. The Pace Planner is designed to maintain awareness of how time is distributed across these activities without turning that awareness into pressure.

## How it works

Each activity is assigned a planned average — a target amount of time per day. A marker tracks progress against that plan by moving forward and backward in the calendar.

Daily averages are chosen from a set of quantised values rather than entered as free numbers. The default set is: 5, 7, 10, 15, 20, 30 minutes. As with the frequency intervals in Recurring Tasks, the point is to remove a non-decision — whether an activity deserves 13 or 14 minutes a day is meaningless, and deliberating over it would add friction without value. The default values can be adjusted to suit your needs.

If the marker sits on today, you are exactly on pace. If you spend time on the activity, the marker moves forward proportionally. Thirty minutes on an activity planned at fifteen minutes per day moves the marker two days ahead. If the marker is ahead of today, that activity has been getting more than its share of time recently — a natural signal to let other things catch up. If the marker is behind today, that activity has been neglected.

No entry is required on days when nothing happens. The marker simply stays where it is.

→ [Example plan](example-plans.md#pace-planner)

## What the marker is not

The marker is not a deadline. It does not generate guilt. Spending an hour on something planned at fifteen minutes a day is fine — it just means the marker moves further ahead, and the activity will naturally fade into the background for a while. The system reflects choices; it does not judge them.

## Leeway

Over time, the gap between plan and reality can grow large enough to stop being useful. A marker that is weeks behind starts to feel hopeless — the plan is so far out of reach that trying seems pointless. A marker that is weeks ahead either creates paralysis — making it hard to engage with the activity at all — or loses its signal value, so the gap between plan and reality goes unnoticed.

The leeway mechanism gently closes these gaps on a regular basis. Once a week, all distances from the present are reduced proportionally — in the reference implementation, by 1 day for each 5 days of gap. A marker three weeks ahead moves back by four days. A marker two weeks behind moves forward by three days.

Leeway is not a reset. It does not erase history or pretend the gap never happened. It gradually reconciles the plan with reality, keeping the markers close enough to the present to remain motivating.

The weekly adjustment is applied in reference to a fixed day — Monday in the reference implementation — but can be run on any day.

## Implementation

This tool has no required technology. Use whatever fits your workflow:

- A Trello board with one card per activity, using due dates as markers
- A spreadsheet tracking dates and daily targets
- A physical calendar with moveable markers
- A plain document updated manually

The structure is the method. The medium is up to you.
