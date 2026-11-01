# Security and privacy

## Reporting a vulnerability

Never open a public issue. Use
[GitHub private vulnerability reporting](https://github.com/jamesng-minhkhoi/petio-mobile/security)
on the petio-mobile repo. Full details: [SECURITY.md on the app repo](https://github.com/jamesng-minhkhoi/petio-mobile/blob/main/SECURITY.md).

## How your data works

- Your data (profiles, records, documents, memories) is stored in Petio's
  cloud (Supabase: Postgres, Auth, and encrypted Storage), scoped per
  household, so only household members can access it.
- Assistant conversations are processed to serve you answers. TODO: verify
  and document exactly what is stored and for how long, mirroring the
  [privacy policy](https://www.petiogo.com/privacy).
- Deleting your account removes your data: TODO verify and document the
  deletion flow here and link the privacy policy sections.

## Backups are your job

Petio backs up your *content* to your account, but exporting family memories
you especially care about is always wise.

**DRAFT** — verify against the build + privacy policy before publish.
