# Changelog

All notable changes to the **PHENOMVALENCE** GitHub profile README.

---

## [2.0.0] — 2026-07-28

### Redesign — Premium Profile Overhaul

Complete rewrite of the profile README for recruiters, clients, and developers.

#### Added

- **12-section premium layout** with clear visual hierarchy and HTML section markers
- **Hero** with local banner, avatar, animated typing SVG, multi-role positioning, and counters (views, followers, stars, visitors)
- **About Me** icon table emphasizing Computer Engineering, full-stack work, AI/ML, African impact, and collaboration
- **Currently Working On** focus roadmap (AI/ML, NLP, CV, React, Laravel, Spring Boot, Next.js, Mobile Money, REST, Android)
- **Tech Stack** reorganized into Languages, Frontend, Backend, Databases, AI/ML, Tools, Cloud with consistent `for-the-badge` shields
- **Featured Projects** card grid with screenshot placeholders, tech badges, Live Demo, and GitHub links:
  - Hanzo Marketplace, CrossLife LMS, Digital Town Square, Bossify Academy, M Grid, Digital Economy Africa, Portfolio Website
- **GitHub Stats dashboard** — stats, top languages, streak, activity graph, contribution snake, productivity cards
- **AI & Machine Learning** section for NLP / CV / predictive projects
- **Experience** table — Sparkcraft Consulting, Proma Africa, Stanbic Bank Tanzania, AIESEC in Tanzania, AIESEC in IFM
- **Certifications** roadmap cards — Google, Cisco, Meta, Microsoft, Oracle, AWS
- **Connect** social badge row + local contact details
- **Quote** and **Support / Collaborate** CTA footer
- `assets/` folder (`banner.png`, `profile.png`, `project-images/`)
- `docs/PROFILE_GUIDE.md` — section docs, project cards, stats, colors/banners
- `.github/workflows/snake.yml` — daily contribution snake generator

#### Changed

- Replaced simple capsule-only hero with custom banner + typing multi-line identity
- Removed duplicate / overlapping interest badge clusters
- Unified badge sizing (`for-the-badge` for stacks, `flat-square` inside project cards)
- Tightened spacing and reduced empty white space via tables and grouped sections
- Aligned theme tokens to GitHub dark blue (`#58A6FF` / `#0d1117`)

#### Removed

- Redundant “Interests” and duplicate “Current Focus” badge strips
- Inline snake setup instructions from the README (moved to workflow + guide)
- Template-style filler that diluted expertise signaling

---

## [1.x] — Prior

Earlier iterations (capsule wave banner, basic stats, partial tech badges, fewer projects). See git history (`ReadMe`, `ReadMe 2`, `stats revision`).
