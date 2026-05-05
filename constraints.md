## Maintenance notes

- Keep the site and PDF exports in sync. When updating `index.html` or `index-short.html` in `vil4max.github.io`, regenerate PDFs:
  - `npm run resume:pdf:all`
  - Optional: sanity check with `npm run resume:check`

- This repo hosts public assets (PDFs/images) referenced from the site. Keep `assets/` up to date before publishing changes.

