# GitHub Profile Guide — Software Engineer & AI Developer

Maintenance guide for the **PHENOMVALENCE** profile README. Positioning: active Software Engineer and AI / ML Developer — no management or non-dev content.

---

## 1. Section overview

| # | Section | What it communicates | Edit location |
|---|---------|----------------------|---------------|
| 1 | **Hero** | Identity, roles, activity counters | Top of `README.md` |
| 2 | **About Me** | Engineering + AI positioning | About table + paragraph |
| 3 | **Currently Building** | Active technical focus | Focus table |
| 4 | **Tech Stack** | Skills by category | Shield groups in `<details>` |
| 5 | **Featured Software Projects** | Production web systems | Project table + `assets/projects/` |
| 6 | **AI & Machine Learning** | NLP / CV / regression work | AI table + `assets/ai/` |
| 7 | **Development Activity** | Graphs, snake, streak, languages | Stats image URLs |
| 8 | **Development Milestones** | Engineering timeline | ASCII timeline + checklist |
| 9 | **Commit History** | Consistency & shipping habit | Heatmap, streak, repo links |
| 10 | **GitHub Statistics** | Aggregate metrics | Stats cards + badges |
| 11 | **Connect** | Professional contact | Shield links |
| 12 | **Quote** | Soft close | Quote line |

HTML comments (`<!-- SECTION N -->`) mark each block.

**Do not add:** business development, AIESEC, leadership/org roles, or non-engineering projects.

---

## 2. Updating project cards (software)

### Replace a screenshot

1. Capture ~**800×420** PNG.
2. Overwrite the file in `assets/projects/` (same name).
3. Push — no README change needed.

| Project | File |
|---------|------|
| Hanzo Marketplace | `assets/projects/hanzo-marketplace.png` |
| CrossLife LMS | `assets/projects/crosslife-lms.png` |
| Digital Town Square | `assets/projects/digital-town-square.png` |
| Bossify Academy | `assets/projects/bossify-academy.png` |

### Update copy or links

In **Featured Software Projects**, edit the matching `<td>`:

- Summary paragraph
- Tech badges
- Live Demo `href`
- Source `href`

### Add a software project

1. Add `assets/projects/your-project.png`.
2. Copy an existing project `<td>`.
3. Place it in a table row (2 columns preferred).
4. Update image, title, summary, badges, and links.

---

## 3. Updating AI projects

### Existing AI cards

| Project | Asset | Repo (if public) |
|---------|-------|------------------|
| News Category Classification | `assets/ai/news-classification.png` | Add link when published |
| Face Emotion Recognition | `assets/ai/face-emotion.png` | `Facial-Emotion-Recognition` |
| Electricity Consumption Prediction | `assets/ai/electricity-prediction.png` | `ElectricityConsumption` |

Edit the AI table cell for pipeline details (tokenization, CNN, feature engineering, etc.).

### Promote a “Future AI” project

1. Create `assets/ai/spam-detection.png` (example).
2. Copy an AI card `<td>` into the three-column table (or add a new row).
3. Remove it from the **Future AI Projects** badge row.
4. Link the GitHub repository.

### Future ideas currently listed

- Spam Detection (NLP)
- Crop Recommendation (ML)
- Recommendation Systems (Deep Learning)

---

## 4. Adding future repositories

1. Push the new repo under `PHENOMVALENCE`.
2. Decide category:
   - **Web / API** → Featured Software Projects
   - **ML / NLP / CV** → AI & Machine Learning
3. Add screenshot under `assets/projects/` or `assets/ai/`.
4. Add a card in `README.md`.
5. Optionally append a ✔ row under **Development Milestones**.
6. Update Live Demo / Source URLs.

Keep the profile engineer-first: only ship technical work here.

---

## 5. Activity, commits & stats widgets

Username everywhere: **`PHENOMVALENCE`**.

| Widget | Service |
|--------|---------|
| Contribution graph | `github-readme-activity-graph.vercel.app` |
| Snake | `raw.githubusercontent.com/.../output/github-contribution-grid-snake-dark.svg` |
| Heatmap / commit calendar | `ghchart.rshah.org/58A6FF/PHENOMVALENCE` |
| Streak | `streak-stats.demolab.com` |
| Stats / languages | `github-readme-stats.vercel.app` |
| Summary cards | `github-profile-summary-cards.vercel.app` |

### Snake setup

Workflow: `.github/workflows/snake.yml`

1. Enable GitHub Actions on this repo.
2. Run **Generate Contribution Snake** (or wait for the daily cron).
3. Image publishes to the `output` branch.

### Theme tokens

| Token | Hex |
|-------|-----|
| Accent | `#58A6FF` |
| Deep | `#1f6feb` |
| Background | `#0d1117` |
| Text | `#c9d1d9` |
| AI accent | `#A371F7` |

Search-replace these in `README.md` to rebrand.

### Banner & avatar

- Replace `assets/banner.png` (~1280×420, keep under ~100KB if possible).
- Replace `assets/profile.png` (square headshot).

### Typing SVG

Edit `lines=` on the Typing SVG URL (spaces → `+`, `&` → `%26`).

---

## 6. Connect links

| Channel | URL |
|---------|-----|
| Portfolio | https://valencemwigani.tech |
| GitHub | https://github.com/PHENOMVALENCE |
| LinkedIn | https://www.linkedin.com/in/valence-mwigani-a8444031b |
| Email | mailto:mwiganivalence@gmail.com |

Update both Hero and Connect when links change.

---

## 7. File map

```text
PHENOMVALENCE/
├── README.md
├── CHANGELOG.md
├── assets/
│   ├── banner.png
│   ├── profile.png
│   ├── projects/
│   ├── ai/
│   ├── icons/
│   └── README.md
├── docs/
│   └── PROFILE_GUIDE.md
└── .github/workflows/snake.yml
```

### Pre-push checklist

- [ ] Only software + AI content (no org/leadership filler)
- [ ] Relative `./assets/` paths
- [ ] Project and AI screenshots updated
- [ ] Repo / demo links correct
- [ ] Stats username is `PHENOMVALENCE`
- [ ] Snake workflow run at least once after push
