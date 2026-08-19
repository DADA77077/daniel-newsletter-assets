# daniel-newsletter-assets

Public image host for Daniel Hershkovitz's **personal** newsletters (Rav-Messer).
Permanent + automatic: drop a file here, `git push`, and it is live on the jsDelivr CDN
at a stable HTTPS URL that renders in every email client (Gmail included).

## URL pattern

```
https://cdn.jsdelivr.net/gh/DADA77077/daniel-newsletter-assets@main/<path>
```

Example:
`https://cdn.jsdelivr.net/gh/DADA77077/daniel-newsletter-assets@main/assets/daniel-circle.png`

## Layout

- `assets/` — permanent, reused across every issue (e.g. `daniel-circle.png`, the round photo).
- `<YYYY-MM-DD-slug>/` — per-issue images (e.g. `2026-08-19-busha/signoff.png`).

## Add an image (the automatic flow)

1. Copy the file into `assets/` (reusable) or a dated issue folder (one-off).
2. `git add -A && git commit -m "add <name>" && git push`
3. Use the jsDelivr URL above in the Rav-Messer "קוד AI חיצוני" HTML.

Notes: filenames are effectively immutable — a new image gets a new name, so CDN caching
never serves a stale version. Only public, send-to-the-whole-list newsletter images live here;
nothing private.
