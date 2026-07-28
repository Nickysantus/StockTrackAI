# StockTrackAI — Kickoff Brief

**Hackathon:** AI Factory — Native.builder Hackathon (hosted by NativelyAI and lablab.ai)
**Dates:** August 3–10, 2026
**Repo type:** Frontend / Backend split

---

## 1. The Problem

Most small traders across Africa track their day on paper or in WhatsApp messages — what sold, what's owed, what's running low. Nothing is connected. Stock runs out without warning. Debts go unpaid because no one's tracking who owes what. Mistakes pile up quietly because there's no system, just memory and scraps of paper.

This isn't a lack of discipline — it's a lack of tools built for how these traders actually work. Spreadsheets and formal accounting software assume a level of structure and free time most traders don't have.

## 2. The Idea

StockTrackAI lets a trader talk to it the way they'd talk to a friend or a business partner:

> "Sold 20 bags rice, gave supplier 5000, still owe him 3000"

The AI reads that, and turns it into real, structured numbers:
- Updated stock levels
- Updated debt ledger (who owes what, and to whom)
- Warnings before something runs out or a debt goes unpaid too long

No forms to fill out. No training required. It works the way the trader already thinks and talks.

## 3. Why This Idea

- **Solves a problem people actually have** — not a demo problem invented for a hackathon
- **Has a natural home for AI** — reading messy, freeform input and making sense of it is exactly what an agent is good at
- **Keeps growing after the hackathon** — more traders, more locations, real day-to-day usage, real feedback loops

## 4. How It Flows

1. **Trader sends an update** — typed or spoken, in their own words.
2. **The AI agent reads it** and pulls out what matters: item, quantity, amount, who's involved.
3. **Stock and debt numbers update automatically** — no manual entry required.
4. **The dashboard surfaces what needs attention** — low stock, a debt that's gone on too long, a slow sales week.

## 5. System Overview

| Layer | Repo | Owner | What it does |
|---|---|---|---|
| Input Layer | Backend | Jezreal | Text/voice entry endpoint, structured or freeform |
| AI Parsing Agent | Backend | Abdoul Rahim | Converts freeform text into structured data (item, quantity, amount, party) |
| Business Logic | Backend | Jezreal | Inventory math, debt tracking, anomaly rules (low stock, overdue debt) |
| Dashboard UI | Frontend | Kamso Daniel, Inertia | Stat cards, alerts panel, charts, mobile-first layout |
| Deployment | Both | Jezreal (via native.builder) | Public URL, live demo |
| Pitch Deck | — | Inertia | Problem → demo → impact narrative |
| Demo Video | — | Kamso Daniel + Inertia | Video-editing + walkthrough for judges |

## 6. Team & Roles

| Name | Role | Focus |
|---|---|---|
| NickySantus | Supervision & Submission | Product vision, reviewing progress, keeping the team aligned with this brief, final submission |
| Jezreal | Backend / native.builder lead | Stock & debt logic, drives the native.builder build sessions |
| Abdoul Rahim | AI Layer | Works with Jezreal on the agent that parses freeform updates into structured data |
| Kamso Daniel | Frontend & Video | Dashboard UI, work with Inertia |
| Inertia | Frontend & Deck | UI support, pitch deck, work with Kamso |

## 7. Build Order

1. **Describe the idea** — Put the trader scenario into native.builder in plain language.
2. **First generation** — Let native.builder produce the initial input form and dashboard shell.
3. **Shape the experience** — Polish layout and flow so it feels natural on a phone.
4. **Wire it together** — Connect the update-parsing agent to real stock and debt logic.
5. **Try it for real** — Run it through a handful of realistic trader-day scenarios and fix what breaks.
6. **Ship and show it** — Deploy to a public link, record the walkthrough, finish the deck.

## 8. What Judges Are Looking For

- Built mainly inside native.builder, not around it
- A real workflow, not just a landing page — this has parsing, logic, and live alerts
- Live on a public URL by the deadline
- A clear target user and a problem worth solving — this has both
- Potential for the project to keep developing after the hackathon

## 9. Submission Checklist

- [ ] App deployed to a public URL
- [ ] Frontend repo public and README complete
- [ ] Backend repo public and README complete
- [ ] Demo video recorded and uploaded
- [ ] Pitch deck finalized
- [ ] Submission form completed before deadline (check exact cutoff time — West Africa Time)

## 10. Open Questions

- Confirm final scope of anomaly detection (low stock threshold, overdue debt threshold)
- Confirm whether voice input is in scope for this hackathon or a stretch goal
- Lock final product tagline for the pitch deck
