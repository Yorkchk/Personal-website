# Personal website

My personal website: who I am, my internships, projects and skills. It is a static site written in plain HTML, CSS and JavaScript, with no build step.

## Structure

| Path | What it is |
| --- | --- |
| `index.html` | The whole page: hero, about, experience, projects, skills, contact |
| `css/styles.css` | Styles, light and dark themes, responsive layout |
| `js/main.js` | Mobile menu, theme switch, active nav link, reveal on scroll |
| `assets/resume/` | The resume PDF offered for download |
| `assets/img/` | Project screenshots |

## Preview locally

```bash
python -m http.server 8000
```

Then open <http://localhost:8000>. Opening `index.html` directly in a browser also works.

## Deploy on GitHub Pages

1. Push this folder to a GitHub repository. Naming it `Yorkchk.github.io` serves the site at `https://yorkchk.github.io/`; any other name serves it at `https://yorkchk.github.io/<repo>/`.
2. In the repository, open **Settings → Pages**, choose **Deploy from a branch**, and select `main` and `/ (root)`.

All links in the site are relative, so it works at either address.

## Updating content

Everything is in `index.html`. After changing `css/styles.css` or `js/main.js`, update the `?v=` date on their tags in `index.html` so browsers load the new version instead of a cached one. To change a resume, replace the PDF in `assets/resume/` and keep the file name.
