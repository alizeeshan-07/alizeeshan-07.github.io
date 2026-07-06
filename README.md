# alizeeshan-07.github.io

Personal academic site built with [Hugo](https://gohugo.io) + the
[Blowfish](https://blowfish.page) theme (theme vendored in `themes/blowfish`,
so no submodule setup is needed). GitHub Actions builds and deploys on every
push to `main`.

## Deploy (one time)

1. Create/confirm the repo `alizeeshan-07.github.io` on GitHub.
2. From this folder:
   ```bash
   git init && git add -A && git commit -m "Personal site (Hugo + Blowfish)"
   git branch -M main
   git remote add origin https://github.com/alizeeshan-07/alizeeshan-07.github.io.git
   git push -u origin main
   ```
3. On GitHub: **Settings → Pages → Build and deployment → Source = GitHub Actions**.
4. Wait for the "Deploy Hugo site to Pages" action to finish. Site goes live at
   https://alizeeshan-07.github.io/

## Fill in the placeholders

- **Photo:** replace `assets/img/author.jpg` with a square headshot.
- **CV:** replace `static/cv.pdf` with your real CV (keep the filename).
- **Social links:** in `config/_default/languages.en.toml`, add your Google
  Scholar / ORCID / X URLs and uncomment those lines.
- **Publications:** edit `content/publications.md` (a per-paper template is in
  the comments there).
- **Text:** `content/_index.md` (home), `content/about.md`, `content/research.md`.

## Local preview (optional)

Install Hugo **extended**, then:
```bash
hugo server
```
