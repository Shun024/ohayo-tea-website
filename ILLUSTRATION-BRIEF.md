# OHAYO TEA — Custom Illustration Commission Brief
### For Concept 04 “Story / お茶物語” (the misatoto-style scroll experience)

**Prepared for:** the illustrator / studio
**Client:** OHAYO TEA — Shiba-Inu bubble-tea house, 95 Princess Street, Manchester
**Live concept to build on:** https://shun024.github.io/ohayo-tea-website/style-4-story/
**Primary style reference:** https://www.town.shimane-misato.lg.jp/misatoto/  (“misatoto” microsite)
**Existing brand asset:** the hand-drawn “tea-dog” 茶犬 logo (black line-art) — see `assets/logo-shiba.jpg`.

---

## 1. The goal in one line
Replace the placeholder SVG artwork in Concept 04 with a **bespoke, flat-vector illustrated
world** — so OHAYO’s site has the same warmth, craft and “scroll-through-a-storybook” feeling
as misatoto, but is unmistakably OHAYO (the Shiba tea-dog, bubble tea, Manchester).

The **motion is already built** (parallax + scroll-reveal in code). We are commissioning the
**art that rides on top of that motion**, delivered as separated layers so it can move.

---

## 2. Art direction / style
- **Flat vector**, rounded, friendly, slightly hand-made — solid colour shapes, minimal or no
  outlines, gentle organic curves. Warm and calm, not loud or cartoonish.
- **Reference feel:** misatoto’s vegetable/townscape illustrations (soft, editorial, storybook).
- **Texture:** optional subtle grain/paper texture is welcome but keep it light.
- **Mascot:** the OHAYO **Shiba “tea-dog” (茶犬)** is the star. Reinterpret the existing
  line-art logo as a **flat-colour character** (cream/tan fur, blushing cheeks) that can appear
  throughout the world — holding a cup, peeking, waving, sleeping.
- **World:** a gentle Japanese-countryside-meets-Manchester tea landscape — rolling green
  hills, tea bushes, a river, small trees, warm sky, drifting clouds, a rising sun.

## 3. Colour palette (locked — sampled from the reference & OHAYO brand)
| Role | Hex |
|---|---|
| Sand / base | `#efdbcb` |
| Sky top | `#f6e6d3` |
| Paper / highlight | `#fef9f3` |
| Ink (line/type) | `#2d2927` |
| Tea green (dark) | `#32645a` |
| Tea green (light) | `#3f7a6d` |
| Badge purple | `#503278` |
| Peach (accent) | `#ffc8b8` |
| Coral (accent) | `#f15464` |
| Gold (buttons) | `#c48426` |
| Yellow (sun/accents) | `#ffd258` |
| Ochre (accents) | `#d89c52` |
Please work **within this palette** (small tint/shade variations are fine).

Type is handled separately (Noto Sans JP in build; the reference uses Morisawa **Tazugane
Gothic** + **Yakumono**, which the client would license if they want an exact type match — not
part of this illustration brief).

---

## 4. Deliverables — asset register
Each asset below maps to a real slot in the build. **Bold = essential**; the rest are “nice”.

### A. Parallax background — the illustrated landscape  ★ most important
Deliver as **separate, individually-named layers** (each its own SVG/file) so they can be moved
at different speeds. Make each layer **≥ 2400 px wide** and **horizontally seamless/tileable** so
sideways/vertical parallax never reveals an edge.
1. **`bg-sky`** — warm gradient sky + rising **sun** (sun as its own element for slow drift).
2. **`bg-clouds`** — 3–5 separate cloud shapes (each exportable alone; they drift independently).
3. **`bg-hills-far`** — pale distant hills (slowest layer).
4. **`bg-hills-mid`** — mid hills + a winding **river/stream**.
5. **`bg-hills-near`** — foreground hill with **tea bushes, small trees, maybe a torii/lantern
   or a hint of Manchester rooftop** (fastest layer).
6. *(optional)* **`bg-foreground`** — grass/leaves band that sits in front of content edges.

### B. The mascot — OHAYO tea-dog 茶犬  ★
7. **`shiba-hero`** — the star pose (e.g. holding/offering a boba cup), ~800×800, for the hero.
8. `shiba-peek`, `shiba-wave`, `shiba-sip`, `shiba-sleep` — 3–4 extra poses to sprinkle through
   the scenes.
9. **`avatar-sprite`** — a small looping **sprite sheet** of the tea-dog for the round avatar
   button’s hover animation (the reference uses a **9-frame** sheet, 40×40 per frame; deliver
   @2x/@3x too). Simple blink / tail-wag / ear-twitch.

### C. Drink illustrations (flat) — one per signature cup  ★
Portrait ~600×800, transparent, each drink recognisable (colour + toppings + the OHAYO cup with
the tea-dog stamp). These replace the placeholder SVG “spots” beside each story and can also be
used as menu tiles. Needed for:
10. **Brown Sugar Tapioca Milk** (黑糖珍珠鮮奶, tiger-striped)
11. **Matcha Tapioca Milk** (靜岡抹茶珍珠鮮奶)
12. **Super Fruitea** (超級水果茶, fruit slices)
13. **Strawberry Tea · Cheese Foam** (芝芝草莓)
14. **White Peach · Cheese Foam** (芝士白桃)
15. **Strawberry Tapioca Milk** (草莓珍珠鮮奶)
16. **Lime Bomber** (暴檸四季春)
17. **Topping Treasure Milk Tea** (寶藏奶茶)
18. **Shiba Waffle** (柴犬燒) — the shiba-shaped waffle.

### D. Spot / decorative elements
Small transparent motifs (~300–400 px) that float and parallax through scenes:
19. tea leaves, 20. boba pearls cluster, 21. peach, 22. strawberry, 23. lemon/lime,
24. cheese-foam swirl, 25. rising steam, 26. a plain OHAYO cup.

### E. UI accents (small)
27. Refined **hamburger / close / arrow / chevron** glyphs to match (optional — CSS covers these).
28. **Favicon** + a small square app icon using the tea-dog.
29. *(optional)* a flat-colour **logo lockup** variant of the wordmark for light/dark backgrounds
    (keep the existing line-art logo as the formal mark).

---

## 5. Motion / technical requirements
- **Layer separation is critical.** Anything that should move independently (each hill band,
  each cloud, the sun, each drink, each spot) must be its own file / clearly-named group — not
  flattened into one image.
- **Formats:**
  - **Primary: SVG** (optimised, grouped, sensible layer names) — best for crisp parallax.
  - **Animated pieces** (avatar hover, optional shiba blink, steam, bobbing boba): deliver as a
    **sprite sheet** *and*/or **Lottie JSON** (preferred) so it loops in the browser.
  - **Raster fallback:** PNG at **@1x / @2x / @3x**, transparent, sRGB.
- **Artboard sizes:** backgrounds ≥2400×900 (seamless); mascot 800×800; drinks 600×800; spots
  300–400²; sprite frames 200×200 (plus the 40×40 avatar variant).
- **Naming:** kebab-case matching the register above (e.g. `bg-hills-mid.svg`,
  `drink-brown-sugar.svg`, `shiba-hero.svg`) so they drop straight into `assets/`.
- **File structure:** `/background`, `/mascot`, `/drinks`, `/spots`, `/ui`, `/source`.
- **Source files:** include editable originals (Illustrator/Figma/Affinity) + exported assets.

## 6. Rights & usage
Full **commercial buyout, exclusive, worldwide, in perpetuity**, across **web, social, print and
packaging** (cups, waffle bags, signage). Source files owned by OHAYO TEA on final payment.
Illustrator credit is welcome in the site footer if desired.

## 7. Suggested phasing (helps quote & prioritise)
- **Phase 1 (MVP for the site):** A. background layers + B7 hero shiba + B9 avatar sprite +
  C10–C12 (three hero drinks) + D19–D22 spots. This alone makes the live concept feel bespoke.
- **Phase 2:** remaining drinks C13–C18, extra shiba poses B8, remaining spots.
- **Phase 3:** waffle, favicon/app icon, logo lockup, optional Lottie animations (steam, boba).

## 8. What we’ll provide the illustrator
- This brief + the live concept URL (shows every slot in context).
- The existing line-art tea-dog logo and brand colours.
- Real drink photos (for accurate colours/toppings): in `assets/drink-*.jpg`.
- The reference site to study for feel (misatoto).

## 9. Questions for the illustrator
1. Comfortable delivering **layered SVG** (and Lottie for the looping bits)?
2. Rough **quote & timeline** for Phase 1 vs. the full set?
3. Any style tests you’d like to do first (we suggest **1 background + the hero shiba** as a
   paid style test before the full commission)?

---
*Once the assets arrive, they drop into `style-4-story/assets/` and swap the placeholder SVGs /
photos — the parallax + scroll-reveal engine already in the page needs no changes.*
