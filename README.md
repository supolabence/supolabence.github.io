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

- **All five images in `public/images/` are user-provided, unpublished research visualizations**. The previous publication-page images have been removed from this project and its ZIP.
- These images are not automatically cleared for public use merely because they were not published. Before deploying, verify that the underlying NBA/SportVU tracking data and any third-party graphical elements can be displayed publicly under the applicable data access agreements.
- The extra-pass orange curves are described as quadratic fits; the figure alone does not establish that they are quantile-regression fits.
- Confirm the precise wording and context of reported model metrics against the original paper.
- Review biography and individual versus collaborative research contributions.
- No license is granted for the repository as a whole; the scientific publications linked from the site retain their respective publisher licenses.

### Image mapping

- `defensive-sequence.png` and `defensive-feature-importance.jpg`: Defensive Gaps
- `secondary-pass-detection.png` and `secondary-inside-out.png`: Secondary Assists
- `extra-pass-duration.png`: Extra Pass

## Planned future extension

A separate Game Momentum / Coaching Decision application can be linked as an additional project when it is ready. GitHub Pages hosts the static portfolio, not a Python backend.
