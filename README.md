# Nikita Rozumnyi · KI-Automatisierung für Unternehmen

Ich automatisiere Geschäftsprozesse mit KI: Rechnungen, Posteingänge, Bewerbungen, Content und Berichte laufen bei meinen Systemen ohne Handarbeit durch. Ich baue mit n8n, Python und den APIs von OpenAI und Anthropic Claude, betreibe alles auf eigener Linux-Infrastruktur und messe den Erfolg in eingesparten Stunden und vermiedenen Fehlern.

**Ab sofort verfügbar** für eine Festanstellung oder Automatisierungsprojekte.

📍 Recklinghausen, NRW · 💬 Deutsch (C1), Ukrainisch/Russisch (Muttersprache), Englisch (technisch)

[![Website](https://img.shields.io/badge/Website-nikita--automation.de-0A66C2?style=flat-square)](https://nikita-automation.de)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Nikita%20Rozumnyi-0A66C2?style=flat-square&logo=linkedin)](https://www.linkedin.com/in/nikita-rozumniy)
[![YouTube](https://img.shields.io/badge/YouTube-%40Nikita.automation-FF0000?style=flat-square&logo=youtube)](https://www.youtube.com/@Nikita.automation)
[![Instagram](https://img.shields.io/badge/Instagram-nikita.automation-E4405F?style=flat-square&logo=instagram)](https://www.instagram.com/nikita.automation)

---

## Was ich automatisiere

| Bereich | Typische Aufgabe | Beispiel unten |
|---|---|---|
| **Buchhaltung & Dokumente** | Belege und Rechnungen automatisch erzeugen, ablegen und archivieren | choice-invoice-automation |
| **HR & Recruiting** | Bewerbungen aus allen Kanälen bündeln, Lebensläufe auslesen, Posteingang sortieren, Schichtpläne prüfen | vier HR-Demoprojekte |
| **Marketing & Content** | Blogartikel zu LinkedIn-Posts, Videos übersetzen, untertiteln und veröffentlichen | linkedin-autopost-n8n, content-publishing-pipeline |
| **Kommunikation** | Meetings und Anrufe transkribieren und zusammenfassen, Telegram-Assistenten | ai-meeting-transcription, telegram-ai-autoreply |
| **Vertrieb** | Lokale Firmen ohne aktuelle Website finden und eine Demo-Seite vorbereiten | business-site-finder |

## Produktive Projekte

| Projekt | Was es macht | Stack |
|---|---|---|
| [**choice-invoice-automation**](https://github.com/nikita-automation/choice-invoice-automation) | Rechnungsautomatisierung für einen Lieferdienst: rund 70 Buchhaltungs-PDFs pro Tag aus Bestell-Webhooks, Versand per E-Mail und Google Drive, 3 Jahre Aufbewahrung als Code | n8n, Python, ReportLab, SQLite, OAuth2 |
| [**linkedin-autopost-n8n**](https://github.com/nikita-automation/linkedin-autopost-n8n) | Zwei LinkedIn-Posts pro Woche, von Claude aus den neuesten Blogartikeln geschrieben, über die LinkedIn Posts API. Läuft seit September 2026 | n8n, Anthropic Claude, WordPress REST API, LinkedIn API |
| [**content-publishing-pipeline**](https://github.com/nikita-automation/content-publishing-pipeline) | Ein Rohvideo wird übersetzt, geschnitten, untertitelt und nach einer Freigabe in Telegram auf LinkedIn, Instagram und YouTube veröffentlicht | n8n, HeyGen, Submagic, Claude, Blotato |
| [**job-hunter-bot**](https://github.com/nikita-automation/job-hunter-bot) | Telegram-Bot: täglicher Abruf der Arbeitsagentur-Jobbörse, Bewertung mit GPT-4o gegen ein Profil, passende Anschreiben, Versand erst nach zwei bewussten Klicks. Erster Lauf: 149 Stellen bewertet | n8n, Python, OpenAI, Telegram Bot API, GitHub Actions |
| [**business-site-finder**](https://github.com/nikita-automation/business-site-finder) | Findet lokale Firmen ohne oder mit veralteter Website und erstellt eine persönliche Demo-Seite plus Brief mit QR-Code. Synthetische Daten, mit CI getestet | Python, SQLite, Jinja2, Google Places API |
| [**ai-meeting-transcription**](https://github.com/nikita-automation/ai-meeting-transcription) | Meeting-Aufnahmen werden zu Transkript, Zusammenfassung und Aufgabenliste, mit menschlicher Prüfung | n8n, Whisper, OpenAI, Google Workspace |
| [**telegram-ai-autoreply**](https://github.com/nikita-automation/telegram-ai-autoreply) | Selbst gehosteter Telegram-Assistent mit Whitelist, Rate-Limit und Gesprächsgedächtnis | Python (Telethon), n8n, OpenAI, Docker Compose |

## Demoprojekte: HR- und Personalautomatisierung

Referenzimplementierungen für wiederkehrende Aufgaben in HR und Personaldienstleistung, nur mit erfundenen Daten. Jedes Projekt hat eine Testsuite (mit Mutationstests geprüft), CI auf Python 3.9 und 3.12 und eine ehrliche Auswertung auf einem zurückgehaltenen Testset, wo ein Modell beteiligt ist.

| Projekt | Was es macht | Stack |
|---|---|---|
| [**shift-plan-compliance-checker**](https://github.com/nikita-automation/shift-plan-compliance-checker) | Prüft Schichtpläne gegen das Arbeitszeitgesetz: Pausen, Ruhezeiten, Tages- und Wochenstunden, Sonn- und Feiertagsarbeit. Nutzbar als CI-Gate | Python (stdlib), GitHub Actions |
| [**applicant-inbox-consolidation**](https://github.com/nikita-automation/applicant-inbox-consolidation) | Führt Bewerbungen aus sechs Kanälen in einem SQLite-Posteingang zusammen und erkennt Dubletten, ohne Fremde mit gleicher Nummer zu verschmelzen | Python, SQLite |
| [**cv-screening-assistant**](https://github.com/nikita-automation/cv-screening-assistant) | Strukturierte Extraktion aus Lebensläufen (DE/EN) mit Regeln oder Claude Structured Output, ausgewertet auf Entwicklungs- und Testset, plus begründetes Screening gegen ein Stellenprofil | Python, Anthropic API |
| [**email-triage-assistant**](https://github.com/nikita-automation/email-triage-assistant) | Sortiert ein Recruiting-Postfach und legt Antwortentwürfe ab, sendet aber nie selbst. Das Modell schlägt vor, der Code entscheidet: Sicherheitsnetze für Recht und DSGVO | Python, IMAP, Anthropic API |

## Wie ich arbeite

- **Nutzen zuerst:** Eine Automatisierung zählt in gesparten Stunden und vermiedenen Fehlern, nicht in der Zahl der Nodes.
- **Produktionsreif:** idempotente Abläufe, verschlüsselte Zugangsdaten, Fehlerbehandlung, versionierte Workflows, Aufbewahrungsregeln.
- **Mensch behält die Kontrolle:** Wo es um Geld, Bewerber oder Kunden geht, gibt ein Mensch frei, bevor etwas rausgeht.
- **Selbst gehostet:** Linux-VPS, Docker, Nginx, cron. Daten und Kosten bleiben beim Kunden.

## Stack

`n8n` `Python` `Make.com` `OpenAI API` `Anthropic Claude` `Whisper` `HeyGen` `Submagic` `ElevenLabs` `Blotato` `REST APIs` `OAuth2` `Webhooks` `SQLite` `PostgreSQL` `Docker` `Linux` `Nginx` `Git` `GitHub Actions` `Telegram Bot API` `Google Workspace` `Airtable`

---

### In English

I'm Nikita Rozumnyi, an AI automation engineer based in Germany. I build production automations with n8n, Python, OpenAI and Anthropic Claude: invoice generation, inbox and applicant triage, content publishing and meeting summaries, self-hosted on Linux. Available now for a full-time role or automation projects. The tables above link every project; each repository has an English README.

## Kontakt

- Website: [nikita-automation.de](https://nikita-automation.de)
- LinkedIn: [linkedin.com/in/nikita-rozumniy](https://www.linkedin.com/in/nikita-rozumniy)
- E-Mail: `nikita.rozumniy77@gmail.com`
