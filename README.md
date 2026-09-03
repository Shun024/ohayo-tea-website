# OHAYO TEA — Website Concept Deck

Three complete, self-contained homepage concepts for **OHAYO TEA**, a Shiba-Inu-themed
bubble-tea house in the heart of Manchester's Chinatown
([ohayotea.com](https://www.ohayotea.com) · [@ohayotea](https://instagram.com/ohayotea)).

This is a **redesign** of the client's current Wix site — same brand, drinks, story and
contact details, rebuilt as three fresh directions to choose from.

## How to view

Open **`index.html`** (the deck landing page) in any browser — it links to all three
concepts. Or open each one directly:

| # | Concept | Folder | Vibe |
|---|---|---|---|
| 01 | **Kawaii Pop** | `style-1-kawaii/index.html` | Cute, playful, mascot-led |
| 02 | **Tokyo Street** | `style-2-street/index.html` | Dark, bold, high-energy |
| 03 | **Modern Craft** | `style-3-craft/index.html` | Calm, editorial, premium |
| 04 | **Story · お茶物語** | `style-4-story/index.html` | Japanese editorial / flat-illustration magazine |

Each file is a single HTML page with embedded CSS + Google Fonts — no build step, no
dependencies. Just double-click. (Internet is needed only for web fonts and the Google
Maps embed.) All three share the same `assets/` folder.

---

## What's real vs. placeholder

**Pulled straight from the current site (real):**
- Brand name, tagline **"Drink it! Don't ask why!"**, and the hand-drawn Shiba "tea-dog"
  logo (`assets/logo-shiba.jpg`).
- The "Who are we?" story — Shiba-Inu-themed tea house, heart of Manchester, *first tea
  company in Manchester to combine freshly brewed fruit tea into our Fresh Fruit Tea
  series*, quality ingredients + handcrafted technique.
- **Real drink photos and names** (with the Chinese names shown on the packaging):
  Brown Sugar Tapioca Milk 黑糖珍珠鮮奶 · Strawberry Tea w/ Cheese Foam 芝芝草莓 ·
  White Peach Tea w/ Cheese Foam 芝士白桃 · Matcha Tapioca Milk 靜岡抹茶珍珠鮮奶 ·
  Strawberry Tapioca Milk 草莓珍珠鮮奶 · Lime Bomber 暴檸四季春 ·
  Super Fruitea 超級水果茶 · Topping Treasure Milk Tea 寶藏奶茶.
  Plus in the "more" list: Dirty OREO, Dirty BISCOFF, Hojicha, Taro, Pistachio Milk,
  Purple Quencher, Lychee Dragon and the OHAYO Shiba Waffle.
- **Ohayo Rewards Club** — free reusable tumbler with a £5+ purchase for new members;
  limited-edition monthly collectable pins for members.
- **Vegan menu** exists (linked to the live page).
- Contact: **95 Princess Street, Manchester M1 4HT** · **0161 236 4883** ·
  **contact@ohayotea.com** · open **7 days a week from 12pm** · IG `@ohayotea` ·
  Facebook `/OHAYOTEA` · Deliveroo.

**Now real (added from the live site):**
- **Prices** are taken from the current in-store menu (`OHAYO A3 MENU.jpg`) — shown as
  *Regular / Large* where the drink has two sizes, single price for large-only fruit teas.
  Toppings from £0.5; non-dairy (oat/soya) milk +£0.6.
- **Deliveroo link** points to the real store:
  `deliveroo.co.uk/brands/ohayo-tea`.

All eight featured drinks are current on-menu items with their exact menu prices. (Two
earlier photo-only items — Black Jade Tea and a plain Four Season Green Tea — were swapped
for the closest real menu drinks that match the photos: **White Peach Tea w/ Cheese Foam**
£4.5 and **Lime Bomber** 暴檸四季春 £5.5.)

**Still worth a quick client check:**
- Google Maps embed is by address; fine as-is, but confirm the pin.

---

## The three directions

### 01 · Kawaii Pop
- **Palette:** cream `#fff7ec`, coral `#e8574b` (sampled from the brand chop/cheese-foam
  bubbles), mustard `#f0a52e`, leaf `#7ba05a`.
- **Type:** Baloo 2 (rounded display) + Nunito (body).
- **Feel:** cute, bouncy, mascot-forward — chunky outlines, sticker badges, drop shadows,
  spinning blob behind the hero cup. Best for a young/family, Instagram-friendly audience.

### 02 · Tokyo Street
- **Palette:** charcoal `#0e0f0d`, electric lime `#c7f24a`, coral `#ff5a46`.
- **Type:** Anton (heavy condensed display) + Space Grotesk (body).
- **Feel:** loud, dark, urban. Giant "DRINK IT. DON'T ASK WHY." headline, tilted neon
  marquee, hover-zoom product grid. Uses the dark/neon-sign photography. Best for a Gen-Z,
  night-out, viral-boba crowd.

### 04 · Story · お茶物語  ← client's requested direction
- **Palette:** warm cream `#fef9f3` / `#fef3e9` / `#efdbcb`, warm-black ink `#2d2927`,
  deep green `#32645a`, soft accents peach `#ffc8b8`, yellow `#ffd258`, coral `#f15464`,
  ochre `#d89c52`, purple `#503278`.
- **Type:** Zen Old Mincho (lyrical serif headlines) + Zen Kaku Gothic New (Japanese-capable
  gothic body) + Zen Maru Gothic (rounded accents).
- **Feel:** Japanese editorial "digital magazine" — flat rounded inline-SVG illustrations
  (shiba, boba cup, tea leaves, fruit, shiba waffle), poetic bilingual headlines, story-card
  grid, generous whitespace. Modelled on the **misatoto** microsite
  (`town.shimane-misato.lg.jp/misatoto/`) the client referenced; palette & type sampled from
  it, then fitted to OHAYO's real content, photos and menu.

### 03 · Modern Craft
- **Palette:** warm paper `#f6efe4`, muted matcha `#5e6b3f`, clay `#b4553f`.
- **Type:** Zilla Slab (serif display) + Inter (body).
- **Feel:** calm, editorial, premium. Generous whitespace, quiet marquee, "three things we
  never skip" craft section, magazine-style menu. Positions OHAYO as a quality handcrafted
  tea house. Best for elevating the brand / attracting an older, spend-more customer.

---

## Shared structure (all three)
Sticky nav → hero → moving marquee → "Who are we?" about → signature drinks menu (real
photos) → craft/vegan/rewards sections → **Ohayo Rewards Club** → **Where are we?** visit
+ Google Map → footer with socials & Deliveroo. Fully responsive (mobile breakpoints
included).

## Suggested next steps
1. Pick a direction (or combine — e.g. Kawaii warmth with the Craft layout).
2. Confirm the two legacy items noted above (Black Jade / Four Season) or swap them.
3. Optional: add an online-order / gift-card link alongside Deliveroo.
4. Optional: wire the newsletter/rewards sign-up to an email provider and swap in any
   newer product photography.

---

### `assets/`
All images are the client's own, downloaded from the current site:
`logo-shiba.jpg` (hero logo) · `hero-brown-sugar-dark.jpg` · `hero-hand-sign.jpg` ·
`lineup.jpg` · and eight `drink-*.jpg` product shots.
