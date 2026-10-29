# Portfolio Website

Multi-page academic portfolio for https://mertyildiz19.github.io
Plain HTML/CSS/JS — no build step, deploys directly to GitHub Pages.

## Structure
- index.html        — home (hero, bio excerpt, research cards, selected publications, experience excerpt, contact)
- bio.html          — Bio (photo + facts sidebar, full bio)
- publications.html — all 16 papers grouped by topic, newest first, with IEEE/Journal/DOI + PDF links
- experience.html   — full timeline (PhD, IMDEA visit, Compulse, UNICEF, Hugo Boss) + Education section (Ph.D., M.Sc., B.Sc.)
- skills.html       — skill cards + languages + interests
- activities.html   — advised theses, TPC roles, reviewing, awards
- contact.html      — email, location, profiles
- css/style.css     — shared design system (every page links this one file)
- js/main.js        — mobile nav toggle + footer year
- assets/Profile_photo.jpg — portrait photo (hero + favicon)
- My_papers_pdfs/   — 15 paper PDFs linked from publications.html

## Working docs (gitignored, never deployed — the website IS the CV)
CV_1.pdf, CV_2.pdf, Cover_Letter (5).pdf, Github_token.txt

## Deployment
Repo: github.com/MertYILDIZ19/MertYILDIZ19.github.io (name MUST match the username for a user-site URL).
Push with a fine-grained PAT (Contents: read/write):
  git remote set-url origin https://x-access-token:<tok>@github.com/MertYILDIZ19/MertYILDIZ19.github.io.git
  git push
  git remote set-url origin https://github.com/MertYILDIZ19/MertYILDIZ19.github.io.git   # strip token after
Then wait 1–5 min and read back https://mertyildiz19.github.io to confirm it's live.

## Verified (2026-10-28)
Design system v2 rebuild (visual + mobile pass):
- Fluid type scale (clamp()), gradient accent highlights, refined cards/timeline/publication
  cards with hover states, dark footer, scroll-reveal animations (JS-gated, reduced-motion safe),
  animated nav underlines, consistent container on all page heroes.
- Mobile: hamburger dropdown with drop animation + Escape-to-close, single-column stacks at
  <=860px/<=720px/<=420px; verified no horizontal overflow at 390px on all 8 pages and clean
  desktop layout at 1280px. All local assets (incl. 15 paper PDFs) resolve; nav active states
  correct per page.
- Fixed: `.section a` was overriding primary-button text color (blue-on-blue) — now scoped to
  `a:not(.btn)`.
DOIs extracted from the papers themselves (14 of 15; VTC-Spring numerology and the
book chapter are PDF-only). Paper links point to IEEE/journal pages, not arXiv.
