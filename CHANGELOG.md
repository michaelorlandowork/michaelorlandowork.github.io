# Changelog

A running log of changes to the résumé website. Newest at the top.
When we make a change, we add a dated entry here.

---

## 2026-06-30 (session 4)

- **UW photo moved** from Band 2 to the **Education** section — it's now a dimmed
  full-bleed background behind the credential cards (the friends-on-a-couch shot
  read oddly under the "cross-border delivery" band). Panels are now slightly
  translucent so the campus photo shows through.
- **Band 2** (cross-border / "US, Europe & Asia") now uses a free Unsplash stock
  photo — an airplane over clouds at golden hour — until a real travel photo exists.
- **Logos fixed:** Solar badge now points to the real `logos/solar.jpg` (was still
  showing the "SC" monogram placeholder). Logo chips changed from near-black to
  **white** so the dark AWS wordmark is readable. All four badges are now real.
- **Folder reorganized:** all of Michael's site photos moved into a `photos/`
  subfolder; `index.html` paths updated. Tidied `logos/` (removed the placeholder
  `solar.png` and the duplicate `moh.svg`). Moved the spare `hero.JPG` and the
  dev `screenshots/` + `uploads/` folders out to `../photo-originals/`.

## 2026-06-30 (session 3)

- **Real photos added** — replaced most web placeholders with Michael's own shots,
  converted from HEIC/large originals, auto-oriented, compressed, and renamed:
  - **Hero** → `hero-ballard.jpg` (Ballard Ave NW street scene; swapped in for the old `hero.JPG`).
  - **Band 1** → `band-water.jpg` (Solar Chapter clean-water pipe install).
  - **Band 2** → `band-uw.jpg` (University of Washington "W", Seattle).
  - **Solar project card** → `project-solar.jpg` (villagers installing solar panels).
  - **AWS project card** → `project-aws.jpg` (logistics warehouse / pallets).
  - **Photography squares** → `photo-1…4.jpg` (kids w/ jerry cans, basket carry, water scoop, dusk spring).
- **Stock fill (3 slots)** — no real photo yet, so used free Unsplash hot-links
  (same pattern as Sports): **F&B** card (cafe interior), **Health** card
  (laptop + stethoscope), **closer** (workspace). Swap for real photos later.
- **Original full-size photos** backed up to `../photo-originals/` (kept out of the
  Website folder so the GitHub upload stays small). Old `hero.JPG` kept as a spare.

## 2026-06-30 (session 2)

- **Mobile version:** added a hamburger menu (≤720px) that opens a full-screen
  nav, since the desktop nav links were hidden on phones with nothing to replace
  them. The rest of the layout was already responsive.
- **Page transition:** added an intro curtain (name → lifts to reveal hero) and a
  fade-out when leaving to the résumé / LinkedIn. Made it self-removing so content
  can never be trapped behind the overlay.
- **Removed** "SQL Data Cleaning & Trend Analysis" from Certifications (PMP only now).
- **Work — Ministry of Health × Akselerasa** bullets updated: "44 community health
  centers (puskesmas)", added "...while restoring the staff attendance system", and
  added the 5 F&B branches bullet.
- **Sports** reworked: named real activities — **Tennis, Hyrox, Half Marathon** —
  each with its own copy. Clicking a photo now opens an enlarged **lightbox** with
  a title + description. Swapped in fitting real stock photos.
- **Photography:** added a credit line — "Every photograph on this site — these
  included — is one of mine."
- **Work logos:** added a logo badge to each role with auto-fallback to initials;
  created `logos/` with monogram placeholders (`moh`, `aws`, `solar`, `alfamart`).
- Balanced the **Life** section so Sports and Photography each have a photo strip.

## 2026-06-30

- **Live on GitHub Pages** at https://michaelorlandowork.github.io/
- Renamed repo to match username for a clean URL (no more duplicated path).
- Compressed `hero.JPG` from ~13 MB to ~0.3 MB (2400px wide) for fast loading.
  Original kept as `hero-original-backup.JPG` in the parent folder.
- Changed accent color from deep red `#C81E2D` to warm orange `#F26A21`
  (red clashed with the color photos).
- Removed all black-and-white / grayscale photo filters → photos now full color.
- Fixed the clipped descender on the "g" in the hero headline.
- Removed the smooth-scroll library + parallax effect (they caused scroll lag);
  scrolling is now crisp/native, reveals + smooth menu jumps kept.
- Added **Home** link to the nav (and made the name click back to top).
- Lightened the ghost headline grey so "that reach people." is readable.
- Added real hero photo (`hero.JPG`).

## Earlier (build history)

- Restyled to the Day One / Wolverine look: dark charcoal, huge Inter headlines,
  monochrome + single accent, monospace-style micro-labels, marquee strip.
- Reduced palette to two colors (black + white) per reference.
- Added a **Life** section with hobbies: Sports + Photography (with photo strip).
- Added full-bleed photo bands and image headers on project cards.
- Added 4 project case studies (F&B launches, Solar Chapter, MoH health app, AWS).
- Built the initial single-page résumé site from the 2026 résumé content.

---

## Plan / to do (next session)

**1. Real photos**
- [x] Replace placeholder photos with real ones — hero, both bands, Solar + AWS
      cards, and all four photography squares are now Michael's own.
- [ ] Replace the 3 remaining Unsplash stock fills with real photos when available:
      F&B branch opening, health clinic, and a confident headshot for the closer.
- [ ] Add real company logos to `logos/` (moh, aws, solar, alfamart) to replace
      the initial monograms.

**2. Content**
- [ ] Rethink the "Work" section framing — still a little CV-like. *Undecided.*

**3. Contact**
- [ ] Add a WhatsApp contact option (button/link).

## Other ideas (parked)

- [ ] Consider a custom domain (e.g. michaelorlando.com) for a more polished URL.
- [ ] Brainstorm/expand the project case studies (deeper stories).
- [ ] Optional: add a short "About me" / blog-style intro section.
