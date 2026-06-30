# Michael Orlando — Portfolio / Résumé Website

A single-page personal résumé site, hosted free on GitHub Pages.

**Live URL:** https://michaelorlandowork.github.io/

---

## Files in this folder

| File | What it is |
|---|---|
| `index.html` | The entire website (HTML + CSS + JS in one file) |
| `hero.JPG` | The big hero background photo (compressed for web) |
| `Michael_Orlando_Resume_2026_New.pdf` | The downloadable résumé (linked from the "Download résumé" button) |
| `README.md` | This file |
| `CHANGELOG.md` | Running log of every change + decisions to keep |

> The other section photos (projects, bands, hobbies) currently load placeholder
> images from the web (picsum.photos). Replace them with real photos when ready —
> see "Swapping photos" below.

---

## How to make a change and publish it

1. Edit `index.html` (or ask Claude to).
2. Go to the GitHub repo → **Add file → Upload files**.
3. Drag in the changed file(s) → **Commit changes**.
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

## Swapping photos

Each image in `index.html` has a comment above it saying what fits, e.g.
`<!-- HERO · swap: a wide, moody photo... -->`.

1. Drop your photo into this `Website` folder.
2. In `index.html`, replace the image URL with your filename, e.g.
   `url('https://picsum.photos/seed/mo-solar9/900/600')` → `url('solar.jpg')`.
3. Keep filenames lowercase, no spaces (`clean-water.jpg`, not `Clean Water.jpg`).
4. Big background photos look best ~1600–2400px wide; the 4 small hobby
   squares ~600px. Compress large files so the site stays fast.

Image spots: hero, 2 full-bleed bands, 4 project cards, closer, 4 photography squares.

---

## Hosting notes

- Repo name matches the username (`michaelorlandowork.github.io`), which is why
  the URL is the clean `https://michaelorlandowork.github.io/`.
- To use a custom domain later (e.g. `michaelorlando.com`): buy the domain, then
  repo **Settings → Pages → Custom domain**.
