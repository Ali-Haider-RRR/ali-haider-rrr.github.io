# LydraCare link pages (GitHub Pages)

These files make a senior's invite link open the app reliably.

Publish them as the ROOT of a GitHub repo named exactly `<your-github-username>.github.io`
(lowercase), e.g. `ali-haider-rrr.github.io`. Then edit two things:

1. `.well-known/assetlinks.json` — replace `REPLACE_WITH_SHA256_FROM_EAS_CREDENTIALS` with your build's
   SHA-256 certificate fingerprint (from `eas credentials`).
2. `404.html` and `index.html` (identical copies) — replace `PASTE_YOUR_PREVIEW_APK_LINK_HERE` with your
   preview APK download link (optional — the install button stays hidden until you do).

Keep `.nojekyll` — without it GitHub Pages hides the `.well-known` folder and Android can't verify the link.

Full step-by-step guide: `../docs/deep-links-setup.md`.
