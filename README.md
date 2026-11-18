# wellcheck-terms-of-service

Privacy policy and terms of service for 잘지내지 (well-check v2). Korean only.

| Page | Source | Path | Status |
| --- | --- | --- | --- |
| Index | `index.md` | `/` | published |
| Signal app privacy policy | `signal-app/privacy.md` | `/signal-app/privacy/` | published |
| Signal app terms of service | `signal-app/terms.md` | `/signal-app/terms/` | published |
| Mini app (guardian) privacy policy v1.0 draft | `privacy.md` | `/privacy/` | `published: false` until mini app v2 launches |
| Mini app (guardian) terms of service v2.0 draft | `terms.md` | `/terms/` | `published: false` until mini app v2 launches |
| Mini app terms 2026-02-18 (v1 alimtalk service, still in force for the mini app) | `archive/terms-2026-02-18.md` | `/terms/2026-02-18/` | published |

Scope split (user decision 2026-11-18): the Android signal app ships first with its own documents covering only the phone owner. The mini app documents cover the guardian and are published together with mini app v2; when they go live, remove `published: false`, link them from `index.md`, and keep the signal-app documents consistent with them.

## Hosting

Cloudflare Pages, connected to this GitHub repository (not GitHub Pages). Domain: `https://wellcheck.rooftopguys.com` (custom domain on the `rooftopguys.com` Cloudflare zone). Customer-support address `wellcheck-support@rooftopguys.com` is a Cloudflare Email Routing address forwarded to the representative's Gmail inbox; both values live in `_config.yml`.

- Production branch: `main`
- Framework preset: Jekyll
- Build command: `bundle exec jekyll build`
- Build output directory: `_site`
- Ruby version: `.ruby-version`

## Editing rules

- Text marked `〔확인 필요: …〕` is undecided. Do not publish to production while any marker remains.
- On every change, bump the version and effective date at the top of the page and add a row to `변경 이력`.
- Keep the privacy policy consistent with the signal app's in-app disclosure (O2) in the main repository: same items, same 30-day retention, no 감시/모니터링/추적 wording.
