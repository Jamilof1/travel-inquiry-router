# Wayfare — Travel Inquiry Router

Collect travel requirements once, create a usable brief, and route it to the right specialist workflow. Project 09 in the Jamil Darwish Automation Lab.

## Modes

- **Demo:** visible local rules determine readiness, priority, region, and desk.
- **AI:** your model reviews the current inquiry and creates a routing brief through the local proxy.

## Quick start

Requires Node.js 22+.

```bash
git clone https://github.com/Jamilof1/travel-inquiry-router.git
cd travel-inquiry-router
npm install
npm run dev
```

For AI mode, copy `.env.example` to `.env`, add `AI_API_KEY`, and restart. PowerShell: `Copy-Item .env.example .env`.

## Provider configuration

The default uses OpenAI Responses and `AI_MODEL=gpt-5`. An OpenAI-compatible chat service can set `AI_BASE_URL`, `AI_MODEL`, and `AI_API_STYLE=chat`. The key is server-only and `.env` is ignored.

## Features

- Traveler, route, date, party, style, budget, and preference intake.
- Desk/workflow routing, priority, completeness, and live travel brief.
- Optional AI route recommendation and next questions.
- Copyable routed brief with synthetic sample data.

## Commands

`npm run dev` starts both processes, `npm test` runs tests, `npm run build` creates `dist/`, and `npm start` serves it.

## Responsible use

Demo data stays local. AI mode sends the displayed inquiry only after a click. This app neither submits nor books. A specialist must verify identity, consent, pricing, availability, visas, safety, accessibility, insurance, and supplier suitability.

MIT — built by [Jamil Darwish](https://jamildarwish.com/).
