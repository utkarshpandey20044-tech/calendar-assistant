# Calendar Assistant

This repository contains an n8n workflow for an automated calendar assistant that runs daily at 2:00 PM and sends a concise HTML email summarizing the two most important events of the day.

## Included files

- `Calender Assistant.json` — the exported n8n workflow
- `README.md` — project documentation

## What the workflow does

- Triggers every day at 14:00
- Reads today's Google Calendar events
- Analyzes event titles, descriptions, and attendees
- Selects the top 2 most important events
- Sends a clean HTML email using Gmail

## Setup

1. Import `Calender Assistant.json` into n8n.
2. Connect your Google Calendar credential.
3. Connect your Gmail credential.
4. Update the recipient email if needed.
5. Save and activate the workflow.

## Notes

- The workflow is configured for the calendar: `f20230388@goa.bits-pilani.ac.in`
- It uses the AI agent to decide importance and format the email.
- If no events are found for the day, it should send a short fallback message.

## License

This project is provided for personal automation use and is shared as-is.
