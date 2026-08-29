# dss-guides

The starter guides of IQSS Data Science Services as one Quarto website: Git and
GitHub, GitHub Pages, VS Code, Emacs, LaTeX, and Overleaf, one section per
guide. Brought together in 2026 from six repositories (`git_guide`,
`github_pages_guide`, `vscode-settings`, `emacs_guide`, `latex_guide`,
`overleaf_guide`), each carried in with its history by `git subtree`. Live at
https://iqss.github.io/dss-guides/.

## Build

```sh
quarto preview   # or quarto render; needs Quarto 1.9+
```

Nothing executes, so a render needs only Quarto. The look is the `dss-theme`
extension, vendored in `_extensions/` (`quarto update IQSS/dss-theme` takes a
newer version). CI (`.github/workflows/publish.yml`) renders on every push to
`main` and publishes to `gh-pages`.

## Layout

One directory per guide (`git/`, `pages/`, `vscode/`, `emacs/`, `latex/`,
`overleaf/`), each page a `.qmd`; the sidebar in `_quarto.yml` gives the
order. On a Dropbox-synced checkout, `_site` is a symlink outside Dropbox.

## Licence

CC BY 4.0. The guides were written by Dominic Skinnion for Data Science
Services, 2024 to 2025.
