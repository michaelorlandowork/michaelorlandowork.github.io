# Michael Orlando — Portfolio / Résumé Website

A single-page personal résumé site, hosted free on GitHub Pages.

**Live URL:** https://michaelorlandowork.github.io/

---

## Files in this folder

| File / folder | What it is |
|---|---|
| `index.html` | The entire website (HTML + CSS + JS in one file) |
| `photos/` | All of Michael's own site photos (see below) |
| `logos/` | Company logo badges for the Work section (`moh.png`, `aws.png`, `solar.jpg`, `alfamart.png`) |
| `Michael_Orlando_Resume_2026_New.pdf` | The downloadable résumé (linked from the "Download résumé" button) |
| `README.md` | This file |
| `CHANGELOG.md` | Running log of every change + decisions to keep |

**Inside `photos/`:**

| File | Where it shows |
|---|---|
| `hero-ballard.jpg` | Hero background — Ballard Ave NW street scene |
| `band-water.jpg` | Band 1 — Solar Chapter clean-water pipe install |
| `band-uw.jpg` | **Education** section background — University of Washington ("W") |
| `project-solar.jpg` | Solar Chapter project card — installing solar panels |
| `project-aws.jpg` | AWS project card — logistics warehouse / pallets |
| `photo-1…4.jpg` | The four Photography squares (kids, basket, water scoop, dusk spring) |

> Most photos are Michael's own: hero, Band 1, the Education background, the
> Solar + AWS project cards, and all four photography squares. Three slots use
> free Unsplash stock photos until real ones exist — the **F&B** card (cafe
> interior), the **Health** card (laptop + stethoscope), the **closer**
> (workspace) — plus **Band 2** (airplane over clouds, for the cross-border
> story). These are hot-linked, like the Sports photos. Full-size originals and
> retired files are backed up one level up in `../photo-originals/`.
> All four Work logos are now real (white chips so they read on the dark tiles).

---

## How to make a change and publish it

1. Edit `index.html` (or ask Claude to).
2. Go to the GitHub repo → **Add file → Upload files**.
3. Drag in the changed file(s) → **Commit changes**. (Upload the whole `logos/`
   folder too if it's not in the repo yet.)
4. Wait ~1–2 minutes — the live site updates automatically.

---

## Design decisions (keep these consistent)

- **Colors:** two only — black `#010101` + white `#FFFFFF`, plus greys derived from them.
- **Accent:** warm orange `#F26A21`, used *sparingly* (name dot, section indexes,
  list markers, marquee dots, toggles, stat +/% signs). Defined once as `--accent`
  at the top of the `<style>` block — change it there to recolor the whole site.
- **Font:** Inter (clean Helvetica-style grotesk), heavy weights for headlines.
- **Style reference:** Day One / Wolverine — dark, editorial, big bold type,
  full-bleed photos, generous space.

---

## Interactions (how the moving parts work)

- **Intro transition:** a black curtain shows the name on load, then lifts to
  reveal the hero. It removes itself afterward so nothing can get stuck behind it.
  Clicking the résumé / LinkedIn buttons fades the page out before leaving.
- **Mobile menu:** below 720px the nav links collapse into a hamburger that opens
  a full-screen menu.
- **Sports tiles:** click a Sports photo to open an enlarged lightbox with its
  title + description. Close with ✕, the backdrop, or Esc. Hover shows a teaser.
- **Work logos:** each role shows a logo badge; if a logo image is missing it
  falls back to the company initials automatically.

---

## Swapping photos

Each image in `index.html` has a comment above it saying what fits, e.g.
`<!-- HERO · swap: a wide, moody photo... -->`.

1. Drop your photo into the `photos/` folder.
2. In `index.html`, replace the image URL with your filename, e.g.
   `url('https://images.unsplash.com/...')` → `url('photos/clean-water.jpg')`.
3. Keep filenames lowercase, no spaces (`clean-water.jpg`, not `Clean Water.jpg`).
4. Big background photos look best ~1600–2400px wide; the small squares ~600px.
   Compress large files so the site stays fast.

Image spots: hero, Band 1, the Education background, 4 project cards, closer,
Band 2, 4 photography squares. (The 3 Sports photos and the F&B / Health /
closer / Band 2 fills are hot-linked Unsplash stock.)

---

## Swapping logos (Work section)

All four badges now use real logos: `moh.png` (Ministry of Health × Akselerasa),
`aws.png` (Amazon Web Services), `solar.jpg` (Solar Chapter), `alfamart.png`
(Alfamart). Each badge falls back to the company initials if its image is missing.

1. To replace one, drop the new file into `logos/` with the same base name. The
   `src` in `index.html` must match the extension — `.png` and `.jpg` both work
   (Solar uses `solar.jpg`).
2. Logos sit on a **white** chip (so dark marks like AWS stay readable), so a
   transparent or white background works well. Square-ish looks best.

---

## Hosting notes

- Repo name matches the username (`michaelorlandowork.github.io`), which is why
  the URL is the clean `https://michaelorlandowork.github.io/`.
- To use a custom domain later (e.g. `michaelorlando.com`): buy the domain, then
  repo **Settings → Pages → Custom domain**.
