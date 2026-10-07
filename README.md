# Nikita Rozumniy — AI Automation Engineer

I build production automation systems for real businesses: event-driven pipelines that connect ordering platforms, documents, AI models and communication channels — running on self-hosted infrastructure I administer myself.

📍 Germany · 💬 Ukrainian / Russian (native), German (C1), English (technical)
🔗 [LinkedIn](https://www.linkedin.com/in/nikita-rozumniy)

## Featured Projects

| Project | What it does | Stack |
|---|---|---|
| [**choice-invoice-automation**](https://github.com/nikita-automation/choice-invoice-automation) | Production invoice automation for a food-delivery business: ~70 accounting PDFs/day generated from order webhooks, delivered by e-mail + Google Drive, with a 3-year retention policy as code | n8n, Python, ReportLab, SQLite, OAuth2, ChoiceQR API |
| [**job-hunter-bot**](https://github.com/nikita-automation/job-hunter-bot) | Telegram bot that runs my own job search: daily Arbeitsagentur crawl, GPT-4o scoring against my CV, tailored German cover letters, applications sent only after two explicit taps. First production run: 149 openings scored, 5 applications out the same day | n8n (self-hosted), Python generators, OpenAI, Telegram Bot API, SMTP, GitHub Actions |
| [**business-site-finder**](https://github.com/nikita-automation/business-site-finder) | Finds local businesses with no or an outdated website, builds a personalised demo site and a print-ready letter with a QR code. Synthetic data only, nothing is sent; tested in CI | Python, SQLite, Jinja2, Google Places API, headless Chrome, GitHub Actions |
| [**linkedin-autopost-n8n**](https://github.com/nikita-automation/linkedin-autopost-n8n) | Twice-weekly LinkedIn posts written by Claude from the latest blog articles, through the LinkedIn Posts API (the built-in n8n node is pinned to a retired API version) | n8n, Anthropic Claude, WordPress REST API, LinkedIn API, OAuth2 |
| [**content-publishing-pipeline**](https://github.com/nikita-automation/content-publishing-pipeline) | End-to-end video pipeline: translate → edit → caption → auto-publish short-form video to LinkedIn, Instagram & YouTube from a single Telegram approval | n8n, HeyGen, Submagic, Anthropic Claude, Blotato, Google Sheets |
| [**ai-meeting-transcription**](https://github.com/nikita-automation/ai-meeting-transcription) | Meeting recordings → transcripts, summaries and action items with human review | n8n/Make.com, Whisper, OpenAI, Google Workspace |
| [**telegram-ai-autoreply**](https://github.com/nikita-automation/telegram-ai-autoreply) | Self-hosted Telegram assistant with whitelist guard and conversation routing | Python (Telethon), n8n, OpenAI, Docker Compose |

## Demo projects — HR and staffing automation, written from scratch

Reference implementations of recurring problems in HR and staffing automation, built on invented data only. Every one has a test suite that was mutation-checked, CI on Python 3.9 and 3.12, and an honest evaluation (a held-out set where a model or classifier is involved). Model-based parts are covered by tests with a stub client, not by live runs.

| Project | What it does | Stack |
|---|---|---|
| [**shift-plan-compliance-checker**](https://github.com/nikita-automation/shift-plan-compliance-checker) | Checks shift plans against German working-time law (ArbZG): breaks, rest periods, daily and weekly hours, Sunday and holiday work. Boundary-tested, usable as a CI gate | Python (stdlib), GitHub Actions |
| [**applicant-inbox-consolidation**](https://github.com/nikita-automation/applicant-inbox-consolidation) | Merges applications from six channels into one SQLite inbox, normalises phone numbers, e-mails and names, and merges duplicates without gluing together strangers who share a phone or a mailbox | Python, SQLite |
| [**cv-screening-assistant**](https://github.com/nikita-automation/cv-screening-assistant) | Structured extraction from CVs and questionnaires (DE/EN): offline rules and a Claude structured-output backend, scored on a development and a held-out set (rules: 96.8 % vs 75 %), plus explained screening against a job profile | Python, Anthropic API |
| [**email-triage-assistant**](https://github.com/nikita-automation/email-triage-assistant) | Sorts a recruiting inbox and prepares reply drafts in the Drafts folder — it never sends. The model proposes, code decides: legal and GDPR safety nets, fact-checked model-written replies | Python, IMAP, Anthropic API |

## How I work

- **Business impact first** — I measure automations in hours saved and errors eliminated, not in node counts
- **Production discipline** — idempotent pipelines, encrypted credential stores, error handling, versioned workflows, data-retention policies
- **Self-hosted by default** — Linux VPS, Docker, Nginx, cron; full control over data and costs

## Stack

`n8n` `Python` `Make.com` `OpenAI API` `Anthropic Claude` `Whisper` `HeyGen` `Submagic` `ElevenLabs` `Blotato` `REST APIs` `OAuth2` `Webhooks` `SQLite` `PostgreSQL` `Docker` `Linux` `Nginx` `Git` `Telegram Bot API` `Google Workspace` `Airtable` `GitHub Actions`

## Currently Learning

`PostgreSQL` · `Docker` · `Python` · `Advanced n8n` · `AI Agents`

## Contact

- LinkedIn: [linkedin.com/in/nikita-rozumniy](https://www.linkedin.com/in/nikita-rozumniy)
- Email: `nikita.rozumniy77@gmail.com`
