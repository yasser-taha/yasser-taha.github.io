# Yasser Taha — Personal Website

Source code for **[yasser-taha.github.io](https://yasser-taha.github.io)** — my personal academic website.

Built with [Hugo](https://gohugo.io) and the [Hugo Blox Academic CV](https://github.com/HugoBlox/hugo-theme-academic-cv) theme.

## Stack

- **Hugo** (extended) — static site generator
- **Hugo Blox Academic CV** — theme via Hugo modules
- **TailwindCSS v4** — styling
- **Pagefind** — client-side search
- **GitHub Actions** — CI/CD, deploys to GitHub Pages on every push to `main`

## Local development

Requires the `website` conda environment (Hugo, Go, Node.js, pnpm).

```bash
conda activate website
export PATH=$PATH:$(pwd)/node_modules/.bin
hugo server --disableFastRender --port 1313
```

## Deployment

Push to `main` — GitHub Actions builds and deploys automatically to GitHub Pages.
