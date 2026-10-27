# Portfolio Website

Multi-page academic portfolio for https://mertyildiz19.github.io
Plain HTML/CSS/JS — no build step, deploys directly to GitHub Pages.

## Structure
- index.html        — home (hero, about excerpt, research cards, selected publications, experience excerpt, contact)
- about.html        — About Me (photo + facts sidebar, full bio)
- publications.html — all 16 papers grouped by topic, newest first, with IEEE/Journal/DOI + PDF links
- experience.html   — full timeline (PhD, IMDEA visit, Compulse, UNICEF, Hugo Boss)
- education.html    — degrees + conferences & doctoral training
- skills.html       — skill cards + languages + interests
- service.html      — TPC roles, reviewing, mentoring
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

## Verified (2026-10-27)
Multi-page rebuild: all 8 pages checked — no horizontal overflow at 1280px or 390px,
nav active states correct, all local assets resolve, publication pills aligned.
DOIs extracted from the papers themselves (14 of 15; VTC-Spring numerology and the
book chapter are PDF-only). Paper links point to IEEE/journal pages, not arXiv.
