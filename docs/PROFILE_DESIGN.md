# PHENOMVALENCE Profile Design

## Direction

The profile uses a precise, editorial, developer-first visual language with restrained cinematic motion. It borrows principles—not brand assets—from the Vercel, Linear, Stripe, and Runway analyses in `awesome-design-md`:

- Vercel: monochrome foundation, technical restraint, and clear hierarchy.
- Linear: compact information architecture and low visual noise.
- Stripe: credible product presentation and a restrained blue accent.
- Runway: cinematic depth, controlled light, and motion used as atmosphere rather than decoration.

The result should feel like an engineer's portfolio, not a badge collection or a marketing landing page.

## Tokens

| Role | Value | Use |
|---|---|---|
| Accent | `#0969DA` | Links, graph line, primary badges |
| Accent soft | `#DDF4FF` | Graph fill and subtle emphasis |
| Ink | `#18181B` | Dark badges and high-emphasis elements |
| Body | `#57606A` | Supporting text in remote widgets |
| Canvas | `#FFFFFF` / transparent | GitHub-native surfaces |

## Composition rules

1. Lead with identity, positioning, and four useful links.
2. Put evidence of work before tools and activity metrics.
3. Use screenshots for project proof; use badges only for actions or compact metadata.
4. Keep no more than two adjacent columns for software projects and three for compact AI projects.
5. Prefer native Markdown headings, prose, code tags, and tables over decorative remote images.
6. Use only the GitHub-hosted contribution snake for visual activity; link to GitHub's native overview for detailed metrics.
7. Avoid unverifiable counters such as manually maintained repository or commit totals.
8. Keep one accent color. Technology logo colors may appear only inside project screenshots or existing assets.
9. Maintain meaningful alt text for every image.
10. Keep the page useful when third-party statistics services fail to load.
11. Use motion only in the hero, focus line, and contribution trail.
12. Every custom animation must provide a static first frame and respect `prefers-reduced-motion` where supported.

## Motion language

- The local `assets/hero.svg` owns the primary motion experience.
- Grid, glow, orbit, and signal animations move slowly and never obstruct text.
- The remote typing line rotates through three evidence-based engineering themes.
- The contribution snake appears once as a playful closing signal, not as the profile's main content.
- Do not embed Vercel-hosted activity graphs or statistics cards; they have returned HTTP 402/503 and leave broken images in the profile.
- Avoid flashing, rapid scaling, continuous page-wide movement, or multiple competing accent colors.

## Content voice

- Direct, specific, and evidence-led.
- Describe systems and outcomes without inflated claims.
- Use sentence case for headings.
- Avoid filler lists of ambitions or planned projects.
- Keep software engineering and applied AI as the two central themes.

## Reference files

- `C:\xampp\htdocs\awesome-design-md\design-md\vercel\DESIGN.md`
- `C:\xampp\htdocs\awesome-design-md\design-md\linear.app\DESIGN.md`
- `C:\xampp\htdocs\awesome-design-md\design-md\stripe\DESIGN.md`
- `C:\xampp\htdocs\awesome-design-md\design-md\runwayml\DESIGN.md`
