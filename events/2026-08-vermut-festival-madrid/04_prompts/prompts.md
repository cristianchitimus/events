# Node 4 — Hero / Key Visual Prompts

**Direction:** Crudo (locked)
**Tool:** Gemini (Nano Banana 2 image model) — gemini.google.com
**Status:** AWAITING_MANUAL_GENERATION
**After completion:** Identity Checkpoint activates automatically (`00_meta/identity-checkpoint.md`)

---

## Setup — what Carlos uploads to Gemini

In a single Gemini chat session, upload **10 images** in this exact order:

| Slot | Image | Source |
|---|---|---|
| 1 | **Mercado de San Fernando interior** — working market, real azulejos + wrought iron + stalls visible | From your Downloads |
| 2 | **Plaza de Lavapiés exterior** — daytime crowd, real neighborhood character | From your Downloads |
| 3 | Pinterest: "harsh flash photography street style Madrid" | From moodboard slot 3 |
| 4 | Pinterest: "brutalist Spanish editorial poster 2020s" | Slot 4 |
| 5 | Pinterest: "big numerals graphic design poster" | Slot 5 |
| 6 | Pinterest: "post-internet rave flyer red yellow" | Slot 6 |
| 7 | Pinterest: "zine layout photocopy texture" | Slot 7 |
| 8 | Pinterest: "Archivo Black layout poster" | Slot 8 |
| 9 | Pinterest: "Spanish independent magazine design 2020s" | Slot 9 |
| 10 | Unsplash/Flickr: "Madrid Lavapiés street night flash" | Slot 10 |

**Critical:** slots 1 and 2 are the *real* venue. Gemini will use them as the primary spatial reference. The other 8 slots define stylistic register.

If you only have a few moodboard images ready, slots 1 + 2 + at least 4 stylistic refs (slots 3, 4, 6, 10 are highest priority) is the minimum acceptable upload.

---

## Stage 1 — 16:9 hero generation (paste into Gemini with all 10 images uploaded)

```
I'm designing brand visuals for "VERMUT FESTIVAL MADRID — 4ª Edición", a
multi-day urban food and music festival running 22–24 August 2026 at the
venue described in the first 2 images I uploaded.

Brand direction (locked):
- Stance: Subversion — tactical pivot. The venue stays VISIBLE in the
  photography, but the brand layer treats it harshly, not preciously.
- Palette (5-color, must drive the image):
   • Rojo Crudo #E5261C (hot scarlet, primary — internet-loud, not earthy)
   • Cian Pavimento #00B5D8 (aggressive cyan, secondary)
   • Amarillo Sirena #F2E63C (siren yellow, accent — used sparingly)
   • Periódico #F2EEE6 (newsprint off-white, light)
   • Negro Mercado #131211 (warm near-black, dark — never pure black)
- Mood: raw, loud, irreverent, immediate, unsanitized.
- Visual motifs: (1) blown-out on-camera flash photography of the venue
  with overexposed highlights on tilework, slight motion blur, harsh
  shadows; (2) real human presence — hands, faces, crowd; (3) the market's
  azulejos and wrought iron must be visible as recognizable elements, not
  abstracted away.
- Typography feel (context only — DO NOT render any text in these images):
  brutal chunky display sans-serif (Archivo Black aesthetic). No script,
  no calligraphy, no decorative serifs.

Venue context (CRITICAL):
- The first 2 images I uploaded are real photos of the actual venue:
  Mercado de San Fernando interior (1940s working market, azulejos,
  wrought iron, food stalls) and Plaza de Lavapiés exterior (multicultural
  Madrid neighborhood plaza). The hero MUST feel like it belongs in those
  specific spaces, not a generic version of "Madrid market".

Audience context:
- 22-35 year-old Madrileños, TikTok-native, mainstream-pro creative
  consumers. They post heavily, expect contemporary internet-coded visual
  energy. The hero must read instantly at thumbnail size on a phone feed.

Generate FOUR distinct hero candidates, each taking a different
compositional approach. All four must share the Crudo treatment (harsh
flash, internet-loud color cast, contemporary photography style).

CANDIDATE A — "INTIMATE" (hands + vermut + market)
Close-to-medium shot of a pair of hands holding a vermut glass in front
of the Mercado de San Fernando azulejos (visible behind, slightly out of
focus but recognizable). Direct on-camera flash, blown highlights on the
tilework, slight motion. The hand and glass occupy the right third of
the frame; upper-left is empty for title overlay.

CANDIDATE B — "SOCIAL" (crowd + dual-zone venue)
Wide shot capturing crowd flow between the market interior and the plaza
exterior — a face or two looking toward camera in the right third, the
market entrance with its azulejo signage visible behind, evening light
mixed with on-camera flash. Motion in the crowd. Upper-left empty.

CANDIDATE C — "ARCHITECTURE-FIRST" (venue as protagonist)
Lower-angle shot looking up at the wrought-iron market structure with
azulejos in frame. A single human element (a silhouette, a pair of legs,
a food stall vendor's torso) anchored in the right third. Harsh flash
treatment, halftone-style print texture overlay implied, very graphic.

CANDIDATE D — "MADRUGADA NIGHT" (Plaza de Lavapiés exterior, after-dark)
Plaza de Lavapiés exterior at night. LED stage lights visible in
background but NOT readable as text. Crowd silhouettes against the LED
glow. On-camera flash hits the foreground subject (a face, a hand
holding a drink) in the right third. Mixed light sources, motion. Upper-
left clear.

For ALL FOUR candidates:
- 16:9 aspect ratio
- Composition that respects the venue's real geometry — DO NOT invent
  architectural details that aren't in the reference photos
- Subject positioned in the right third; upper-left clear of focal
  elements (this is where headline overlay will go at Node 5)
- Lower-right or lower-third should also have breathing room (CTA
  placement at Node 5)
- Editorial photography quality — feels like a contemporary Spanish
  independent magazine cover, not a stock photo
- ABSOLUTELY NO text, NO logos, NO watermarks, NO graphic overlays in
  the image itself — these are pure photographic backgrounds that text
  will be added to later
- The Crudo palette colors should manifest in the image's tonal cast
  (harsh red highlights, cyan shadow tints, yellow flash bounce) — not
  as overlays or filters, but as if the lighting and palette of the
  scene happened to match

AVOID: wood-burning vintage typography, mustard yellow saturation,
terracotta, burnt umber, warm earth tones, sepia photography, golden
hour soft light, shallow depth-of-field bokeh, hand-drawn floral
borders, rustic charm filter, Lightroom warm-faded preset, farmer's
market poster aesthetic, chalkboard menu lettering, hand-drawn folk
illustration, abstract female figures, Etsy illustration aesthetic,
tarot illustration, rounded corner UI, soft gradients, friendly mascot,
SaaS visual language, sanitized corporate photography, vermut glass
icon as graphic, wine bottle illustration, grape clusters, music notes,
microphones, guitars, drone shot, aerial view, architecture-only empty
shot, generic street photography unrelated to Madrid, generic European
market shots, stock photography aesthetic, AI-clean perfect skin, AI-
clean perfect lighting, lens flare, bokeh, tilt-shift, vignette, fake
film grain.
```

---

## Selection criteria (Carlos picking 1 of 4)

✅ **Look for:**
- The venue is recognizably Mercado de San Fernando / Plaza de Lavapiés — not generic
- Azulejos or wrought iron are actually visible in the frame (Candidates A, B, C)
- The flash/lighting feels harsh and contemporary, not soft or pretty
- Upper-left is genuinely clear (test: imagine 6-word headline in Archivo Black there — does it fit?)
- A human element is present, however small — fully unpopulated frames feel cold for a mainstream-pro audience
- The colors in the image already lean toward the Crudo palette without needing post-processing

❌ **Reject:**
- Any candidate where the venue could be "anywhere in Spain" — too generic
- Any candidate with golden-hour / soft-light cast (anti-style)
- Any candidate where text overlay placement would clash with focal elements
- Any candidate with rendered text, hands holding signs, visible logos
- Any candidate with AI-tells: too-perfect skin, too-clean lighting, identical crowd faces, melted hand fingers, surreal architectural impossibilities
- Any candidate that reads "vintage" or "heritage tourism" — the entire point is to break from that

If 0 of 4 candidates pass: re-run the prompt with stronger venue-specificity instructions ("The market in slot 1 has X distinctive feature — the hero must show that feature").

If 2+ candidates pass: pick the one that best supports headline + CTA placement. Save the others as alternates in `04_hero/alternates/` — they may become useful for banner variants at Node 5.

---

## Stage 2 — 9:16 vertical (after picking 16:9 winner)

In the same Gemini chat thread, after picking, paste:

```
Using the 16:9 hero I just selected (Candidate [A/B/C/D]) as exact
reference, regenerate the same scene in 9:16 vertical aspect ratio.

Maintain:
- Same subject, same lighting, same color cast, same venue elements
- Same Crudo treatment — harsh flash, internet-loud color, contemporary
  photography quality
- Subject anchored in lower-third (NOT right-third — the vertical
  composition shifts to lower-third for stories/Reels framing)
- Upper-half clear for vertical title overlay
- ABSOLUTELY NO text, NO logos, NO watermarks

The 9:16 must feel like it was shot at the same moment and place as the
16:9 — it's the same hero in vertical framing, not a different image.

AVOID: [same anti-style block as Stage 1].
```

---

## Files expected in `04_hero/` after Node 4 completes

```
04_hero/
├── prompts.md                ← THIS FILE (committed now)
├── hero-16-9.png             ← Stage 1 winner (Carlos generates and crops to 16:9)
├── hero-9-16.png             ← Stage 2 output (Carlos generates from 16:9 winner)
├── alternates/
│   ├── candidate-a-16-9.png  ← optional, only if you want to keep alternates
│   ├── candidate-b-16-9.png
│   ├── candidate-c-16-9.png
│   └── candidate-d-16-9.png
└── source/
    └── all-four-candidates-composite.png  ← the 4-up Gemini grid for audit trail
```

---

## Time estimate for Carlos

| Step | Time |
|---|---|
| Upload 10 moodboard images | 5 min |
| Stage 1 — generate 4 candidates | 3–5 min (Gemini is fast) |
| Review + pick 1 | 5–10 min |
| Stage 2 — generate 9:16 from winner | 2–3 min |
| Crop + export PNGs at correct dimensions | 5 min |
| **Total Node 4** | **~20–30 min** |

If Gemini under-delivers (all 4 feel generic / off-brand) — re-prompt with venue-specific anchors from your real venue photos before regenerating. Don't accept a soft hero.

---

## What happens after Node 4

1. Carlos commits `hero-16-9.png` and `hero-9-16.png` to `04_hero/`
2. **Identity Checkpoint activates** — Carlos opens `00_meta/identity-checkpoint.md`, fills in the 8-question checklist, sends Claude the verdict
3. If pass → Node 5 (Banners) executes
4. If fail → cascade rework based on which test failed (Test 1 = upstream rework at Node 1/2/4; Test 2 = compositional reprompt of Node 4 only)

Do NOT proceed to Node 5 until the checkpoint passes. This is the only mandatory gate in the canvas.
