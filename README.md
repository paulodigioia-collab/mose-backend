# MOSE.ART — Backend Ops Board
> A private, live **ticking clock + master to-do** board for the MOSE.ART dinner-experience build. Personal ops only — **not for investors**.

**▶ Live board:** __VERCEL_URL__  · open on your phone; the clock counts down to the first night.
**▶ Source (this repo):** __REPO_URL__  · so your Claude can edit / upgrade it.

---

## For Johnny's Claude — how to work on this
- It is **one self-contained file: `index.html`** (HTML + CSS + JS, no build step, no dependencies, no keys).
- To change things, edit inside the `<script>` at the bottom:
  - **The to-dos** → the `PHASES` array (each phase has items `[id, "text", "lock|go|idea"]`).
  - **Decisions / content** → the `DECISIONS` and `CONTENT` arrays.
  - **The event date** (the countdown target) → the `EVENT` constant (currently `2026-09-04T19:30` — a working date, confirm).
- Checkmarks are saved in the browser (localStorage), per device.
- **Publish a change:** commit + push to this repo, then redeploy on Vercel (`vercel --prod`) — or connect this repo to the Vercel project for auto-deploy on push.
- Keep it **personal and simple** — this is the "what do we both need to see" board.

## The project in one paragraph
MOSE.ART is a private dinner + club experience in Amsterdam. We sell in waves: **inner circle (~600 friends) → wider circle (to net ~120 diners) → club tickets (unique QR)**. Payment is **upfront** (a deposit that becomes bottle/champagne credit at the event). The full plan + locked rules live in the main workspace (`MASTER_SELL_PLAN.md`); this board is the at-a-glance tracker of it.

## Johnny's lane (your to-dos)
- Write the event **story / theme** (from your other account).
- **Curate your own contacts** — reserve spots for your people and call them ("I reserved a spot for you"). A curated-spot builder for this is in the plan (build later).
- The **promo / aftermovie** content (works projected on walls + spoken word, dark→light "tunnel" reveal).

## Rules (don't break)
- Brand is **MOSE.ART**, never "Mozart."
- **Don't lock any price yet** — the numbers from the last call were garbled; confirm first.
- Payment is **upfront only**; the "nominate 2 people" perk is shown **before** payment.
