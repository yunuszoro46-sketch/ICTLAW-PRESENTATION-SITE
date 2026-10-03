# The Cyber Times

A newspaper-style crime report that turns a presentation topic into an interactive web page: **a CEO impersonation scam carried out through a fake Facebook profile and mobile banking (MFS) transfers in Bangladesh.**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Open%20the%20Site-BA0000?style=for-the-badge&logo=render&logoColor=white)](https://cyber-times-onrender-com.onrender.com/)

**Live site:** https://cyber-times-onrender-com.onrender.com/
---

## The case

Fahim downloads public LinkedIn photos and details belonging to CEO Farhan Ahmed and opens a fake Facebook account using his full name and the company's branding. He sends urgent messages to three department managers, claims a medical emergency while travelling abroad, and persuades them to transfer BDT 2 Lakhs by mobile banking. The fraud is discovered when the real CEO returns. The company reports the profile, cyber police trace the mobile wallet to Fahim's real national ID registration, and he is arrested and charged.

## What is on the page

- **Header:** sticky bar with the blackletter title, section links, a dark/light toggle and a scroll-progress line.
- **Article opening:** centered kicker, headline, italic deck and byline, then a full-width black hero band with the lead illustration.
- **The short version:** four plain-language cards (what happened, the motive, how he was caught, how to stop it) under the case strip.
- **Why it works:** four pressure levers (authority, urgency, fear, secrecy) with a counter for each, plus real FBI IC3 statistics.
- **Case file strip:** suspect, victim, loss and status in four boxes.
- **Story:** single reading column with a drop cap, a pull quote, illustrations with captions, and three animated SVG scenes (cloned profile, scam chat, money trail).
- **Following the Money and timeline:** simple vertical step lists.
- **The Charges:** seven tap-to-expand rows. **The Punishment:** a boxed list.
- **Corporate Advisory:** six safeguards with priority badges, tick cards and a live progress bar.
- **Hover zoom:** every image and animation grows slightly under the mouse (`.zoom` wrapper).

## Legal references used

| Act / Code | Section | Offence |
|---|---|---|
| Cyber Security Act 2023 | 24 | Identity theft and digital impersonation |
| Cyber Security Act 2023 | 23 | Digital / electronic fraud |
| Cyber Security Act 2023 | 26 | Unauthorized collection / use of identity details |
| Penal Code 1860 | 416 & 419 | Cheating by personation |
| Penal Code 1860 | 420 | Cheating and inducing delivery of property |
| Penal Code 1860 | 468 & 471 | Forgery for the purpose of cheating |
| Money Laundering Prevention Act 2012 / MFS rules | n/a | Receiving fraud proceeds in an NID-linked wallet |

> **Disclaimer:** Section numbers were supplied by the project author and are not legal advice. Verify them against the official text of each law before relying on them. The case number, timestamps, account age and the "Central Bank" side story are **illustrative placeholders**.

## Design

- **Concept:** a New Yorker-inspired editorial layout: white space, a 700px reading column, large serif type and hairline rules.
- **Palette:** white, ink `#1a1a1a`, grey `#6b6b6b`, crimson `#c8102e`. Dark theme uses `#121212` and `#ff5a6e`.
- **Typography:** UnifrakturMaguntia (title), Playfair Display (headlines), Source Serif 4 (body), Libre Caslon Text italic (decks and quotes), Inter (labels).
- **Accessibility:** visible keyboard focus, real buttons, checkboxes and `<details>` rows, light and dark themes, reduced-motion support.

## Project structure

```
cyber-times/
├── index.html    # the whole site: HTML, CSS, JS and embedded images
├── render.yaml   # Render static-site config
├── README.md
└── .gitignore
```

No build step, no dependencies. Fonts load from Google Fonts.

## Run locally

Open `index.html` in any modern browser.

## Deploy on Render

1. Push this repo to GitHub.
2. In Render, choose **New → Static Site** and connect the repo.
3. Leave **Build Command** empty and set **Publish Directory** to `.`
4. Create the site. Every push to `main` redeploys automatically.

## Design prompts

The look was developed iteratively and the prompts can be reused in Figma, Dribbble shots or Lovable. The key brief:

> Redesign "The Cyber Times" as a high-density editorial front page in the style of an investigative newspaper issue. Blackletter masthead, huge red serif headline, two-column justified story with a drop cap, evidence collage hero, a charges grid, a punishment box in italic type, a case file and timeline sidebar, and a corporate advisory card with priority badges. Newsprint, ink and crimson palette. Responsive, with dark mode.

## Credits

- Illustrations: _add the artist, source and licence for each of the seven embedded images before publishing._
- Built with HTML, CSS and a little JavaScript, designed and iterated with Claude.

## Licence

_Choose a licence (for example MIT) before publishing._


## Facts and sources

The story is an illustrative case study. Statistics come from the FBI IC3 2025 Internet Crime Report. Bangladesh cyber law changed in 2025 and 2026 (2023 Act repealed by the 2025 Ordinance, then the 2026 Act), so re-check legal references before publishing. Sources are listed at the bottom of the page.
