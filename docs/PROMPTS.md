# Prompts

Document type: reference (Diataxis). Reusable prompts for the work environment.

## Morning brief

The prompt fired by the weekday cron job (7:57 AM Dublin time):

> Generate my morning brief in English. Include:
>
> 1. Schedule - List upcoming meetings and events with times, attendees, and any preparation needed
> 2. Important emails - Summarize unread emails that need attention, grouped by urgency
> 3. Messages requiring response - Flag any direct messages or mentions that need a reply
> 4. Action items - List any pending tasks or follow-ups from recent activity
>
> Keep the briefing concise and scannable. If there's nothing notable in a section, skip it rather than saying "nothing to report."

## Re-register the morning brief

Use when a session has expired and the cron is gone:

> Set up the morning brief as a recurring task again.

## Run the brief once

Use for an on-demand brief outside the schedule:

> Generate my morning brief now.

## Verify the schedule

Use to confirm the cron job is registered in the current session:

> List my scheduled cron jobs.
