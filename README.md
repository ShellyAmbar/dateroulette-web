# dateroulette-web

Deploy target for the [Dateroulette](https://dateroulette.online) web app.

This repo holds no source — it's populated automatically by a GitHub
Actions workflow in the (private) `ShellyAmbar/Hive` repo, which builds
`web/` there as a Next.js static export and pushes the output to this
repo's `gh-pages` branch on every push to `Hive`'s `main` branch.

GitHub Pages serves from the `gh-pages` branch, with `dateroulette.online`
configured as the custom domain.

Source: `ShellyAmbar/Hive` → `web/`
Workflow: `ShellyAmbar/Hive` → `.github/workflows/deploy-web.yml`
