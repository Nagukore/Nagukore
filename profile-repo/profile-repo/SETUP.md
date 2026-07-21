# Setup Notes

This repo is ready to drop into your `Nagukore/Nagukore` profile repository as-is, with one manual step.

## 1. Files
Copy everything into the root of your profile repo (the repo named exactly `Nagukore`, same as your username):

```
README.md
assets/
.github/workflows/snake.yml
.github/workflows/metrics.yml
```

## 2. Snake animation workflow (`snake.yml`)
No setup required — it uses the default `GITHUB_TOKEN` that Actions provides automatically.

- On first run (or `workflow_dispatch`), it generates the contribution snake and pushes it to an `output` branch.
- The README already references:
  `https://raw.githubusercontent.com/Nagukore/Nagukore/output/github-contribution-grid-snake.svg` (and the `-dark` variant).
- If your default branch isn't `main`, update the `branches:` trigger in `snake.yml` accordingly.

## 3. Metrics workflow (`metrics.yml`)
This one needs a **Personal Access Token**, because the default `GITHUB_TOKEN` can't read your full profile/activity data.

1. Go to **GitHub → Settings → Developer settings → Personal access tokens → Fine-grained tokens** (or classic).
2. Create a token with at least: `read:user`, `repo` (public repos is enough if all your repos are public).
3. In your profile repo: **Settings → Secrets and variables → Actions → New repository secret**.
4. Name it `METRICS_TOKEN` and paste the token value.
5. Run the workflow once manually (Actions tab → *Generate Metrics Dashboard* → *Run workflow*) to generate `metrics.svg` on first use.

If you'd rather skip this, the README doesn't hard-depend on `metrics.svg` — it isn't currently embedded — so you can delete `metrics.yml` with no broken links. Add `![metrics](./metrics.svg)` under **GitHub Analytics** in `README.md` once you've generated it, if you want it visible.

## 4. Enable Actions
Make sure **Settings → Actions → General → Workflow permissions** is set to **"Read and write permissions"**, or the snake workflow won't be able to push to the `output` branch.

## 5. Verify
After the first successful run of `snake.yml`, check that the `output` branch exists and contains the `.svg`/`.gif` files — then the snake animation in your README will render.
