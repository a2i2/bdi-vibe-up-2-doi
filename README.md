# Vibe Up 2.0 — Citation & Release Log

This repository is a **public citation and release-tracking record** for
**Vibe Up 2.0**, which is closed-source / proprietary software.

It does **not** contain source code. Instead, it exists so that the
software can be cited in academic work via a persistent DOI, and so that
the history of releases and their DOIs is transparent and easy to look up.

## What's in here

- [`CITATION.cff`](./CITATION.cff) — machine-readable citation metadata for the **current** release (used by GitHub's "Cite this repository" button, Zenodo, and reference managers)
- [`CHANGELOG.md`](./CHANGELOG.md) — human-readable summary of changes per release
- Release notes for each tagged version — published as [GitHub Releases](https://github.com/a2i2/bdi-vibe-up-2-doi/releases), not as files in this repository
- A version history table (below) mapping each release to its DOI

No implementation details, source code, build configs, or internal
documentation are published here. For access to the software itself,
see [Access & Licensing](#access--licensing) below.

## How to cite

To cite the current version of Vibe Up 2.0, use the metadata in
[`CITATION.cff`](./CITATION.cff), or click **"Cite this repository"** in
the sidebar of this GitHub repo.

If you need to cite a **specific past version** (e.g. because that's the
version you actually used in your research), use its DOI from the table
below rather than the current CITATION.cff, which always reflects the
latest release.

### Concept DOI (cite the project in general)

> 10.xxxx/zenodo.xxxxxxx

This DOI always resolves to the metadata for the most recent version.

## Versioning

Snapshots use CalVer in the form `yyyy.mm.micro`:

| Part | Meaning |
|------|---------|
| `yyyy` | Four-digit year of the release |
| `mm` | Two-digit month of the release |
| `micro` | Two-digit counter, starting at `01` for the first release of that month and incrementing for each further release in it |

`micro` resets to `01` at the start of every month, so the first release of
August 2026 is `2026.08.01`, a second release that month is `2026.08.02`,
and the first release of September 2026 is `2026.09.01` — not `2026.09.03`.
All parts are zero-padded.

Git tags carry a leading `v` (e.g. `v2026.08.01`); the `version` field in
[`CITATION.cff`](./CITATION.cff) and the changelog headings do not.

## Version history

Releases that predate this repository are not listed here and have no
DOI; see [`CHANGELOG.md`](./CHANGELOG.md) for that earlier history.

| Version | Release date | DOI | Release notes |
|---------|--------------|-----|----------------|
| 2026.08.01 | 2026-08-31 | _pending_ | [Notes](https://github.com/a2i2/bdi-vibe-up-2-doi/releases/tag/v2026.08.01) |

*(Add a row here each time a new version is tagged and archived. The
"Release notes" column links to that version's
[GitHub Release](https://github.com/a2i2/bdi-vibe-up-2-doi/releases) —
release notes are published there, not as files in this repository.)*

## How this log is maintained

1. A new version of Vibe Up 2.0 is released internally.
2. A git tag is pushed (e.g. `v2026.08.01` — see [Versioning](#versioning)) and a GitHub Release is published against it, with the release notes (no source) in the release body.
3. Zenodo, connected to this repository, automatically archives the tagged release and mints a new version-specific DOI.
4. `CITATION.cff` and the version history table above are updated with the new version and DOI.

## Access & Licensing

Vibe Up 2.0 is closed-source. For access, licensing, or
collaboration inquiries, please contact:

**A2I2 Admin** — [a2i2-admin@deakin.edu.au](mailto:a2i2-admin@deakin.edu.au)  
Deakin University - Applied Artificial Intelligence Initiative — [https://a2i2.deakin.edu.au](https://a2i2.deakin.edu.au)

## License

The **contents of this repository** (release notes, changelogs, and
citation metadata) are licensed under LICENSE, e.g. CC-BY-4.0.
This license applies only to the materials in this repo and does **not**
extend any rights to the Vibe up 2.0 software itself, which
remains proprietary and is governed by its own license terms.
