# Pei Wang's Academic Homepage

This repository contains the source for Pei Wang's academic homepage, built with [Jekyll](https://jekyllrb.com/) and the [Academic Pages](https://github.com/academicpages/academicpages.github.io) theme.

- Website: <https://pei-wang-cs.github.io/pei-wang.github.io/>
- ORCID: <https://orcid.org/0009-0007-0437-9141>
- GitHub: <https://github.com/pei-wang-cs>

## Content

- Site-wide metadata and sidebar: `_config.yml`
- Homepage: `_pages/about.md`
- Publications: `_publications/`
- Navigation: `_data/navigation.yml`

## Local preview

Install Ruby, Bundler, and the dependencies in `Gemfile`, then run:

```bash
bundle install
bundle exec jekyll serve --config _config.yml,_config_docker.yml --livereload
```

The site is available at <http://localhost:4000/pei-wang.github.io/>.

For a production build with stricter front-matter validation:

```bash
bundle exec jekyll build --strict_front_matter
```

## Deployment path

The repository is currently named `pei-wang.github.io`, so GitHub Pages treats it as a project site under `/pei-wang.github.io`. If the repository is renamed to `pei-wang-cs.github.io` for a root user site, change `baseurl` in `_config.yml` to an empty string.

In **Settings → Pages → Build and deployment**, set **Source** to **GitHub Actions**. The workflow in `.github/workflows/jekyll-build.yml` builds, uploads, and deploys the site; using branch deployment as well would start a redundant GitHub-generated Pages workflow.

## License

The theme is derived from Academic Pages and Minimal Mistakes under the MIT License. See `LICENSE` for details.
