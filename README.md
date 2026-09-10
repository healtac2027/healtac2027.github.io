# healtac2027.github.io

Draft website for **HealTAC 2027**, the 10th Healthcare Text Analytics Conference.

Based on the [Minimal Mistakes Jekyll theme](https://github.com/mmistakes/minimal-mistakes).

## Status

This is a draft. It was seeded from the HealTAC 2026 site and reset for 2027: all
year-specific content (dates, venue, theme, keynotes, programme, committees, registration
fees, sponsors) is marked *TBC* and needs filling in as it is confirmed.

## Local preview

```sh
bundle install
bundle exec jekyll serve
```

## Deployment

`.github/workflows/pages.yml` builds the site and deploys it to GitHub Pages on every push
to the `healtac2027-draft` branch, and can also be run manually from the Actions tab. The
workflow overrides `url` and `baseurl` at build time, so `_config.yml` can keep pointing at
the site's final home (`https://healtac2027.github.io/`) while the draft is served from
whichever repository hosts it.

**One-time setup required.** Before the first deploy succeeds, enable Pages on this
repository: *Settings -> Pages -> Build and deployment -> Source: **GitHub Actions***. This
cannot be automated, because creating a Pages site needs admin rights that the workflow's
`GITHUB_TOKEN` does not have. Once it is set, re-run the workflow from the Actions tab and
the draft is served at:

    https://leo-zhang-xinyue.github.io/healtac2027.github.io/

For the conference's real home, create a `healtac2027` GitHub organisation with a
`healtac2027.github.io` repository, as was done for 2025 and 2026; the site then serves at
`https://healtac2027.github.io/` and `_config.yml` already points there.
