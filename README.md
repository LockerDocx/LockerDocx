<h1 align="center">Gerard Morales</h1>
<p align="center">
  <strong>Systems · AI Integration · Cybersecurity</strong><br>
  Barcelona, Catalonia, Spain · Founder at WebProDev · Open to work
</p>

---

## About

Systems and software developer based in Barcelona, currently in the first year of **ASIX
(cybersecurity)** at Institut Tecnològic de Barcelona. I build AI-integrated web products
through **WebProDev** and take on infrastructure, IT support and development work. Comfortable
across the stack: hardware and networks at the bottom, TypeScript and Python applications at
the top.

## Featured — AI Agent for Firefox

[`LockerDocx/firefox-ai-agent`](https://github.com/LockerDocx/firefox-ai-agent) · MIT

Free, open-source AI agent that drives a real Firefox browser from a plain-language goal.
A Python orchestration loop observes the page as an indexed table of elements, requests one
operation and one target from a language model, and executes it — the model never writes
selectors or code.

- **Measured, not estimated.** The executor prompt was reduced by **52.4 %** (21,233 →
  10,111 characters) on a dense page and decoupled from page size;
  `scripts/bench_prompt_size.py` reproduces the full trade-off curve.
- **Built around a real failure.** v0.13.0 shipped a one-line quoting bug that broke every
  click, fill and select with a JavaScript `SyntaxError`; 585 tests missed it because the
  suite replaced the CDP layer. Now covered end to end.
- **Scored without self-flattery.** `scripts/live_battery.py` determines success from the
  final URL rather than the agent reporting `DONE`, and emits `NO EVALUABLE` rather than a
  percentage that cannot be compared against a target.

**819 tests**, ruff clean, shipped through a release pipeline that publishes the wheel, the
`.xpi` and the source archive, with every change logged in `CHANGELOG.md` alongside what
was measured and what was not.

## Selected Work

| Project | Description | Stack |
|---|---|---|
| [Quatre40optics](https://github.com/LockerDocx/Quatre40optics) | Client website rebuilt from a Hostinger builder site into a maintained codebase and migrated to Vercel at no cost, with the DNS runbook included. | Next.js 14, React 18, TypeScript, Tailwind |
| [Arnamar.sl](https://github.com/LockerDocx/Arnamar.sl) | Client AI platform for renovation work: natural-language input driving image editing, plus vision-based surface estimation from site photos. | React 18, Vite, TypeScript, Express, Gemini 2.5 |
| [arduino-iot-monitor](https://github.com/LockerDocx/arduino-iot-monitor) | Final project for my systems and networks cycle: live temperature and humidity from an Arduino UNO + DHT11 to a web dashboard. | Arduino, Next.js, Firebase, TypeScript |
| [Webprodev](https://github.com/LockerDocx/Webprodev) | Website of my own studio: services, portfolio and pricing, plus client and admin dashboards and an AI chat widget. | React, TypeScript, Firebase |

## Experience

**Founder and Developer — WebProDev** · Jun 2023 – present
Web development, custom software and AI integration for clients, from first conversation
through design, build, deployment and maintenance.

**IT Support Technician — Châteauform, Campus Belloch** · Feb 2025 – Apr 2026 · 365 h
User onboarding and offboarding, Active Directory and Microsoft Exchange for accounts,
mailboxes, permissions and shares, hardware deployment, and asset management in GLPI.

**Hardware Technician — Mondo Computer, Forlì, Italy** · Jun 2026 · ~150 h · Erasmus+
Component-level diagnosis and refurbishment of laptops, and reassembly of working machines
from salvageable parts.

## Education and Certification

- **ASIX, Cybersecurity** — Institut Tecnològic de Barcelona · from Sep 2026
  Systems administration, networking, virtualisation and security on Windows and Linux.
- **Sistemes Microinformàtics i Xarxes** — Escola Ginebró · 2024 – 2026 · grade 8.80
  Hardware, operating systems and networking, culminating in the IoT project above.
- **Cisco Networking Academy — Introduction to Cybersecurity** · Nov 2025 · 6 h, 7 labs
- **Cisco Networking Essentials** · 2026

**Languages** — Catalan and Spanish, native.

**Contact** — [LinkedIn](https://www.linkedin.com/in/gerard-morales/) ·
Open to opportunities in systems administration, IT support, development and AI integration,
in Barcelona or remote.
