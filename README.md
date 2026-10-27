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
1. Push access — needs gh auth login or an SSH key, then:
     cd portfolio-website
     git init -b main
     git add . && git commit -m "Portfolio site"
     git remote add origin https://github.com/mertyildiz/mertyildiz.github.io.git
     git push -u origin main
   (If an old mertyildiz.github.io repo exists, either delete it on GitHub first
   or `git pull`/force-push. The URL currently 404s as of 2026-10-26.)
   NOTE: CV_*.pdf and Cover_Letter are excluded via .gitignore — the website
   itself is the CV; those PDFs stay local only.
2. After push: wait 1–5 min, check https://mertyildiz.github.io

## Verified locally (2026-10-27)
Rendered at localhost:8765 — desktop 1280px and mobile 390px checked after
content update (email, photo, under-review group, service list, experience).
