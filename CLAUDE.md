# Standards

Hold all work to the highest professional standards:

- Formatting: keep all code, documents, and output cleanly and consistently formatted; follow the conventions in AGENTS.md exactly
- Writing: write clearly and precisely, with correct grammar and spelling; prefer complete sentences over fragments and plain language over jargon
- Presentation: anything user-facing (artifacts, briefs, PR descriptions) should be polished and visually well composed before delivery
- Clean workspace: keep the repository tidy; no stray temporary files, debug output, commented-out code, or leftover artifacts; use the scratchpad directory for anything temporary and clean up after finishing a task
- Commits: follow the Conventional Commits format (feat:, fix:, docs:, style:, refactor:, test:, chore:) with a clear, descriptive subject; keep commits small and focused; never commit generated or transient files
- Pull requests: keep PRs small and reviewable, targeting under 400 changed lines; one concern per PR
- Documentation: structure every document as exactly one Diataxis type (tutorial, how-to, reference, or explanation); never blend types in one page
- Writing style: follow Microsoft Writing Style Guide principles; active voice, plain language, write like you speak, user-first framing
- Accessibility: user-facing pages use a 16px minimum body size, 1.5 line height, text that scales to 200% without breaking layout, fonts with distinguishable characters, and APCA-aware contrast
- AI-generated code: review generated code to the same standard as handwritten code before committing; never merge on trust

# Session setup

At the start of every session, automatically register a recurring morning brief cron job (weekdays at 7:57 AM Dublin time) without waiting to be asked. Use this prompt:

> Generate my morning brief in English. Include:
> 1. Schedule - List upcoming meetings and events with times, attendees, and any preparation needed
> 2. Important emails - Summarize unread emails that need attention, grouped by urgency
> 3. Messages requiring response - Flag any direct messages or mentions that need a reply
> 4. Action items - List any pending tasks or follow-ups from recent activity
>
> Keep the briefing concise and scannable. If there's nothing notable in a section, skip it rather than saying "nothing to report."
