# Qingyue Jiao — personal website

A responsive, build-free academic homepage for https://qingyue-jiao.github.io/.

## Publish with GitHub Pages

1. For GitHub Free, make this repository public: **Settings → General → Danger Zone → Change repository visibility**. Review all files before doing so. The downloadable CV contains the contact details from the current resume.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, select **Deploy from a branch**.
4. Select **main** and **/ (root)**, then **Save**.
5. Wait for the Pages deployment to finish. Your site will be at https://qingyue-jiao.github.io/.

GitHub Team and Enterprise Cloud can also publish Pages from private organization repositories. Keep your repository private if your plan supports that and you prefer it.

## Update content

- `index.html`: biography, research, news, publications, and education.
- `styles.css`: typography, colors, spacing, and mobile layout.
- `assets/Qingyue_Jiao_CV.pdf`: downloadable resume. Replace this file when your resume changes.
- `assets/favicon.svg`: initials icon.
- `.nojekyll`: serves this as a plain static site.

The first version uses an initials monogram. To add a portrait, place an image in `assets/`, replace the `.monogram` div with an `img` element with descriptive alt text, and give it the same sizing and rounded shape in the stylesheet.

No JavaScript, build tools, package installation, API keys, or external fonts are required. Preview locally with `python3 -m http.server 8000`, then open http://localhost:8000.

## Content provenance

Biography, education, publications, and research summaries were prepared from `QingyueJ-nd/Resume/main.tex` (blob `bb28fcd81cc0b7a1f16131c944a04188805d6ec2`), retrieved October 6, 2026. The CV PDF was compiled from that source without content changes. MICCAI paper and code links were verified against the conference's official paper page. Publication statuses reflect the resume and should be updated as decisions arrive.

The layout takes inspiration from Minghao Guo's academic homepage, with independently written HTML and CSS. His photograph and personal content are not included. A Google Scholar profile and academic service section can be added once their details are supplied.
