# Asset Specifications — Muhammad Raheel GitHub Profile

Replace temporary SVG placeholders with real assets before (or soon after) publishing. The README already references the paths below.

## Repository layout

```text
/
├── README.md
├── ASSETS.md
├── SETUP.md
└── assets/
    ├── banner/
    │   └── github-banner.svg   ← temporary (replace with .png recommended)
    ├── profile/
    │   └── muhammad-raheel.png ← YOU MUST PROVIDE
    ├── apps/
    │   ├── tamam-customer.svg  ← temporary placeholders (replace with .png)
    │   ├── tamam-vendor.svg
    │   ├── blaxity.svg
    │   ├── droparabia.svg
    │   ├── rewardee.svg
    │   ├── ride-hailing.svg
    │   ├── logicorp.svg
    │   ├── tradyom.svg
    │   └── megamart.svg
    └── screenshots/            ← optional
```

---

## 1. Banner — `assets/banner/github-banner.png`

| Spec | Value |
|------|--------|
| Filename | `github-banner.png` (preferred) or keep `.svg` |
| Size | **1280 × 320** px (or 1500 × 500) |
| Format | PNG (or SVG) |
| Max file size | Under ~300 KB |
| Style | Dark navy (`#0B1220` → `#0F172A`), cyan accent `#22D3EE` |
| Content | Name + title only; no clutter, no agency branding |
| Text | Muhammad Raheel · Flutter Tech Lead \| Senior Mobile Engineer |

**Current status:** Temporary SVG is included and works on GitHub. Export a polished PNG from Figma/Canva if you want a photographic or richer banner.

**After adding PNG:** update README banner `src` from `.svg` to `.png`.

---

## 2. Profile photo — `assets/profile/muhammad-raheel.png`

| Spec | Value |
|------|--------|
| Filename | `muhammad-raheel.png` |
| Size | **400 × 400** px minimum (square) |
| Format | PNG or JPG |
| Style | Professional headshot, clear face, neutral/simple background |
| Optional use | Add under the hero name if desired |

**Current status:** **Missing — you must provide this file.**

Optional README snippet (add under the name if you want the photo shown):

```html
<img src="./assets/profile/muhammad-raheel.png" width="140" alt="Muhammad Raheel" />
```

---

## 3. App icons — `assets/apps/*.png`

Replace each temporary SVG with the **official store icon** (1024×1024 export resized).

| File | App | Notes |
|------|-----|--------|
| `tamam-customer.png` | Tamam Customer | Replace `tamam-customer.svg` |
| `tamam-vendor.png` | Tamam Vendor | Replace `tamam-vendor.svg` |
| `blaxity.png` | Blaxity | Replace `blaxity.svg` |
| `droparabia.png` | Droparabia | Replace `droparabia.svg` |
| `rewardee.png` | Rewardee | Replace `rewardee.svg` |
| `ride-hailing.png` | Ride Hailing | Replace `ride-hailing.svg` |
| `logicorp.png` | Logicorp | Replace `logicorp.svg` |
| `tradyom.png` | Tradyom | Replace `tradyom.svg` |
| `megamart.png` | MegaMart | Replace `megamart.svg` |

| Spec | Value |
|------|--------|
| Size | **256 × 256** or **512 × 512** px |
| Format | PNG with transparency if available |
| Corners | Prefer original square icon; GitHub will display as-is |
| Source | App Store / Play Console export — do not invent icons |

**After replacing:** in `README.md`, change each `./assets/apps/<name>.svg` → `./assets/apps/<name>.png`.

---

## 4. Screenshots — `assets/screenshots/` (optional)

| Spec | Value |
|------|--------|
| Size | Phone frames ~ **1170 × 2532** or cropped UI at ~800 px wide |
| Format | PNG or JPG |
| Count | 1–2 per featured app max |
| Rule | Only real product screenshots — never mock fake UI |

Suggested names (only if you add them):

```text
assets/screenshots/tamam-customer-1.png
assets/screenshots/megamart-1.png
assets/screenshots/rewardee-1.png
```

Wire them into project cards only after files exist.

---

## 5. CV button

The CV badge currently points to [muhammadraheel.dev](https://muhammadraheel.dev/).

**Provide one of:**

1. Public CV URL (Google Drive / Dropbox / portfolio path), or  
2. `assets/cv/muhammad-raheel-cv.pdf` committed to the repo

Then update both CV badge `href`s in `README.md`.

---

## 6. Missing info to supply (optional upgrades)

| Item | Status |
|------|--------|
| Ride Hailing public store links | Not provided — placeholder in Featured Projects |
| Direct CV URL | Not provided — links to portfolio |
| Profile photo | Not provided |
| Official app icon PNGs | SVG placeholders only |
| Exact MegaMart download count | Intentionally omitted (highlighted qualitatively only) |

---

## 7. Where each asset goes

| Asset | Path |
|-------|------|
| Banner | `assets/banner/github-banner.png` |
| Profile photo | `assets/profile/muhammad-raheel.png` |
| App icons | `assets/apps/<app-name>.png` |
| Screenshots | `assets/screenshots/` |
| CV (optional) | `assets/cv/muhammad-raheel-cv.pdf` |
