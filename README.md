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
- Homepage layout: `_layouts/home.html`
- Shared academic styling: `_sass/layout/_academic.scss`
- Publication list styling: `_sass/layout/_publications.scss`

## Layout and style

The homepage uses a compact academic layout inspired by [Shenao Wang's homepage](https://shenaow.github.io/): a sticky profile sidebar, section navigation, serif typography, and a continuous About / News / Publications page. On small screens, the profile sits above the content and contact links wrap onto multiple lines. Light and dark themes are supported.

Homepage publications are generated from `_publications/`, grouped by year with the newest first. Both the homepage and `/publications/` use compact entries; full abstracts and BibTeX remain on each paper's detail page. Adding a publication does not require duplicating its information on the homepage.

After changing JavaScript sources, regenerate the checked-in browser bundle:

```bash
npm install
npm run build:js
```

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
