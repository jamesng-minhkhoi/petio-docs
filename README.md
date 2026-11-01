# Petio Docs

Source of truth for Petio's public documentation, synced to GitBook.

This repo is written for **users** (how to use the app). Contributor-facing
material lives in the app repo:
[CONTRIBUTING.md](https://github.com/jamesng-minhkhoi/petio-mobile/blob/main/CONTRIBUTING.md).

## Publishing with GitBook (one-time setup)

1. Sign in at [app.gitbook.com](https://app.gitbook.com).
2. Create an organization (e.g. `petio`).
3. In it, create a space named **Petio Docs**.
4. Space settings → **Integrations / GitHub**: connect your GitHub account,
   then sync this repo (`jamesng-minhkhoi/petio-docs`) into the space.
   GitBook mirrors the repo root; `SUMMARY.md` defines the sidebar, so edits
   to structure happen here and propagate automatically.
5. Space visibility → **Public**, and grab the public URL (likely
   `https://petio.gitbook.io/petio` or similar).
6. Update the site: replace `PETIO_DOCS_URL` in
   [`petio-landingpage/src/lib/site-links.ts`](https://github.com/jamesng-minhkhoi/petio-landingpage/blob/main/src/lib/site-links.ts)
   with the real URL (one line), and flip the `/docs` redirect to
   `permanent: true` after the URL is confirmed stable.

## Editing docs

- Commit to `main` — if sync is enabled, changes go live automatically.
- Keep user-testable facts verifiable against a real build: write what the
  app does, not what it should do. Mark anything unverified with **DRAFT**
  exactly where the current pages do.
- Screenshots go in `assets/` and are referenced by relative path
  (`![Today view](assets/home.png)`). Placeholder slots are marked in each
  page — same convention as the app README.

## Status

Content is scaffolded against the app's current feature surface. Pages marked
**DRAFT** have verified structure but unfinished copy.

## License

Petio Docs are part of the Petio project and are licensed under the
[GNU AGPL-3.0](LICENSE), matching the app.
