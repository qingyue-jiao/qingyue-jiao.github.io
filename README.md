# Qingyue Jiao — academic website

Academic Pages / Jekyll website for https://qingyue-jiao.github.io.

## Publish with GitHub Pages

For GitHub Free, make this repository public. In Settings → Pages, choose **Deploy from a branch**, branch **main**, folder **/(root)**, then Save. A paid organization plan may support Pages from a private repository. No `.nojekyll` file should be present: this site requires Jekyll.

## Update content

- `_pages/about.md`: biography, research interests, news.
- `_pages/research.md`: six research projects.
- `_data/publications.json`: publications, authors, status, and links.
- `_data/featured.json`: publication IDs featured on the homepage.
- `_includes/education.html`: education shared by About and CV.
- `_pages/cv.md`: CV overview and skills.
- `files/Qingyue_Jiao_CV.pdf`: downloadable resume.
- `_config.yml`: name, profile links, metadata, and optional portrait path.
- `assets/css/personal.css`: responsive visual styling.

Add a portrait under `images/` and set `author.avatar` to its path in `_config.yml`.

## Local preview

Install Ruby and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open http://localhost:4000. Run `bundle exec jekyll build` for a production build.

## Theme

Uses [Academic Pages](https://github.com/academicpages/academicpages.github.io), pinned to commit `c089e79c7bce7ff453de525bc0bb80c261400cf6` through `jekyll-remote-theme`. Local files override the theme's navigation, author profile, typography, and content. Upstream layouts, Sass, and assets are provided by the theme. The MIT license is retained.
