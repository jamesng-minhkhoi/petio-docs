# Contribute

Petio is open source under AGPL-3.0, and every kind of contribution helps.

| I want to... | Where |
|--------------|-------|
| Report an app bug | [petio-mobile issues](https://github.com/jamesng-minhkhoi/petio-mobile/issues) (bug template) |
| Suggest a feature | [petio-mobile issues](https://github.com/jamesng-minhkhoi/petio-mobile/issues) (feature template) |
| Build something | [CONTRIBUTING.md](https://github.com/jamesng-minhkhoi/petio-mobile/blob/main/CONTRIBUTING.md) |
| Translate | [Translations](translations.md) |
| Fix the docs | PRs on this repo |
| Ask a question | [Discussions](https://github.com/jamesng-minhkhoi/petio-mobile/discussions) |

## The quick version of the dev setup

```bash
git clone https://github.com/jamesng-minhkhoi/petio-mobile.git
cd petio-mobile
npm ci                      # Node 22
cp .env.example .env        # local Supabase keys (supabase start)
npx expo start
```

Validation before any PR: `npm run preflight` and `npm test`. Commits follow
Conventional Commits (enforced).

**DRAFT** — keep this page mirrored with the app repo's README and LICENSE.
