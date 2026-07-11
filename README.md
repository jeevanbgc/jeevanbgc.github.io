# Jeevan GC — Personal Website

Personal site for [Jeevan B. GC, PhD](https://jeevanbgc.github.io/) — Senior AI Scientist working on peptide design at AbbVie.

## Preview locally

Open `index.html` in your browser, or run a simple server:

```bash
cd /Users/jeevanbgc/Documents/jeevanbgc_personal_website
python3 -m http.server 8080
```

Then visit [http://127.0.0.1:8080](http://127.0.0.1:8080)

## Deploy to GitHub Pages

1. Create a repo named `jeevanbgc.github.io` on GitHub.
2. Push this project to the `main` branch.
3. In **Settings → Pages**, set **Source** to **GitHub Actions**.
4. The site goes live at **https://jeevanbgc.github.io/**

```bash
git init
git add index.html publications.html research.html css/ .github/
git commit -m "Add personal website"
git branch -M main
git remote add origin https://github.com/jeevanbgc/jeevanbgc.github.io.git
git push -u origin main
```

## Edit content

- `index.html` — Home page (bio, education, links)
- `publications.html` — Publication list
- `research.html` — Research overview
- `css/style.css` — Styling

Update the contact email in `index.html` (currently a placeholder).

## MkDocs (optional)

The `docs/` folder contains an alternate MkDocs version. To use it:

```bash
source .venv/bin/activate
mkdocs serve
```

The static HTML site in the project root is the primary version for deployment.
