# nailpass-content

Public website and content packs for the NailPass app, served by GitHub Pages (`main`, root).

- `/` landing page, `/privacy`, `/support`, `/terms` (EN + VI)
- `v1/` content pack for schemaVersion 1. The app reads
  `https://horizon-lab-studios.github.io/nailpass-content/v1/manifest.json`.

Publishing a pack: copy the `tool/build_pack.dart` output into `v1/` and push, **manifest last**, so a half-uploaded
pack is never advertised. Never rename or move this repo once an app version is in the stores (spec §6.3).
Firebase config files never go in this repo.
