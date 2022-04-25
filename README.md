# MatomoBoard

Compile your matomo metrics in a single static web interface

Demo : https://socialgouv.github.io/matomoboard

## How it works

- a scheduled github action fetch data from your matomo API every hour and store the result in GIT
- a website is rendered from this data and published to the repo `gh-pages` branch to make it available at `https://[USER].github.io/matomoboard`

## Setup

- Click "Use this template" from the [template repo](https://github.com/socialgouv/matomoboard) to create your own GitHub repo

- In your Github Repo settings:

  - Enable "Pages" on the `gh-branch`
  - Add `MATOMO_URL` and `MATOMO_TOKEN` in the `secrets` section

- Run the `Update data` Github workflow from the repo `Actions` Tab to get the first render

💡 The `MATOMO_TOKEN` can be obtained from matomo Settings/Personal/Security panel.

## Dev

Check the [matomoboard-actions](https://github.com/socialgouv/matomoboard-actions) repo for the code;
