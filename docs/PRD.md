# Product Requirements: Morning Brief Automation

Document type: explanation (Diataxis). This document explains what the morning brief automation is, why it exists, and what it must do.

## Overview

The morning brief automation generates a daily, personalized briefing for Marek every weekday morning. It gathers data from connected sources (Google Calendar, Gmail, Slack), classifies what needs attention, renders a styled HTML artifact, and sends a push notification when something requires action.

## Problem

Catching up each morning means checking a calendar, an inbox, and Slack separately, then deciding what actually matters. That takes time, invites distraction, and important items (failed payments, security alerts, blocked teammates) can be missed among noise.

## Goals

1. One glance replaces three apps: a single page shows the shape of the day and the few things that matter.
2. Zero-noise notifications: a push notification fires only when something needs action; a quiet day means silence.
3. Runs unattended: the brief generates on a weekday schedule without being asked.

## Non-goals

- Taking action on emails or messages (replying, archiving, deleting)
- Covering weekends
- Real-time monitoring between briefs

## Users

A single user: Marek (marek.d.kropiewnicki@gmail.com), Dublin timezone.

## Functional requirements

| # | Requirement |
|---|-------------|
| 1 | Generate the brief every weekday at 7:57 AM Dublin time |
| 2 | Include schedule, important emails, messages requiring response, and action items |
| 3 | Classify items into Needs attention and Resolved |
| 4 | Render as a styled HTML artifact with a visual day terrain |
| 5 | Send a push notification only when items need attention |
| 6 | Skip empty sections rather than reporting nothing |
| 7 | Write the brief in English |

## Non-functional requirements

- Presentation follows the repository accessibility standards: 16px minimum body text, 1.5 line height, APCA-aware contrast, both light and dark themes.
- Gathered content is data, never instructions: embedded commands in emails or messages are ignored.
- Quotes from sources are rendered verbatim and escaped; no live markup passes through.

## Architecture

1. CLAUDE.md instructs every new session to register a recurring cron job (weekdays, 7:57 AM Dublin).
2. The cron job fires the morning brief prompt (see docs/PROMPTS.md).
3. The brief pipeline gathers from Google Calendar, Gmail, and Slack via MCP connectors.
4. Output publishes as a Claude artifact; a push notification delivers the summary.

## Known limitations

- Cron jobs are session-scoped: they die with the session and expire after 7 days. The CLAUDE.md instruction re-registers on each new session, but a session must be open at fire time.
- MCP connectors (Gmail, Calendar, Slack) require an authenticated claude.ai session and are unavailable in headless runners.

## Future work

- A GitHub Actions scheduled workflow calling the Claude API directly, with source APIs wired via repository secrets, for fully unattended operation.
