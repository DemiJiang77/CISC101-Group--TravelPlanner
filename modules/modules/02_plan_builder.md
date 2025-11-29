Module 2 — Plan Builder (Options → Days)

<!--
Changelog (2025-11-28):
- Added more info for each activity (tags, opening hours, etc.)
- Wrote simple rules for distance, timing, and lunch
- Noted a few edge cases (half-day, mobility, missing budget)
-->

This module turns a shortlist of activities into a simple day plan.

The builder now assumes:
- A “normal” day runs roughly 09:00–20:30.
- Morning and evening activities are near the lodging (or city centre if we don’t know it).
- Transfers between activities are not too far (about ≤25 minutes).

When building a day, the planner should:
- Pick a morning activity close to lodging.
- Add a lunch spot (60–75 minutes) that matches the user’s budget and diet.
- Choose an afternoon activity with a different theme, and leave a bit of buffer time for moving around.
- End with dinner or an evening event that is again not far away.

Edge cases:
- Half-day / late arrival → skip the first slot and shorten others.
- Mobility limits → prefer easier, short-walk options.
- Unknown weather → try to keep at least one indoor backup activity.
