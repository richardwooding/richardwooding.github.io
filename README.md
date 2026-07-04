# richardwooding.github.io

My personal developer site — [richardwooding.github.io](https://richardwooding.github.io/).

A self-contained static site built in the [gloam](https://github.com/richardwooding/gloam)
design language, featuring my open-source projects in a carousel.

- Source lives in `docs/` (linked-mode gloam: `gloam.css` / `gloam.js` are vendored).
- Deployed to GitHub Pages via `.github/workflows/pages.yml` (GitHub Actions).
- `.github/workflows/gloam-sync.yml` opens a weekly PR when the vendored gloam assets
  drift from upstream; `docs/.gloam-version` records the synced commit.

To refresh the gloam assets manually: `sh docs/sync-gloam.sh docs main`.
