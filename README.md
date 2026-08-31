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

## Version history

No version has been tagged and archived yet, so there are no DOIs to
list. See [`CHANGELOG.md`](./CHANGELOG.md) for the release history of the
apps in the meantime.

| Version | Release date | DOI | Release notes |
|---------|--------------|-----|----------------|
| — | — | — | — |

*(Add a row here each time a new version is tagged and archived. The
"Release notes" column links to that version's
[GitHub Release](https://github.com/a2i2/bdi-vibe-up-2-doi/releases) —
release notes are published there, not as files in this repository.)*

## How this log is maintained

1. A new version of Vibe Up 2.0 is released internally.
2. A git tag is pushed (e.g. `v2026.08.31`) and a GitHub Release is published against it, with the release notes (no source) in the release body.
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
