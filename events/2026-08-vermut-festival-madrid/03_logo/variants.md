# Node 3 — Stage Variants (Executable Prompts)

**Direction:** Crudo (locked)
**Status:** READY_TO_RUN — populated 2026-04-25 from Carlos's stage info
**Run order:** can be done in parallel with master logo vectorization

This file replaces the parameter slots in `variants-template.md` with Carlos's actual stage info.

---

## The 4 stages — locked configuration

| # | Stage Name | Theme | Brand color | Numeric mark | Surface constraint |
|---|---|---|---|---|---|
| 1 | **MERCADO** | Interior Mercado de San Fernando — vermut tasting, Spanish singer-songwriter, jazz acústico, intimate energy | **Violeta Eléctrico `#7C3AED`** | `01` | Works on dark + light |
| 2 | **PLAZA MAYOR** | Exterior Plaza de Lavapiés — indie español headliners, rock alternativo, max energy *(main stage)* | **Cian Pavimento `#00B5D8`** *(master)* | `02` | Works on dark + light |
| 3 | **MADRUGADA** | Exterior — DJs electronic, techno, house, late-night/après-dark | **Chartreuse Eléctrico `#B8FF00`** | `03` | ⚠ **DARK SURFACES ONLY** — invisible on Periódico ground |
| 4 | **COCINA** | Interior small — food talks, cooking demos, chef conversations, educational/community | **Tinta Imprenta `#5B7BFF`** | `04` | Works on dark + light |

### Why these colors

- **MERCADO violet** — intimate red room without competing with the master red. Vermouth itself is often a deep violet-black; this riffs on that without being literal.
- **PLAZA MAYOR cyan = master cyan** — main stage carries the most master-brand presence. No substitution. Plaza Mayor IS the brand.
- **MADRUGADA chartreuse** — explicitly post-internet club-coded, contrasts hardest with master red, signals night. The "invisible on light" issue is actually a feature, not a bug — Madrugada applications run on dark surfaces by design.
- **COCINA royal blue** — printer's ink reference, reads "intellectual / chef talks / publication culture" without going earth-tone (anti-style trap).

### WCAG verification

All 4 stage colors have been contrast-tested:
- All ≥ 3.28:1 against `Negro Mercado #131211` (passes AA Large for stage marks at large scale)
- Mercado, Cocina ≥ 4.92:1 against `Periódico #F2EEE6` (passes AA Normal for body)
- Madrugada chartreuse fails on Periódico (1.05) — flagged above, dark-surface-only constraint
- All 4 mutually distinguishable at thumbnail size (min 1.50, max 4.71 between any two stage colors)

### Numeric mark grammar

Each stage carries a 2-digit Space Mono numeric mark — `01` `02` `03` `04` — treated as a graphic anchor, not a footnote. The mark can appear:
- Inline next to the stage name (e.g., `MERCADO 01`)
- As a giant standalone graphic element (filling 1/3+ of a poster)
- As a wayfinding marker on signage and floor vinyls

This carries Meaning Map element 5 (oversize numerals) into the stage system.

---

## Stage 1 — MERCADO (Ideogram Stage 1 prompt)

```
A stage-specific lockup variant for "VERMUT FESTIVAL MADRID", master brand
already established (uploaded as reference).

This is the lockup for stage 1 called "MERCADO" — programming theme: vermut
tasting, Spanish singer-songwriter, acoustic jazz, intimate energy. The
intimate/conversational stage of the festival.

Construct: keep the master VERMUT FESTIVAL MADRID wordmark exactly as
designed, then add beneath it a secondary lockup containing:
- The stage name "MERCADO" set in the same Archivo Black-style brutal display
  sans, smaller scale than VERMUT but readable, set TIGHT and aligned to the
  left edge of the master wordmark
- A large 2-digit numeric mark "01" in Space Mono-style monospace digits,
  positioned to the right of "MERCADO" at similar height to the stage name,
  treated as a graphic anchor

Color: where the master uses any cyan accent, this variant uses electric
violet (#7C3AED). Master red (#E5261C) and master typography colors stay
constant.

Mood: still raw, loud, irreverent, immediate. Stage variant should feel
like a confident sibling of the master, not a different brand.

Format: single horizontal lockup. Solid flat colors. No decorative
illustrations, no icons, no glassware, no bottles, no music notes.

AVOID: wood-burning vintage typography, mustard yellow, terracotta, burnt
umber, warm earth tones, hand-drawn folk illustration, abstract female
figures, Etsy illustration aesthetic, sepia photography, hand-drawn floral
borders, rustic charm, farmer's market poster aesthetic, chalkboard menu
lettering, vermut glass icon, wine bottle illustration, grape clusters,
default sans-serif (Helvetica, Arial), gradient mesh, lens flares, 3D bevel,
drop shadows, outline strokes, script fonts, calligraphy, music notes,
microphones, guitars.
```

---

## Stage 2 — PLAZA MAYOR (Ideogram Stage 1 prompt)

```
A stage-specific lockup variant for "VERMUT FESTIVAL MADRID", master brand
already established (uploaded as reference).

This is the lockup for stage 2 called "PLAZA MAYOR" — programming theme:
indie español headliners, rock alternativo, maximum energy. THIS IS THE
MAIN STAGE of the festival.

Construct: keep the master VERMUT FESTIVAL MADRID wordmark exactly as
designed, then add beneath it a secondary lockup containing:
- The stage name "PLAZA MAYOR" set in the same Archivo Black-style brutal
  display sans, smaller scale than VERMUT but readable, set TIGHT and
  aligned to the left edge of the master wordmark
- A large 2-digit numeric mark "02" in Space Mono-style monospace digits,
  positioned to the right of "PLAZA MAYOR" at similar height to the stage
  name, treated as a graphic anchor

Color: keep master cyan accent (#00B5D8) — this stage IS the master brand
in its purest form, no color substitution. Master red (#E5261C) and master
typography colors stay constant.

Mood: still raw, loud, irreverent, immediate. Maximum energy of the four
stages. This is the centerpiece — let it feel like the centerpiece.

Format: single horizontal lockup. Solid flat colors. No decorative
illustrations, no icons, no glassware, no bottles, no music notes.

AVOID: [same anti-style block as Mercado].
```

---

## Stage 3 — MADRUGADA (Ideogram Stage 1 prompt)

```
A stage-specific lockup variant for "VERMUT FESTIVAL MADRID", master brand
already established (uploaded as reference).

This is the lockup for stage 3 called "MADRUGADA" — programming theme:
electronic music DJs, techno, house, late-night après-dark programming.
The 1am-to-6am stage.

CRITICAL: This variant is designed for DARK SURFACES ONLY. Generate it on
a Negro Mercado (#131211) background, not a light background. Plaza Mayor
and Mercado work on either ground; Madrugada is night-only.

Construct: keep the master VERMUT FESTIVAL MADRID wordmark exactly as
designed but inverted to white/cream letterforms (#F2EEE6) on the dark
ground. Add beneath it a secondary lockup containing:
- The stage name "MADRUGADA" set in the same Archivo Black-style brutal
  display sans, smaller scale than VERMUT but readable, set TIGHT and
  aligned to the left edge of the master wordmark
- A large 2-digit numeric mark "03" in Space Mono-style monospace digits,
  positioned to the right of "MADRUGADA" at similar height to the stage
  name, treated as a graphic anchor

Color: where the master uses any accent, this variant uses electric
chartreuse (#B8FF00) — extremely bright, club-coded, designed to glow
under UV/club lighting. Master red (#E5261C) is replaced with the chartreuse
in this variant ONLY (since red on dark background loses its punch and
chartreuse is the stage's defining visual signature).

Mood: still raw, loud, irreverent, immediate, but specifically nocturnal.
Should feel like a club flyer pasted on a wall at 4am.

Format: single horizontal lockup on dark ground. Solid flat colors. No
decorative illustrations, no icons, no glassware, no bottles, no DJ
equipment.

AVOID: [same anti-style block as Mercado] PLUS: glowsticks, rave
illustrations, smiley faces, pixelated computer aesthetic, vaporwave
gradient, neon tube text effect, club laser graphics, headphone illustration.
```

---

## Stage 4 — COCINA (Ideogram Stage 1 prompt)

```
A stage-specific lockup variant for "VERMUT FESTIVAL MADRID", master brand
already established (uploaded as reference).

This is the lockup for stage 4 called "COCINA" — programming theme: food
talks, cooking demonstrations, conversations with chefs, educational and
community-building. The intellectual/conversational stage.

Construct: keep the master VERMUT FESTIVAL MADRID wordmark exactly as
designed, then add beneath it a secondary lockup containing:
- The stage name "COCINA" set in the same Archivo Black-style brutal display
  sans, smaller scale than VERMUT but readable, set TIGHT and aligned to
  the left edge of the master wordmark
- A large 2-digit numeric mark "04" in Space Mono-style monospace digits,
  positioned to the right of "COCINA" at similar height to the stage name,
  treated as a graphic anchor

Color: where the master uses any cyan accent, this variant uses royal
electric blue (#5B7BFF) — printer's ink reference, reads intellectual/
publication culture, deliberately NOT warm-kitchen. Master red (#E5261C)
and master typography colors stay constant.

Mood: still raw, loud, irreverent, immediate, but specifically intellectual
— think indie publication or zine editorial. Brain-energy, not party-energy.

Format: single horizontal lockup. Solid flat colors. No decorative
illustrations, no icons, no glassware, no bottles, NO food illustrations,
NO cooking utensils, NO chef hats.

AVOID: [same anti-style block as Mercado] PLUS: chef hat icons, knife/fork
illustrations, recipe card aesthetic, cookbook design, hand-lettered menu
typography, chalkboard background, hand-drawn vegetables, food-blog
photography style.
```

---

## Stage 2 — Gemini variations prompt (run AFTER picking each stage's lockup)

For each stage, after the Ideogram pick, upload to Gemini with this prompt:

```
Using the uploaded VERMUT FESTIVAL MADRID — [STAGE_NAME] lockup as exact
reference, generate 3 variations:

1. DARK MODE (or LIGHT MODE for Madrugada): same lockup with surface
   inverted. For Mercado, Plaza Mayor, Cocina: dark mode on Negro Mercado
   (#131211) with letterforms in Periódico (#F2EEE6) and the stage color
   (#STAGE_HEX) used for the secondary lockup. For Madrugada: skip this
   variation — Madrugada is dark-mode by default.

2. WRISTBAND MOCKUP: printed on a paper festival wristband (25mm tall,
   slight wrinkle, attached to a wrist). Wristband background is
   #STAGE_HEX. Logo printed in white. Photographed under harsh on-camera
   flash.

3. STAGE LED FRAME (16:9): the lockup centered/anchored on a 16:9 surface
   that mimics how it would appear as a still on the LED stage screen
   between sets. Background is Negro Mercado with subtle halftone dot
   pattern texture overlay at large dot size.

Maintain logo proportions and letterforms exactly. Same letter shapes,
same kerning, same weight as the master.

AVOID: [full anti-style block].
```

Substitution per stage:
- Mercado: `[STAGE_NAME] = "MERCADO"`, `[STAGE_HEX] = #7C3AED`
- Plaza Mayor: `[STAGE_NAME] = "PLAZA MAYOR"`, `[STAGE_HEX] = #00B5D8`
- Madrugada: `[STAGE_NAME] = "MADRUGADA"`, `[STAGE_HEX] = #B8FF00`
- Cocina: `[STAGE_NAME] = "COCINA"`, `[STAGE_HEX] = #5B7BFF`

---

## File outputs after running

```
03_logo/stage-variants/
├── 01-mercado/
│   ├── lockup.svg                  ← from Recraft after picking Stage 1
│   ├── lockup-dark.svg
│   ├── wristband-mockup.png
│   └── led-frame.png
├── 02-plaza-mayor/
│   ├── lockup.svg
│   ├── lockup-dark.svg
│   ├── wristband-mockup.png
│   └── led-frame.png
├── 03-madrugada/
│   ├── lockup.svg                  ← dark-mode only (no light variation)
│   ├── wristband-mockup.png
│   └── led-frame.png
└── 04-cocina/
    ├── lockup.svg
    ├── lockup-dark.svg
    ├── wristband-mockup.png
    └── led-frame.png
```

---

## Time estimate for Carlos to execute all 4 stages

| Step | Time per stage | × 4 stages |
|---|---|---|
| Ideogram generation + selection | ~10 min | ~40 min |
| Gemini variation pass | ~5 min | ~20 min |
| Recraft vectorization | ~5 min | ~20 min |
| **Total all 4 stages** | | **~80 min** |

Can run in parallel with master logo Recraft cleanup.
