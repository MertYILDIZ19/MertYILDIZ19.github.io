# Portfolio Website

Single-page academic portfolio for mertyildiz.github.io.
Plain HTML/CSS/JS — no build step, deploys directly to GitHub Pages.

## Structure
- index.html        — the whole site (hero, about, research, publications, service, experience, education, skills, contact)
- css/style.css     — all styling (responsive down to 390px)
- js/main.js        — mobile nav toggle + footer year
- assets/Profile_photo.jpg — portrait photo (hero + favicon)
- CV_1.pdf          — industry CV (Mert's working doc, not part of the site)
- CV_2.pdf          — academic CV (Mert's working doc, not part of the site)
- Cover_Letter (5).pdf — cover letter (Mert's working doc, not part of the site)

## What's real (from LinkedIn + Google Scholar + Mert's CVs, Oct 2026)
- Bio / research interests / service (TPC IEEE WCNC 2025, MAIN 2026; reviewer Computer Networks, Vehicles, IEEE WCNC/VTC/VNC/MAIN/MedComNet)
- Publications grouped: Under Review (3), Data Centers & LLM Serving, Vehicular Networks & V2X, Other
- Experience timeline (Sapienza PhD Nov 2023–present; IMDEA visit Feb–Jul 2026 under Prof. Ajmone Marsan; Compulse industry Jan 2019–Jan 2025)
- Education timeline (PhD Sapienza, defense expected Jan 2027; M.Sc. Data Science 110/110; B.Sc. Industrial Engineering Yasar)
- Skills cards (Systems & Networking, Theoretical Foundations, AI & ML, Programming & Tools)
- Links: Google Scholar, LinkedIn, GitHub
- Email: mert.yildiz@uniroma1.it
- Photo: assets/Profile_photo.jpg

## TODO before going live
1. ~~Push access~~ DONE (2026-10-27) — repo renamed to `MertYILDIZ19.github.io`
   (must match the GitHub username for a user-site URL), pushed, and verified
   live at https://mertyildiz19.github.io with the animated background.
   NOTE: CV_*.pdf and Cover_Letter are excluded via .gitignore — the website
   itself is the CV; those PDFs stay local only.
2. Optional: delete Github_token.txt locally and revoke the PAT in GitHub.

## Verified locally (2026-10-27)
Rendered at localhost:8765 — desktop 1280px and mobile 390px checked after
content update (email, photo, under-review group, service list, experience).
