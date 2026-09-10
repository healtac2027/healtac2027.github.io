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

Served by GitHub Pages from the `main` branch using GitHub's built-in Jekyll build, the
same arrangement as the 2025 and 2026 sites (no Actions workflow). Because the repository
is named `healtac2027.github.io` inside the `healtac2027` organisation, it publishes at:

    https://healtac2027.github.io/

`_config.yml` already sets that `url` with `baseurl: /`, so pushing to `main` is all that
is needed to update the live site.
