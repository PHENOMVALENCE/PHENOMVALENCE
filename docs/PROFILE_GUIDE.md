# GitHub Profile README — Maintenance Guide

Complete reference for updating the **PHENOMVALENCE** profile README. Designed so you can refresh content without redesigning the layout.

---

## Table of contents

1. [Section overview](#1-section-overview)
2. [Updating project cards](#2-updating-project-cards)
3. [Updating GitHub stats](#3-updating-github-stats)
4. [Changing colors and banners](#4-changing-colors-and-banners)
5. [Social links & contact](#5-social-links--contact)
6. [Certifications](#6-certifications)
7. [Contribution snake](#7-contribution-snake)
8. [File map](#8-file-map)

---

## 1. Section overview

| # | Section | Purpose | How to edit |
|---|---------|---------|-------------|
| 1 | **Hero** | Identity, typing SVG, counters | Top of `README.md` — banner, title, typing lines, badges |
| 2 | **About Me** | Positioning for recruiters | Table rows + short paragraph |
| 3 | **Currently Working On** | Live focus roadmap | Focus table checkmarks |
| 4 | **Tech Stack** | Categorized shields | Add/remove badge lines inside each `<details>` block |
| 5 | **Featured Projects** | Portfolio cards | Table cells + `assets/project-images/` |
| 6 | **GitHub Stats** | Metrics dashboard | Query params on stats URLs |
| 7 | **AI & ML** | Domain specialization | Project table + skill badges |
| 8 | **Experience** | Career narrative | Experience table rows |
| 9 | **Certifications** | Credential roadmap | Status column + links |
| 10 | **Connect** | Social discovery | Shield links |
| 11 | **Quote** | Soft close | Single italic line |
| 12 | **Support** | CTA / collaboration | Contact buttons |

HTML comments (`<!-- SECTION N — ... -->`) mark each block in `README.md`.

---

## 2. Updating project cards

### Replace a screenshot

1. Export a screenshot at **~800×420** (PNG preferred).
2. Overwrite the matching file in `assets/project-images/` **keeping the same filename**.
3. Commit and push. No README edit required if the filename is unchanged.

| Project | Asset file |
|---------|------------|
| Hanzo Marketplace | `hanzo-marketplace.png` |
| CrossLife LMS | `crosslife-lms.png` |
| Digital Town Square | `digital-town-square.png` |
| Bossify Academy | `bossify-academy.png` |
| M Grid | `m-grid.png` |
| Digital Economy Africa | `digital-economy-africa.png` |
| Portfolio Website | `portfolio-website.png` |

### Update description, tech, or links

In `README.md` → **Featured Projects**, find the project `<td>` and edit:

- Summary paragraph
- Tech badges (`img.shields.io`)
- Live Demo `href`
- GitHub `href`

### Add a new project card

1. Add `assets/project-images/your-project.png`.
2. Copy an existing `<td>...</td>` block.
3. Paste into a table row (2 cards per row works best).
4. Update image `src`, title, description, badges, and links.

---

## 3. Updating GitHub stats

All stats widgets use username **`PHENOMVALENCE`**. Change it only if the GitHub username changes.

### GitHub Stats & Top Languages

Service: [github-readme-stats](https://github.com/anuraghazra/github-readme-stats)

```text
https://github-readme-stats.vercel.app/api?username=PHENOMVALENCE&...
https://github-readme-stats.vercel.app/api/top-langs/?username=PHENOMVALENCE&...
```

Useful flags:

| Param | Effect |
|-------|--------|
| `count_private=true` | Include private commits (needs PAT on some hosts) |
| `include_all_commits=true` | Lifetime commits |
| `langs_count=8` | Number of languages |
| `bg_color` / `title_color` / `text_color` | Theme |

### Streak

Service: [github-readme-streak-stats](https://github.com/DenverCoder1/github-readme-streak-stats)

```text
https://streak-stats.demolab.com?user=PHENOMVALENCE&...
```

### Activity graph

Service: [github-readme-activity-graph](https://github.com/Ashutosh00710/github-readme-activity-graph)

```text
https://github-readme-activity-graph.vercel.app/graph?username=PHENOMVALENCE&...
```

### Productivity cards

Service: [github-profile-summary-cards](https://github.com/vn7n24fzkq/github-profile-summary-cards)

```text
https://github-profile-summary-cards.vercel.app/api/cards/stats?username=PHENOMVALENCE&theme=github_dark
https://github-profile-summary-cards.vercel.app/api/cards/productive-time?username=PHENOMVALENCE&theme=github_dark&utcOffset=3
```

`utcOffset=3` matches East Africa Time (EAT). Adjust if you relocate.

### Profile views / visitors

- Views: `https://komarev.com/ghpvc/?username=PHENOMVALENCE&...`
- Visitors: `https://visitor-badge.laobi.icu/badge?page_id=PHENOMVALENCE.PHENOMVALENCE&...`

Followers and stars use Shields.io GitHub endpoints and update automatically.

---

## 4. Changing colors and banners

### Design tokens (current theme)

| Token | Value | Usage |
|-------|-------|-------|
| Primary accent | `#58A6FF` | Badges, stats titles, typing SVG |
| Deep accent | `#1f6feb` | Gradients, graph lines |
| Background | `#0d1117` | Stats cards, dark panels |
| Text | `#c9d1d9` | Stats body text |
| Muted | `#8b949e` | Secondary labels |

Search-and-replace these hex values across `README.md` when rebranding.

### Typing animation

Edit the `lines=` query on the Typing SVG URL:

```text
https://readme-typing-svg.demolab.com?font=Fira+Code&...&lines=Line+One;Line+Two;Line+Three
```

Use `+` for spaces and `%26` for `&`.

### Hero banner

1. Design a wide banner (~**1280×420**, under **500KB**).
2. Replace `assets/banner.png`.
3. Optional: use [capsule-render](https://github.com/kyechan99/capsule-render) instead of a local file.

### Profile photo

Replace `assets/profile.png` with a square headshot (400×400 recommended).

### Footer wave

```text
https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f6feb,100:58A6FF&height=120&section=footer
```

Adjust the `color=` gradient stops to match a new palette.

---

## 5. Social links & contact

Update every occurrence of these URLs in `README.md` (Hero + Connect sections):

| Channel | Current |
|---------|---------|
| Portfolio | https://valencemwigani.tech |
| LinkedIn | https://www.linkedin.com/in/valence-mwigani-a8444031b |
| Email | mailto:mwiganivalence@gmail.com |
| GitHub | https://github.com/PHENOMVALENCE |
| Twitter / X | placeholder — set your handle |
| Instagram | placeholder — set your handle |
| Phone | +255 753 775 184 |

---

## 6. Certifications

When you earn a credential:

1. Change status from `🔜 Upcoming` to `✅ Earned`.
2. Wrap the provider badge or row title in a link to the credential URL.
3. Optionally add issue/expiry dates in a new column.

Cisco already notes CCNA foundation / in progress from DIT training.

---

## 7. Contribution snake

Workflow file: `.github/workflows/snake.yml`

1. Push to `main` (or run **Actions → Generate Contribution Snake → Run workflow**).
2. Wait for the job to publish SVGs to the `output` branch.
3. The README already points to:

```text
https://raw.githubusercontent.com/PHENOMVALENCE/PHENOMVALENCE/output/github-contribution-grid-snake-dark.svg
```

If the image 404s until the first run completes, that is expected. Re-run the workflow after enabling Actions on the repo.

---

## 8. File map

```text
PHENOMVALENCE/
├── README.md                      # Profile (rendered by GitHub)
├── CHANGELOG.md                   # Redesign history
├── assets/
│   ├── banner.png
│   ├── profile.png
│   ├── project-images/
│   └── README.md
├── docs/
│   └── PROFILE_GUIDE.md           # This file
└── .github/
    └── workflows/
        └── snake.yml              # Contribution snake generator
```

### Quick checklist after edits

- [ ] Relative asset paths still start with `./assets/`
- [ ] No duplicate social badges
- [ ] Stats username is still `PHENOMVALENCE`
- [ ] Project Live Demo / GitHub links are correct
- [ ] Images optimized (banner &lt; ~500KB)
- [ ] Preview on GitHub after push (dark mode + light mode)
