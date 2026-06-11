# LI-Prospects

Working repository for a B2B prospect research agent supporting Dan Nugent, Principal Consultant at The Seismic Group. The agent identifies and qualifies LinkedIn prospects for the firm's group sourcing (GPO-style) procurement program serving $100M+ US food & beverage manufacturers.

The agent researches, qualifies, scores, and organizes prospects. It does **not** conduct outreach — the consultant owns all engagement.

## Repository structure

| File | Purpose |
|---|---|
| `CLAUDE.md` | The agent's system prompt: ICP, target personas, search strategy, fit-scoring rubric, and guardrails. Sessions in this repo operate under it. |
| `prospects/prospects.csv` | The master prospect list. One row per qualified prospect, fields per the capture spec in `CLAUDE.md`. |
| `exclusion-list.csv` | Current program members and active pipeline opportunities. Every new prospect is checked against this before being added. |

## Quick-start commands

- `build list [segment] [count]` — produce a scored prospect table for that F&B segment
- `expand account: [company name]` — find all target-persona stakeholders at one company
- `find PE: [segment]` — identify PE firms and partners with portfolio exposure in that segment
- `verify: [company name]` — research revenue, ownership, and fit signals for a flagged company
- `list report` — summary of total prospects by segment, persona, and fit score

## Placeholders to complete before deployment

- [x] Replace `[FIRM NAME]` and `[CONSULTANT]` in `CLAUDE.md` — The Seismic Group / Dan Nugent
- [ ] Populate `exclusion-list.csv` with current members and active deals
- [ ] Note any priority segments or geographies-within-US to mine first
