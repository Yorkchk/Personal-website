# Personal website

My personal website: who I am, my internships, projects and skills. It is a static site written in plain HTML, CSS and JavaScript, with no build step.

**Live site: [yorkchk.github.io/Personal-website](https://yorkchk.github.io/Personal-website/)**

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

The site is served by GitHub Pages from the `main` branch of this repository:

1. In the repository, open **Settings → Pages**, choose **Deploy from a branch**, and select `main` and `/ (root)`.
2. It is then live at <https://yorkchk.github.io/Personal-website/>.

All links in the site are relative, so it also works unchanged on a custom domain. Once one is set in **Settings → Pages → Custom domain**, the address above redirects to it.

## Updating content

Everything is in `index.html`. After changing `css/styles.css` or `js/main.js`, update the `?v=` date on their tags in `index.html` so browsers load the new version instead of a cached one. To change the resume, replace `assets/resume/Youssef_Cherkaoui.pdf` and keep the file name; visitors download it as `Youssef_Cherkaoui.pdf`.
