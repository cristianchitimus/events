# Status — Vermut Festival Madrid 2026 (4ª Edición)

**Last updated:** 2026-04-25 by Claude (Node 3 stage variants populated, Identity Checkpoint armed)
**Current phase:** Logo (master generated, vectorization pending; stage variants ready to run)
**Active branch:** `event/2026-08-vermut-festival-madrid`
**Workflow path:** C (artifact fallback — manual push)
**Owner:** Claude (strategist) + Carlos (client)
**Client approver:** Carlos, Festival Vermut Madrid team

## Node progress

| Node | Status | Date | Notes |
|------|--------|------|-------|
| 1 — Brief | AWAITING_PUSH | 2026-04-25 | Captured. |
| 2 — Direction | COMPLETE | 2026-04-25 | Crudo APPROVED. |
| 2.5 — Audit | SKIPPED | 2026-04-25 | Carlos opted to skip. |
| 3 — Logo (master, Ideogram + Gemini) | COMPLETE | 2026-04-25 | Composite PNG saved by Carlos. Pending: crop into 6 standalone files + Recraft vectorization. |
| 3 — Logo (master, vectorization Stage 3) | AWAITING_MANUAL_GENERATION | 2026-04-25 | Recraft pass on 3 standalone logo PNGs (cropped from composite). Recommended NOW (parallel-safe). |
| 3 — Logo (stage variants, Appendix A) | AWAITING_MANUAL_GENERATION | 2026-04-25 | All 4 stages populated and ready in `03_logo/variants.md`. ~80 min total in parallel. |
| 4 — Hero | NOT_STARTED | — | Runs after master logo SVG is locked + 2 venue photos available. |
| Identity Checkpoint | ARMED | 2026-04-25 | Pre-flight checklist ready in `00_meta/identity-checkpoint.md`. Activates after Node 4. |
| 5 — Banners | NOT_STARTED | — | Castizo Spanish copy + reformatting. |
| 6 — Video | NOT_STARTED | — | 4 LED stages (Appendix A applies). Per-stage LED dimensions TBD. |
| 7 — Music | NOT_STARTED | — | Atmospheric only, between sets. |
| 8 — Print | NOT_STARTED | — | — |
| 8.5 — Production | NOT_STARTED | — | Spain ISO 216. Imprenta TBD. |
| 9 — Brand Bible | NOT_STARTED | — | Final deadline 2026-07-20. |

## Status legend

- `NOT_STARTED` — Hasn't been touched yet
- `IN_PROGRESS` — Actively being worked on
- `ARMED` — Configured and ready, activates on a trigger event
- `AWAITING_MANUAL_GENERATION` — Prompts ready, user runs external AI tool
- `AWAITING_INPUT` — Waiting on missing config from client
- `AWAITING_REVIEW` — Output ready, user/client reviewing
- `AWAITING_PUSH` — Files generated, user pushes manually (Path C)
- `COMPLETE` — Done, no action needed
- `SKIPPED` — Deliberately bypassed
- `NEEDS_REWORK` — Failed checkpoint, needs upstream regeneration
- `FAILED` — Unrecoverable error

## The 4 stages — locked

| # | Stage | Theme | Color | Mark |
|---|---|---|---|---|
| 1 | MERCADO | Vermut tasting + acoustic + Spanish singer-songwriter (intimate) | Violeta Eléctrico `#7C3AED` | `01` |
| 2 | PLAZA MAYOR | Indie español + rock alternativo (main stage, max energy) | Cian Pavimento `#00B5D8` *(master)* | `02` |
| 3 | MADRUGADA | Electronic + techno + house DJs (late-night) | Chartreuse Eléctrico `#B8FF00` *(dark surfaces only)* | `03` |
| 4 | COCINA | Food talks + cooking demos + chef conversations (educational) | Tinta Imprenta `#5B7BFF` | `04` |

All 4 stage colors WCAG-verified ≥3.28:1 against Negro Mercado; mutually distinguishable at thumbnail size.

## Open questions / blocking items

**Blocking nothing right now** — everything has a path forward. Remaining gaps below are for downstream nodes:

**Needed before Node 4:**
- ⚠ 2 venue photos (interior of Mercado de San Fernando + Plaza de Lavapiés exterior)
- Master logo SVG vectorized

**Needed before Node 6:**
- Per-stage LED dimensions and aspect ratios (4 screens)

**Needed before Node 8.5:**
- Imprenta provider and special finishes

**Needed before Node 5:**
- Existing IG hashtag and custom filter references
- Festival IG handle

**Needed before Node 9:**
- Sponsor logo files (Cinzano, Mahou, Estrella Galicia, Lavapiés locals)

## Next recommended action

**Two parallel tracks for Carlos:**

**Track A — finish master logo (~30–45 min):**
1. Crop the Gemini composite PNG into 6 standalone files (3 logo variants + 3 mockups)
2. Run Recraft Stage 3 on the 3 logo PNGs (primary, mono white, mono black)
3. Clean SVG paths in Illustrator/Figma
4. Commit final files to `03_logo/`

**Track B — execute stage variants (~80 min, parallelizable across the 4 stages):**
1. Open `03_logo/variants.md`
2. Run each stage's Ideogram prompt → pick → run Gemini variation prompt → run Recraft if SVG needed
3. Save outputs to `03_logo/stage-variants/0[1-4]-[stage-name]/`

**Track C — gather Node 4 inputs in parallel:**
4. Source 2 venue photos (mandatory for Node 4 hero)

When Tracks A + C are done → I execute Node 4 — Hero (prompts manifest for Gemini).
After Node 4 → Identity Checkpoint runs (checklist already armed in `00_meta/identity-checkpoint.md`).

## Recent activity log

- 2026-04-25 (morning): Node 1 brief captured.
- 2026-04-25 (later): Node 2 — Crudo recommended.
- 2026-04-25 (later): Node 2 — Crudo APPROVED. Node 3 master prompts generated.
- 2026-04-25 (later): Carlos completed Ideogram + Gemini for master. Provided 4 stage names + themes.
- 2026-04-25 (later): Stage variants populated in `variants.md`. WCAG verified. Identity Checkpoint pre-flight armed.
