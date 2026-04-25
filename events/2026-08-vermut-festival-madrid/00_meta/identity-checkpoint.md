# Identity Checkpoint — Pre-flight Checklist

**Status:** ARMED — runs after Node 4 hero is generated and committed.
**Mandatory:** never bypass. Never auto-progress from Node 4 to Node 5 without explicit pass on this checkpoint.

This file is the fillable form. Once Node 4 outputs (hero 16:9 + 9:16) are in place, Carlos opens this file and fills in the answers. Claude reads it back, applies the decision tree, and either green-lights Node 5 or routes to a Node 1/2/4 rework.

---

## Prerequisites — must all be ✅ before checkpoint runs

- [ ] **Logo SVG** — `03_logo/logo-primary.svg` (vectorized) ✅ when present
- [ ] **Logo dark mode** — `03_logo/logo-darkmode.png` or `.svg`
- [ ] **Hero 16:9** — `04_hero/hero-16-9.png`
- [ ] **Hero 9:16** — `04_hero/hero-9-16.png`
- [ ] **Direction sheet** — `02_direction/direction-CHOSEN.md` (already in place — Crudo, locked)

If any prerequisite is missing, do not proceed. Generate the missing artifact first.

---

## Setup — view artifacts side-by-side

Open in one viewing context (Figma file, single browser tab with all images, split-screen mockup tool):

1. Master logo (primary + dark mode + monochrome variants)
2. Hero 16:9 with logo overlaid in upper-left at intended display size
3. Hero 9:16 with logo overlaid in lower-third at intended display size
4. Crudo palette swatches and motif samples from `direction-CHOSEN.md`

Do **not** review them sequentially in different windows. The whole point of the checkpoint is the side-by-side relational read.

---

## Test 1 — Coherence (3 questions)

Looking at all artifacts together, answer each question. Be honest — a "no" here is much cheaper to fix than a "no" caught at Node 8.

### Q1.1 — Same world?

> Could these visuals plausibly come from the same event? If the logo feels premium-formal but the hero feels casual-playful, you have a stance mismatch.

**Carlos's answer:** [ ] Yes  [ ] No  [ ] Almost — note:

If No → fix at **Node 2** (regenerate direction with stricter Subversion stance). If Almost → tighten Node 4 hero prompt with stance-specific instructions.

---

### Q1.2 — Same room?

> Does the hero look like it belongs in YOUR venue (Mercado de San Fernando interior + Plaza de Lavapiés exterior), or does it look like a generic version of "Madrid market festival"?

**Carlos's answer:** [ ] Yes  [ ] No  [ ] Almost — note:

If No → moodboard slots 1-2 weren't strong enough. Fix at **Node 2 moodboard** with stronger venue photos (specifically: actual interior of Mercado de San Fernando showing real azulejos and wrought iron + actual Plaza de Lavapiés exterior with real architecture, not stock).

---

### Q1.3 — Same audience?

> Imagine your actual audience — 22-35 year-old TikTok-native Madrileños, mainstream-pro creative consumers — walking into the venue and seeing the hero projected on the LED at the entrance. Do they feel addressed, or does it feel aimed at someone else (older, more elite, more touristy)?

**Carlos's answer:** [ ] Yes  [ ] No  [ ] Almost — note:

If No → audience fields in Node 1 weren't specific enough. Regenerate Node 1, then cascade Node 2, 3, 4. (This is the most expensive failure mode — rare if Node 1 was solid, which it was here.)

---

## Test 2 — Commercial Intent (5 questions)

Coherence isn't enough. Imagine the hero as a paid Instagram or TikTok ad in someone's feed.

### Q2.1 — Clarity in 1 second

> Can someone tell what this is and who it's for at a one-second glance? Test: scroll past the image at scrolling speed; what do you remember?

**Carlos's answer:** [ ] Yes  [ ] No  — note:

### Q2.2 — Hierarchy

> Is there a clear visual path — what reads first, second, third? Or does everything shout at the same volume?

**Carlos's answer:** [ ] Clear hierarchy  [ ] Everything competes  — note:

### Q2.3 — Trust cues

> Does the design feel intentional (generous spacing, restraint, consistency) or improvised (mixed systems, busy)? Note: Crudo's brand stance is "deliberately raw," so "improvised-feeling" is correct as long as it's *consistently* improvised — controlled rawness, not actual sloppiness.

**Carlos's answer:** [ ] Intentional rawness  [ ] Sloppy rawness  — note:

### Q2.4 — Proof cues

> Does the design suggest "this team has done this before"? Portfolio-grade polish? If the hero feels like a first attempt, the event feels like a first attempt — even though this is the 4ª edición.

**Carlos's answer:** [ ] Confident  [ ] First-attempt-feeling  — note:

### Q2.5 — Direction (composition setup for Node 5)

> Does the hero composition leave clear room for a headline overlay (upper-left preferred for 16:9) and a CTA placement (lower-right or lower-third)? Strong composition points the viewer toward where text will live at Node 5.

**Carlos's answer:** [ ] Clear empty zones for type  [ ] Hero competes with type  — note:

---

## Decision tree (apply after answering all 8)

### All 8 = Yes / Pass
✅ **Brand is coherent and commercial. Proceed to Node 5.**
- Update status: `Identity Checkpoint` → `COMPLETE`
- Commit: `chore(checkpoint): Identity Checkpoint passed for Vermut Festival Madrid 2026, proceeding to Node 5`
- Next: execute Node 5 — Banners (copy in castizo Spanish + reformatting prompts)

### Test 1 fails (any of Q1.1, Q1.2, Q1.3 = No)
⚠ **Fix is upstream. Cascade rework needed.**
- Q1.1 fail → regenerate Node 2 (stance mismatch)
- Q1.2 fail → regenerate Node 2 moodboard (missing venue photos), then re-run Node 4
- Q1.3 fail → regenerate Node 1 (audience too vague), then cascade Node 2, 3, 4
- Update status: mark failing upstream node `NEEDS_REWORK`

### Test 1 passes but Test 2 fails
⚠ **Brand is coherent but not commercial. Composition fix only.**
- Re-prompt Node 4 with stronger composition guidance:
  - Subject right-third for 16:9
  - More negative space upper-left
  - Stronger focal hierarchy
- Mark Node 4 `IN_PROGRESS` again, regenerate hero
- Re-run this checkpoint
- Do NOT regenerate Node 1, 2, or 3

### Mixed verdict (mostly pass, 1-2 borderline "Almost")
⚠ **Judgment call.**
- If borderline questions are in Test 2 → minor Node 4 reprompt usually fixes it
- If borderline questions are in Test 1 → take the cost and rework upstream; the checkpoint failure pattern says "almost" usually becomes "definitely no" once it ships at scale

---

## Common Crudo-specific failure patterns to watch for

These are pattern-matched from the failure modes in the canvas docs, applied to our specific Subversion direction:

### "Hero is loud but feels generic-edgy, not Lavapiés"
→ Q1.2 fail. The flash photography came out as generic editorial flash, not specifically Madrid market flash. Fix: Node 4 reprompt with explicit Mercado de San Fernando azulejo + ironwork references AND real moodboard slot 1-2 venue photos.

### "Logo and hero look brutal in different ways"
→ Q1.1 fail. The logo went brutalist-typographic and the hero went brutalist-photographic but they don't speak to each other. Fix: Node 4 reprompt asking the hero to *include type elements* so it bridges to the logo's language. NOT a Node 2 regeneration.

### "Looks like a club flyer, not a festival"
→ Q1.3 fail. The Subversion went too far past tactical pivot into full break. Fix: Node 4 reprompt with explicit "include venue photography prominently in frame, treat it harshly but make sure it reads as the Mercado de San Fernando, not as a generic warehouse rave."

### "Beautiful but cold"
→ Q2.1 + Q2.3 fail. The brand is technically correct but lacks warmth/humanity. Fix: Node 4 reprompt to include human subjects (hands holding vermut, faces in the crowd) instead of just venue architecture.

---

## Sign-off block (fill in when checkpoint passes)

**Checkpoint result:** [ ] PASSED   [ ] FAILED — rework needed
**Date completed:**
**Carlos signature/initials:**
**Notes:**

---

## When this checklist activates

- After Carlos commits Node 4 hero outputs (`hero-16-9.png` + `hero-9-16.png`) to the repo
- Before any Node 5 work begins
- Carlos opens this file, fills in the 8 answers, then sends them to Claude (or just the verdict block) — Claude applies the decision tree
