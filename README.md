# Bence Supola — Applied Data Science Portfolio

An Astro-based research and applied data science portfolio, hosted on GitHub Pages.

## Local development

Requires Node.js 22 or newer.

```bash
npm install
npm run dev
```

Open the local address printed by Astro (usually http://localhost:4321).

## Deployment

1. Push all files to the `main` branch of `supolabence/supolabence.github.io`.
2. In GitHub repository **Settings → Pages → Build and deployment**, select **GitHub Actions** as the source.
3. Check the **Actions** tab for the `Deploy Astro to GitHub Pages` workflow.
4. When deployment completes, visit https://supolabence.github.io/.

The repository includes a GitHub Actions workflow to build and publish Astro automatically.

## Content and rights review before publishing

- **The portfolio includes both unpublished research visualizations and a published PLOS ONE figure.** The defensive partial-dependence visualization is Figure 4 from the PLOS ONE paper, licensed CC BY 4.0, with attribution on the case-study page. Other publisher figure exports have been removed.
- These images are not automatically cleared for public use merely because they were not published. Before deploying, verify that the underlying NBA/SportVU tracking data and any third-party graphical elements can be displayed publicly under the applicable data access agreements.
- The extra-pass orange curves are described as quadratic fits; the figure alone does not establish that they are quantile-regression fits.
- Confirm the precise wording and context of reported model metrics against the original paper.
- Review biography and individual versus collaborative research contributions.
- No license is granted for the repository as a whole; the scientific publications linked from the site retain their respective publisher licenses.

### Image mapping

- `defensive-sequence.png` and `defensive-partial-dependence.png`: Defensive Gaps (the latter is published Figure 4, CC BY 4.0)
- `secondary-pass-detection.png` and `secondary-inside-out.png`: Secondary Assists
- `extra-pass-duration.png`: Extra Pass

## Planned future extension

A separate Game Momentum / Coaching Decision application can be linked as an additional project when it is ready. GitHub Pages hosts the static portfolio, not a Python backend.

## Deployment note

The GitHub Actions workflow does not enable npm caching because the starter project does not include a package-lock.json. This avoids the setup-node missing-lockfile error.

## Research-grounded editorial review (November 2026)

The three case studies have been rewritten against the full-text papers. Defensive Gaps is about identifying cutting openings, not player-choice prediction. Secondary Assists investigates ball movement and shot quality, with event extraction as the enabling technical task. Extra Pass operationalizes a missed extra-pass opportunity using conservative simulation; pass duration is only one input, not a game-play prediction.

Unpublished diagnostic plots are distinguished from published Figure 4 (PLOS ONE, CC BY 4.0). All numerical results are scoped to the papers’ datasets and validation methods. Data-provenance and reuse conditions remain a separate consideration.
