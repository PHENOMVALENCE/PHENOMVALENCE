# GitHub Profile Guide — Software Engineer & AI Developer

Maintenance guide for the **PHENOMVALENCE** profile README. Positioning: active Software Engineer and AI / ML Developer — no management or non-dev content.

---

Design rules live in [`PROFILE_DESIGN.md`](PROFILE_DESIGN.md). Read that file before changing layout, colors, badges, or remote widgets.

## 1. Section overview

| # | Section | What it communicates | Edit location |
|---|---------|----------------------|---------------|
| 1 | **Hero** | Identity, positioning, and contact links | Top of `README.md` |
| 2 | **What I build** | Engineering + AI positioning | Intro and capability table |
| 3 | **Selected work** | Production web systems | Project table + `assets/projects/` |
| 4 | **Applied AI** | NLP / CV / regression work | AI table + `assets/ai/` |
| 5 | **Technical toolkit** | Skills by category | Compact four-column table |
| 6 | **Engineering trajectory** | Evidence-led development timeline | Text timeline |
| 7 | **GitHub activity** | Contribution graph and core statistics | Two widget providers |
| 8 | **Contact** | Collaboration call to action | Closing block |

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

### Add an AI project

1. Create `assets/ai/spam-detection.png` (example).
2. Copy an AI card `<td>` into the three-column table (or add a new row).
3. Add a concise description of the implemented pipeline.
4. Link the GitHub repository when it is public.

---

## 4. Adding future repositories

1. Push the new repo under `PHENOMVALENCE`.
2. Decide category:
   - **Web / API** → Selected work
   - **ML / NLP / CV** → Applied AI
3. Add screenshot under `assets/projects/` or `assets/ai/`.
4. Add a card in `README.md`.
5. Add a dated entry to **Engineering trajectory** only when it represents a meaningful career milestone.
6. Update project and repository URLs.

Keep the profile engineer-first: only ship technical work here.

---

## 5. Activity

Username everywhere: **`PHENOMVALENCE`**.

| Widget | Service |
|--------|---------|
| Contribution snake | `raw.githubusercontent.com/PHENOMVALENCE/PHENOMVALENCE/output/` |

Keep the activity section limited to the GitHub-hosted contribution snake and native GitHub profile links. Do not add third-party activity graphs, statistics cards, heatmaps, counters, or language cards without first checking that the endpoints return HTTP 200 reliably.

### Optional snake workflow

Workflow: `.github/workflows/snake.yml`

1. Enable GitHub Actions on this repo.
2. Run **Generate Contribution Snake** (or wait for the daily cron).
3. Image publishes to the `output` branch.

The snake is displayed in the current profile and depends on this workflow publishing the SVG to the `output` branch.

### Theme tokens

| Token | Hex |
|-------|-----|
| Accent | `#0969DA` |
| Accent soft | `#DDF4FF` |
| Ink | `#18181B` |
| Text | `#57606A` |
| Background | `#FFFFFF` / transparent |

Search-replace these in `README.md` to rebrand.

### Hero and avatar

- Edit `assets/hero.svg` for the animated hero. Preserve its `1280×420` view box, accessible title/description, static first frame, and reduced-motion rule.
- `assets/banner.png` is retained as the previous static banner and fallback source.
- Replace `assets/profile.png` (square headshot).

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
│   ├── hero.svg
│   ├── banner.png
│   ├── profile.png
│   ├── projects/
│   ├── ai/
│   ├── icons/
│   └── README.md
├── docs/
│   ├── PROFILE_DESIGN.md
│   └── PROFILE_GUIDE.md
└── .github/workflows/snake.yml
```

### Pre-push checklist

- [ ] Only software + AI content (no org/leadership filler)
- [ ] Relative `./assets/` paths
- [ ] Project and AI screenshots updated
- [ ] Repo / demo links correct
- [ ] Contribution snake username is `PHENOMVALENCE`
- [ ] No duplicate activity widgets or manually maintained counters
