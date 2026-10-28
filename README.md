# DOI in Summary — OJS 3.4 fork

Displays article DOI links in issue tables of contents and homepage article summaries.
This `stable-3_4_0` line is maintained by ojs-inator, based on the Lepidus DOI in Summary plugin (GPL-3.0).

## Compatibility and release

- OJS **3.4.x**: this branch, version **2.0.0.1**, with English, Brazilian Portuguese, and Persian plugin metadata.
- OJS **3.5.x**: use the separate `main` branch (3.x); do **not** install 3.x on OJS 3.4.
- OJS 3.3.x: upstream's separate `stable-3_3_0` branch.

The 2.0.0.1 changes are localized metadata and release documentation; the OJS 3.4 PHP runtime, templates, styles, registration identity and install layout remain unchanged from 2.0.0.0. No schema or settings migration is required.

## Installation

For managed ojs-inator deployments, use the pinned OJS 3.4 Gallery plugin bundle and explicitly apply/replay it through OJS Toolkit. Bundle installation alone does not enable the plugin per journal.

To install manually, upload a release package with root folder `doiInSummary` via **Settings → Website → Plugins → Upload a new plugin**, then enable it for the journal. Avoid packaging the enclosing GitHub repository name as the plugin folder.

## Validation

The `ojs34-checks` workflow checks plugin metadata, English/Persian translation keys, PHP syntax and the OJS 3.4 entrypoint. The existing Cypress test exercises DOI display with a populated DOI against a running OJS fixture; run that integration test before deploying to production.

## License

GPL-3.0; based on the work of Lepidus Tecnologia, copyright 2015–2023.
