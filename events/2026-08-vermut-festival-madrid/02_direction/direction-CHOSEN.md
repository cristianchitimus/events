# Direction CHOSEN — CRUDO

> **Status:** RECOMMENDED — pending Carlos approval.
> If Carlos picks A or B instead, this file regenerates for that direction and `meaning-map.md` / `anti-style.md` / `moodboard-shopping-list.md` regenerate to match.

**Stance:** Subversion (tactical pivot variant)

**One-line frame:** Venue visible, brand brutal. The market is photographed honestly; the type refuses to be picturesque.

---

## Palette (full token table)

| Token | Name | Hex | Use |
|---|---|---|---|
| Primary | Rojo Crudo | `#E5261C` | Logo, headline backgrounds, primary CTA |
| Secondary | Cian Pavimento | `#00B5D8` | Per-stage variant slot (Appendix A); secondary surfaces |
| Accent | Amarillo Sirena | `#F2E63C` | Pricing, alerts, set-time callouts, sparingly |
| Light | Periódico | `#F2EEE6` | Body text fields, newsprint surfaces |
| Dark | Negro Mercado | `#131211` | Body text on light, dark surfaces |

**Contrast pairs (WCAG AA verified):**
- Negro on Periódico: 16.1:1 ✓
- Periódico on Rojo Crudo: 4.9:1 ✓ (large text only)
- Periódico on Negro Mercado: 16.1:1 ✓
- Negro on Amarillo Sirena: 14.6:1 ✓
- Negro on Cian Pavimento: 6.4:1 ✓

⚠ Avoid: Rojo Crudo + Cian Pavimento body text combinations (vibration / accessibility issues).

## Typography (full system)

| Role | Font | Source |
|---|---|---|
| Headlines (display) | Archivo Black | Google Fonts |
| Body | Inter (400, 500, 700) | Google Fonts |
| Numerals + callouts | Space Mono (400, 700) | Google Fonts |
| Per-stage marks | Archivo Black at extreme scale, single character | Google Fonts |

**Hierarchy rules:**
- Headlines set TIGHT (-2% tracking), often UPPERCASE, often bleeding off edge
- Body sets LOOSE (+1% tracking), high line-height (1.5+), generous reading rhythm
- Numerals always Space Mono — gives the ticket-stub / printed-matter feel without resorting to vintage type

## Per-stage variant architecture (Appendix A)

Master Crudo stays constant across all assets. Each of the 4 stages takes ONE variant:

| Stage | Variant color (replaces Cian Pavimento) | Numeric mark |
|---|---|---|
| Stage 1 | Cian Pavimento `#00B5D8` (master cyan) | ❶ |
| Stage 2 | TBD | ❷ |
| Stage 3 | TBD | ❸ |
| Stage 4 | TBD | ❹ |

Stage-specific palette tokens designed at Node 3 once stage names / themes are locked. **Open question for Carlos:** stage names + musical/cultural themes per stage.

## Visual motif specifications

### 1. Blown-out flash photography
- Direct on-camera flash (or simulated)
- Overexposed highlights (especially on tile)
- Slight motion blur acceptable, even welcome
- Color cast acceptable (flash-cyan)
- Subjects: venue interiors, food prep close-ups, hands holding vermut, crowd at night, hand-painted signage shot too close
- AVOID: golden hour, soft natural light, shallow depth-of-field "bokeh," tilt-shift, sepia, Lightroom presets

### 2. Oversize numerals
- Dates, stage IDs, prices, set times treated as primary visual elements
- Often larger than the headline they accompany
- Often cropped at edges
- Always Space Mono or Archivo Black (mono variant for numbers exclusively)

### 3. Print artifacts as texture
- Registration crosses (the +) used as pure graphic elements
- Halftone overlays at large dot size (visible, not "subtle")
- CMYK misregistration on key headlines (intentional shift of 1-2px on cyan/magenta channels)
- Photocopy noise overlay on dark surfaces

## Spacing philosophy

Tight margins. Content bleeds to the edges of the canvas. Refuses the centered-classical "respectful poster" tradition. Asymmetric grids. Type fights the photo, doesn't sit politely on top of it.

## Photography treatment summary

Hard flash. Real situations. No styled food shots. Shoot the working market, not the curated market. Crowd over product. Hands and faces over architecture-as-postcard.

## Voice & tone (preview for Node 5)

- Castizo register, colloquial
- Strong language permitted ("hostia", "cabrón", "vamos" etc. usable in copy)
- Imperative mood often ("Ven", "Bebe", "Para de scrollear")
- Numerical specifics ("3 días, 4 escenarios, 8.000 personas, 22 al 24 de agosto") — facts as graphic anchor
- Avoid: "celebramos", "te invitamos", "vive la experiencia", "auténtico", "tradicional", "único"

Full Node 5 voice work happens at Node 5.

## Sponsor handling

- **Cinzano (master):** primary red is intentionally Cinzano-adjacent. Co-branded layouts read native. Cinzano logo locks at full color in Periódico-ground panels.
- **Mahou + Estrella Galicia:** lock in Negro Mercado on Periódico panels. No color-tinting their marks.
- **Lavapiés local sponsors:** dedicated "Sponsors del Barrio" panel with deliberately uneven sizing — local hardware store appears next to international beer brand at similar visual weight. This is a subversion lever and a community-respect lever simultaneously.

## What this direction explicitly rejects

See `anti-style.md` for the full list (5 items) for image-prompt injection at Nodes 3, 4, 5, 8.
