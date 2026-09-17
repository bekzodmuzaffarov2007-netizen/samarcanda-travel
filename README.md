# Samarcanda Travel

Premium Uzbekistan travel platform.

## Current status

The live site is currently a static GitHub Pages prototype. The production architecture is planned as a Next.js application with a database, secure server-side APIs, a custom-trip planner, booking/inquiry system, and Telegram AI assistant.

## Telegram + AI architecture

The Telegram bot should be deployed as a separate server-side service or API route with:

- Telegram Bot API webhook
- server-side AI API key stored only in environment variables
- PostgreSQL/Supabase for conversations and inquiries
- structured tour data shared with the website
- Uzbek, Russian, and English responses
- human handoff for complex requests

Never put Telegram bot tokens or AI API keys in the browser or GitHub repository.
