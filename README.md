# caddiebot-packs

Course data packs for **CaddieBot**, a personal phone-only Android golf GPS app. The app downloads these files; nothing here is an app build.

## What is published
Each course is one zip, attached to a [GitHub release](../../releases) (not stored in the git tree):

- `<course>-v<N>.zip`: `manifest.json` (per-file sha256), `course.json` (green / bunker / fairway / water / tee outlines, hole lines), `greens.json` (front / middle / back), `card.json` (scorecard), `elev.json` (elevation grid), `hole_images.json` (image frames) and `holeN.webp` (per-hole aerial image).
- `index.json`: list of courses with id, name, version, size, sha256, first-tee coordinates and the pack download URL. The app fetches it from `releases/latest/download/index.json`.

New pack versions are published as new releases with an updated `index.json`.

## Courses (v1)
Orchard Hills Golf Course (9 holes) and Paramus Golf Course (18 holes), Paramus, NJ. Paramus scorecard yardages are third-party and marked unverified.

## Licence and attribution
- Course geometry: (c) [OpenStreetMap](https://www.openstreetmap.org/copyright) contributors, available under the [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/). The geometry in these packs is a derived database (aligned/corrected against imagery) and is offered here under the ODbL.
- Aerial imagery: NJ OGIS 2020 orthophotography (State of New Jersey, public data), resampled and cropped per hole.
- Elevation: USGS 3DEP (public domain).
- Scorecard data: yardage, par and handicap facts with their source noted in each `card.json`.

No personal data and no secrets are stored here.
