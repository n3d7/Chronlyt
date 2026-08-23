# Statistics

Statistics answers one practical question: **what happened during the period I selected?** It is a factual workspace, separate from Analytics, which looks for broader patterns and observations.

## Choose a period

The selector at the top applies to every Statistic on the page. Choose Today, Yesterday, This Week, Last Week, Last 7 Days, This Month, Last Month, Last 30 Days, This Year, All Time, or a custom inclusive date range.

When **Show comparisons** is enabled, Chronlyt compares the selection with the immediately preceding equivalent period. All Time has no comparison. If the earlier value is zero, Chronlyt reports “New this period” instead of an infinite percentage.

Timestamp-backed records are assigned to the local calendar period in which they started. A Focus Session that crosses midnight is one session, and pausing, resuming, recovering, or hiding the window never creates another start.

## Customize the workspace

Choose **Customize** to:

- add a Statistic from the searchable, grouped picker;
- drag Statistics into a different order;
- cycle between Small, Medium, Large, and Wide sizes;
- remove a Statistic without deleting any underlying data;
- restore the default layout.

The Statistics layout is stored locally and independently from the Dashboard layout.

## Understand the numbers

Use the information icon for the exact definition and select a card for details. The default layout includes Focus Time, Timers Started, Activities, Net Financial Change, Focus over time, Tasks Completed, Plan vs Actual, Activity Breakdown, Time Leaks, and Learning Time. Additional choices cover session duration, a focus heatmap, Goal-linked time, health, finance, content, XP, streaks, and recorded Rule Violations.

Finance follows `income − expenses + signed adjustments`. Opening balances are excluded. If more than one currency is present, each currency remains separate because Chronlyt does not invent exchange rates.

Time Leaks count only explicit categories such as procrastination, social media, or idle time. Rule Violations and unplanned content are likewise based only on what you deliberately record; Chronlyt does not infer classifications.

## Empty periods

An empty card explains which source record would populate it. No data is displayed as a percentage, `NaN`, or an empty chart. Changing or removing Statistics never changes Tasks, Activities, Focus Sessions, or Finance records.
