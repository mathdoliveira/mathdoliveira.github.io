# uploads/ — image drop-in map

Every image slot on the site is wired to the exact filenames below. **Drop a JPG at the listed path and it will appear automatically** — no code changes, no rebuilds. If a file is missing, the existing paper-stripe SVG placeholder stays visible, so the site never breaks while you're still shooting.

All images: JPG (or WebP with `.jpg` extension), sRGB, quality ~82, each ≤ 200 KB.
Subjects should work with `object-fit: cover` — keep the focal point near the centre.

## Folder structure

```
uploads/
├── social/
│   └── og-image.jpg                       # 1200 × 630 — share preview
├── products/
│   ├── acne-leather-jacket.jpg            # 1000 × 1000 — card + product page (front)
│   ├── acne-leather-jacket-back.jpg       # 1000 × 1000 — product gallery thumb 2
│   ├── acne-leather-jacket-detail.jpg     # 1000 × 1000 — product gallery thumb 3 (collar)
│   ├── acne-leather-jacket-lining.jpg     # 1000 × 1000 — product gallery thumb 4 (cuff / lining)
│   ├── chanel-flap-bag.jpg                # 1000 × 1000 — card
│   ├── reformation-floral-dress.jpg       # 1000 × 1000 — card + more-from-seller
│   ├── ganni-silk-blouse.jpg              # 1000 × 1000 — card + more-from-seller
│   ├── levis-501.jpg                      # 1000 × 1000 — card + more-from-seller
│   └── toteme-coat.jpg                    # 1000 × 1000 — swipe.html card + more-from-seller
├── people/
│   └── seller-marie-l.jpg                 # 200 × 200 square — seller avatar on product.html
└── editorial/
    └── trust-authentication.jpg           # 1000 × 1250 (4:5) — trust section on landing
```

## Where each file appears

| File | Appears on | Slot |
|---|---|---|
| `social/og-image.jpg` | all 5 pages (head) | `og:image`, `twitter:image` — Slack/iMessage/LinkedIn preview |
| `products/acne-leather-jacket.jpg` | `index.html` (landing swipe deck), `swipe.html` (feed + saved), `product.html` (gallery main) | card photo |
| `products/acne-leather-jacket-back.jpg` | `product.html` | gallery thumb 2 |
| `products/acne-leather-jacket-detail.jpg` | `product.html` | gallery thumb 3 |
| `products/acne-leather-jacket-lining.jpg` | `product.html` | gallery thumb 4 |
| `products/chanel-flap-bag.jpg` | `index.html`, `swipe.html` | deck card |
| `products/reformation-floral-dress.jpg` | `index.html`, `swipe.html`, `product.html` | deck card + more-from-seller |
| `products/ganni-silk-blouse.jpg` | `index.html`, `swipe.html`, `product.html` | deck card + more-from-seller |
| `products/levis-501.jpg` | `index.html`, `swipe.html`, `product.html` | deck card + more-from-seller |
| `products/toteme-coat.jpg` | `swipe.html`, `product.html` | deck card + more-from-seller |
| `people/seller-marie-l.jpg` | `product.html` | seller avatar (overlays the "ML" initials if missing) |
| `editorial/trust-authentication.jpg` | `index.html` | trust section, 4:5 portrait |

## Production notes

- **Backdrop:** warm paper, linen, or aged wood. Avoid white seamless — it fights the site's `#f2ede4` paper background.
- **Lighting:** one soft source, natural if possible. Favor shadow + texture over catalog flatness.
- **Palette guide:** site colours are paper `#f2ede4`, forest `#2f3a2e`, gold `#b08a4a`, clay `#b8624a`. Shots should live inside that range; anything very saturated or clinical white will look glued on.
- **References:** Vestiaire Collective homepage stills, The Row lookbooks, Our Legacy editorial, Purple Magazine archives.

## If you only have one afternoon

Produce these four files first — they cover ~80% of the site's visual credibility:

1. `products/acne-leather-jacket.jpg`
2. `products/chanel-flap-bag.jpg`
3. `editorial/trust-authentication.jpg`
4. `social/og-image.jpg` (can be a crop of #1 or #3)

Everything else is layering.
