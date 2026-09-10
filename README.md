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
