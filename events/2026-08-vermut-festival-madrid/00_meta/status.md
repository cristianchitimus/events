# Status — Vermut Festival Madrid 2026 (4ª Edición)

**Last updated:** 2026-04-25 by Claude (Node 3 master prompts ready)
**Current phase:** Logo (master prompts ready for execution; stage variants awaiting input)
**Active branch:** `event/2026-08-vermut-festival-madrid`
**Workflow path:** C (artifact fallback — manual push)
**Owner:** Claude (strategist) + Carlos (client)
**Client approver:** Carlos, Festival Vermut Madrid team

## Node progress

| Node | Status | Date | Notes |
|------|--------|------|-------|
| 1 — Brief | AWAITING_PUSH | 2026-04-25 | Captured and refined. |
| 2 — Direction | COMPLETE | 2026-04-25 | **Crudo (Subversion / tactical pivot) APPROVED by Carlos.** |
| 2.5 — Audit | SKIPPED | 2026-04-25 | Carlos opted to proceed direct to Node 3. Can be run later if Node 3 outputs surface tropes that need negative-prompting. |
| 3 — Logo (master) | AWAITING_MANUAL_GENERATION | 2026-04-25 | Prompts ready in `03_logo/prompts.md`. Carlos to run Ideogram → Gemini → Recraft. |
| 3 — Logo (stage variants, Appendix A) | AWAITING_INPUT | 2026-04-25 | Template ready in `03_logo/variants-template.md`. **Needs stage names + themes from Carlos.** |
| 4 — Hero | NOT_STARTED | — | Runs after master logo + at least 2 venue photos available. |
| Identity Checkpoint | NOT_STARTED | — | Mandatory between Node 4 and Node 5. |
| 5 — Banners | NOT_STARTED | — | IG feed/stories + TikTok + web + OOH metro. Castizo Spanish copy. |
| 6 — Video | NOT_STARTED | — | 4 LED stages (Appendix A applies). Per-stage LED dimensions TBD. |
| 7 — Music | NOT_STARTED | — | Atmospheric only, between sets. |
| 8 — Print | NOT_STARTED | — | Wristbands ×3, A4 trifold, A1 carteles, photocall, floor vinyls, signage. |
| 8.5 — Production | NOT_STARTED | — | Spain ISO 216. Imprenta TBD. |
| 9 — Brand Bible | NOT_STARTED | — | Final deadline 2026-07-20. |

## Status legend

- `NOT_STARTED` — Hasn't been touched yet
- `IN_PROGRESS` — Actively being worked on
- `AWAITING_MANUAL_GENERATION` — Prompts ready, user runs external AI tool
- `AWAITING_INPUT` — Waiting on missing config from client (e.g., stage names)
- `AWAITING_REVIEW` — Output ready, user/client reviewing
- `AWAITING_PUSH` — Files generated, user pushes manually (Path C)
- `COMPLETE` — Done, no action needed
- `SKIPPED` — Deliberately bypassed
- `NEEDS_REWORK` — Failed checkpoint, needs upstream regeneration
- `FAILED` — Unrecoverable error

## Open questions / blocking items

**Blocking Node 3 stage variants (Appendix A):**
- ⚠ **The 4 stage names** (short, castizo-friendly preferred — 1-2 syllables ideal)
- ⚠ **Per-stage themes** (1 line each — what kind of programming each stage hosts)
- (Optional) Per-stage preferred colors — if not provided, Claude picks based on themes

**Non-blocking (capture before Node 4 / 6 / 8.5):**
- 2 venue photos (interior of Mercado de San Fernando + Plaza de Lavapiés exterior) — needed for Node 4 hero generation
- Per-stage LED dimensions and aspect ratios (4 screens) — needed for Node 6
- Imprenta provider and special finishes — needed for Node 8.5
- Existing IG hashtag and custom filter references
- Festival IG handle
- Sponsor logo files (Cinzano, Mahou, Estrella Galicia, Lavapiés locals)
- WCAG sign-off (AA recommended baseline)

## Next recommended action

1. **Carlos runs the master logo pipeline** — Ideogram → Gemini → Recraft, ~45–70 min total. Files commit to `03_logo/`.
2. **Carlos provides stage names + themes** in the next message → Claude regenerates `variants-template.md` as executable per-stage prompts.
3. While the master logo is being generated, Carlos can be gathering the 2 venue photos for Node 4.
4. Once master logo is locked, proceed to **Node 4 — Hero**.

## Recent activity log

- 2026-04-25 (morning): Node 1 brief captured.
- 2026-04-25 (later): Node 2 — Crudo recommended.
- 2026-04-25 (later): Node 2 — Crudo APPROVED by Carlos. Node 3 master prompts generated. Stage variants template parameterized, awaiting stage names.
