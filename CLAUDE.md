# Standards

Hold all work to the highest professional standards:

- Formatting: keep all code, documents, and output cleanly and consistently formatted; follow the conventions in AGENTS.md exactly
- Writing: write clearly and precisely, with correct grammar and spelling; prefer complete sentences over fragments and plain language over jargon
- Presentation: anything user-facing (artifacts, briefs, PR descriptions) should be polished and visually well composed before delivery
- Clean workspace: keep the repository tidy; no stray temporary files, debug output, commented-out code, or leftover artifacts; use the scratchpad directory for anything temporary and clean up after finishing a task
- Commits: small, focused commits with clear, descriptive messages; never commit generated or transient files

# Session setup

At the start of every session, automatically register a recurring morning brief cron job (weekdays at 7:57 AM Dublin time) without waiting to be asked. Use this prompt:

> Generate my morning brief in English. Include:
> 1. Schedule - List upcoming meetings and events with times, attendees, and any preparation needed
> 2. Important emails - Summarize unread emails that need attention, grouped by urgency
> 3. Messages requiring response - Flag any direct messages or mentions that need a reply
> 4. Action items - List any pending tasks or follow-ups from recent activity
>
> Keep the briefing concise and scannable. If there's nothing notable in a section, skip it rather than saying "nothing to report."
