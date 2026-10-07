# TailWag — Puppy Food Quiz Brochure

A one-page marketing brochure with an interactive 6-question quiz that recommends a puppy food recipe. Visual direction is taken from the "Tourvia" travel reference: full-bleed photo hero, a giant translucent brand word sitting *behind* the subject, pill-shaped UI, clean sans-serif hierarchy.

---

## 1. Visual system

### Colour
| Token | Hex | Use |
|---|---|---|
| Ink | `#0E1A2E` | Headlines, body text, selected chips, result card background |
| Muted | `#5B6575` | Card tags, helper text, progress label |
| Page ground | `#DCE4EF` | Outer page background (cool blue-grey) |
| Card | `#F4F7FB` | Question card fill |
| Card line | `#E1E7F0` | Question card border |
| Chip line | `#C9D3E0` | Unselected chip / input border |
| Path | `#9AA8BC` | Dotted connector lines and arrowheads |
| Paw | `#C3CDDB` | Paw prints on the bend of the path |
| Accent | `#2F6BFF` | Arrow circles on CTAs, question numbers, progress bar |
| White | `#FFFFFF` | Section backgrounds, primary pill buttons |
| Hero word | `rgba(225,238,252,0.62)` | Giant "TAILWAG" over the sky |

### Type
- **Font:** Plus Jakarta Sans (Google Fonts), weights 400 / 500 / 600 / 700.
- **Hero word:** 236px, weight 600, letter-spacing −0.03em, line-height 1.
- **H1:** 58px, weight 500, line-height 1.08, letter-spacing −0.025em.
- **H2 (section statement):** 44px, weight 500, centred, line-height 1.18.
- **Card question:** 23px, weight 600.
- **Result product name:** 40px, weight 500.
- **Body / UI:** 13–16px, weight 500.
- **Case:** Title Case for headlines and buttons (matches the reference).

### Shape & components
- Section corners: 28px. Question cards: 24px. Info card: 20px.
- **Pill buttons:** white pill + 40px accent circle holding a ↗ arrow (`Start The Quiz`, `Add To Cart`).
- **Ghost pill:** 1px translucent white border (`Retake Quiz`, nav CTA).
- **Eyebrow pill:** outlined pill with a short dash before the label (`— How It Works`).
- **Chips:** 44px min height, outlined; selected = Ink fill with white text.
- No drop shadows; depth comes from photography and the dark hero fade.

---

## 2. Layout & copy

### Hero (full-bleed photo, 760px tall)
Layer order, back to front:
1. Meadow photo of the golden retriever puppy (cover).
2. Giant word **TAILWAG**, centred, top 112px.
3. Background-removed cutout of the same puppy, aligned to the photo, so his head overlaps the word.
4. Bottom dark fade (transparent → `#0B1220`, 340px) for text legibility.

- **Nav:** `TailWag.` logo · centred pill nav: **Food Quiz** (active) · Shop · Recipes · Our Vets · Contact · right CTA: **Shop Food ↗**
- **Bottom-left:**
  - Eyebrow: *Puppy Food Quiz*
  - H1: **Find The Perfect Food For Your New Puppy**
  - Button: **Start The Quiz ↗**
- **Bottom-right info card:** photo of the puppy eating from a white bowl · **6 questions · 2 minutes** · *Vet-formulated recipes matched to your pup*

### How it works + quiz (white section)
- Eyebrow: *How It Works*
- H2: **Six Questions About Your Puppy. One Recipe Made For Exactly Who They Are.**
- Progress: "X of 6 answered" with a thin accent bar.

**The path (backward S):** row 1 runs left → right (1 → 2 → 3), a dotted bend with paw prints curves down the right side, row 2 runs right → left (4 → 5 → 6), then a dotted arrow drops from card 6 into the result.

| # | Tag | Question | Answers |
|---|---|---|---|
| 01 | The Basics | What's your puppy's name? | Text input (default "Biscuit") |
| 02 | Age | How old is {name}? | Under 3 months · 3–6 months · 6–12 months |
| 03 | Size | How big will {name} grow? | Toy · Small · Medium · Large · Giant |
| 04 | Energy | How active is {name}? | Calm · Playful · Very active |
| 05 | Digestion | Any tummy sensitivities? | None · Sensitive · Allergies · Not sure |
| 06 | Taste | How does {name} like to eat? | Crunchy · Soft · Mix it up |

### Result card (navy)
- Photo: puppy lying beside the navy food bag.
- Eyebrow: *{name}'s Perfect Match*
- Product: **{Small / Medium / Large} Breed Puppy Recipe, Chicken & Brown Rice**
- Perk chips (driven by answers):
  - Size → *Mini kibble for small jaws* / *Balanced for steady growth* / *Joint support for big growers*
  - Energy → *Extra protein for active pups* (Very active) or *DHA for brain development*
  - Tummy → *No artificial fillers* (None) or *Gentle on sensitive tummies*
  - Taste → *Crunchy kibble* / *Soft-baked bites* / *Kibble + wet topper*
- Price: **$42 / bag**
- Buttons: **Add To Cart ↗** · **Retake Quiz**

### Footer
*TailWag. · Recipes formulated with veterinary nutritionists [CREDENTIAL]* · *Questions? Ask a TailWag vet — [CONTACT]*

---

## 3. Behaviour
- Typing a name updates every question, the result eyebrow, live.
- Selecting a chip updates the progress bar, product name and perk chips.
- **Retake Quiz** clears answers 2–6 (keeps the name) and scrolls back to the quiz.
- **Responsive:** below 1000px the path stacks into a single column (arrows and bend hidden), the nav pill and info card hide, and the result card stacks vertically. Below 600px the hero shortens to 640px.

## 4. Imagery
| Slot | Image |
|---|---|
| Hero | Golden retriever puppy sitting in a meadow, low angle, deep blue sky with headroom above |
| Hero cutout | Same photo, background removed, layered over the hero word |
| Info card | Puppy eating kibble from a white ceramic bowl on an oak floor |
| Result card | Puppy lying beside a plain navy kraft-paper food bag on a grey backdrop |

## 5. Placeholders to fill
- `[CREDENTIAL]` — vet / nutritionist credential line
- `[CONTACT]` — vet contact method
