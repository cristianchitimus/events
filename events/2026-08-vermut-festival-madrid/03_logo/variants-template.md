# Node 3 — Stage Variants Template (Appendix A)

**Direction:** Crudo (locked)
**Status:** AWAITING_INPUT — needs stage names + themes from Carlos before generation
**Master logo dependency:** must be locked first (Stage 1 of `prompts.md`)

This template generates the 4 per-stage logo variants once Carlos provides stage names + per-stage musical/cultural themes. Each variant follows the master Crudo system with two substitutions: **one color token** + **one numeric mark**.

---

## What we need from Carlos to populate this template

| Slot | Need | Example |
|---|---|---|
| Stage 1 NAME | Short Spanish/castizo name | e.g., "Tasca", "Plaza", "Solera", "El Foro" |
| Stage 1 THEME | Musical/cultural identity | e.g., "indie español + flamenco fusion" |
| Stage 1 PALETTE COLOR | Hex code substituting Cian Pavimento | e.g., the master cyan, OR a new color |
| Stage 2, 3, 4 | Same |

---

## Stage variant palette assignments (DRAFT — pending input)

The 4 stage colors must:
- Be visually distinguishable from each other at thumbnail size
- All maintain WCAG AA contrast against `Negro Mercado #131211`
- Avoid earth tones, mustards, sepia (anti-style)
- Cohere as a *family* — each stage feels like a sibling of the master, not a different brand

**Default suggestion (Carlos can override):**

| Stage | Suggested color | Hex | Numeric mark | Implied vibe |
|---|---|---|---|---|
| Stage 1 | Cian Pavimento (master) | `#00B5D8` | ❶ | the "main stage" — keeps the master cyan, has the most master-brand presence |
| Stage 2 | Magenta Castiza | `#E91E78` | ❷ | hot, club-coded, after-dark |
| Stage 3 | Verde Veneno | `#3DDC97` | ❸ | acid green, weird/leftfield programming |
| Stage 4 | Naranja Calle | `#FF7A1A` | ❹ | aggressive orange, daytime/streetwear |

These are placeholders. The right colors flow from the actual stage *programming*. Once Carlos sends stage names + themes, I'll re-pick.

---

## Per-stage Ideogram prompt template

(Use AFTER the master logo is locked. Run once per stage with substitutions filled in.)

```
A stage-specific lockup variant for "VERMUT FESTIVAL MADRID", master brand
already established (uploaded as reference).

This is the lockup for stage [X] called "[STAGE_NAME]" — programming theme:
[STAGE_THEME].

Construct: keep the master VERMUT FESTIVAL MADRID wordmark exactly as
designed, but add beneath it (or to the right, lower right corner) a
secondary lockup containing:
- The stage name "[STAGE_NAME]" set in the same Archivo Black-style brutal
  display sans, smaller scale than VERMUT but readable
- A large numeric mark "[NUMERIC]" in Space Mono-style monospace digits,
  treated as a graphic anchor

Color substitution: where the master uses cyan accent (#00B5D8), this
variant uses [STAGE_COLOR_HEX].

Mood: still raw, loud, irreverent, immediate. Stage variant should feel
like a sibling, not a different brand.

Format: single horizontal lockup. Solid flat colors. No decorative
illustrations, no icons, no glassware, no bottles.

AVOID: wood-burning vintage typography, mustard yellow, terracotta, burnt
umber, warm earth tones, hand-drawn folk illustration, abstract female
figures, Etsy illustration aesthetic, sepia photography, hand-drawn floral
borders, rustic charm, farmer's market poster aesthetic, chalkboard menu
lettering, vermut glass icon, wine bottle illustration, grape clusters,
default sans-serif (Helvetica, Arial), gradient mesh, lens flares,
3D bevel, drop shadows, outline strokes, script fonts, calligraphy.
```

### Substitution slots:
- `[X]` → 1, 2, 3, or 4
- `[STAGE_NAME]` → e.g., "TASCA"
- `[STAGE_THEME]` → e.g., "indie español + flamenco fusion"
- `[NUMERIC]` → ❶ ❷ ❸ ❹ (filled circled-number characters), or `01 02 03 04` if circled glyphs render poorly
- `[STAGE_COLOR_HEX]` → e.g., `#00B5D8`

---

## Per-stage Gemini prompt template

(After Carlos picks one variant per stage from Ideogram results.)

```
Using the uploaded stage [X] lockup as reference, generate 3 variations:

1. DARK MODE — same lockup on Negro Mercado (#131211) background, with
   letterforms in Periódico (#F2EEE6).

2. WRISTBAND MOCKUP — printed on a stage-tier paper wristband (25mm tall,
   slight wrinkle, attached to wrist), wristband background color is
   [STAGE_COLOR_HEX]. Logo printed in white. Photographed under harsh
   flash.

3. STAGE LED FRAME (16:9) — the lockup centered/anchored on a 16:9
   surface that mimics how it would appear as a still on the LED stage
   screen during set changes. Background is Negro Mercado with subtle
   halftone dot pattern texture overlay.

Maintain logo proportions exactly. Same letter shapes, same kerning,
same weight as master.

AVOID: [full anti-style list].
```

---

## File outputs after variants are run

```
03_logo/stage-variants/
├── escenario-1-[NAME]/
│   ├── lockup.svg
│   ├── lockup-dark.svg
│   ├── wristband-mockup.png
│   └── led-frame.png
├── escenario-2-[NAME]/...
├── escenario-3-[NAME]/...
└── escenario-4-[NAME]/...
```

(Stage folder names use the actual stage names provided by Carlos.)

---

## When this template gets activated

The instant Carlos provides:
1. The 4 stage names
2. The 4 themes (one line each is fine)
3. (Optional) preferred stage colors — otherwise I'll pick based on themes

I'll fill the substitution slots, regenerate this file as the executable per-stage prompt set, and Carlos can run them in Ideogram + Gemini in parallel with the master logo workflow.
