# References

This site uses **Zotero** as the source of truth for references, exported to **BibTeX** for reproducible builds.

## Workflow (Zotero → BibTeX → MkDocs)

1. In Zotero, select the collection you want to publish.
2. Right‑click → **Export Collection…**
3. Choose format **BibTeX** (or Better BibTeX if you use it).
4. Save/export to: `docs/references/library.bib` (overwrite the existing file).
5. Commit + push. GitHub Actions will rebuild the site.

## How to cite in pages

Use author‑date citation keys like this:

- `[@Ali2025]` for a single citation
- `[@Ali2025; @NIST2020]` for multiple citations

## Notes

- Keep BibTeX keys stable (especially if you use Better BibTeX with automatic keys).
- Prefer DOI where available.


## Mapped literature matrices (derived exports)

The repo also includes **derived** reference exports created from your mapped literature spreadsheets:

- `docs/references/selected-from-mapping.bib`
- `docs/references/selected-from-mapping.ris`

These are **not** the canonical Zotero export. They exist to make the literature mapping reproducible and to ensure every cited mapped item has a machine-readable reference entry, even when the original spreadsheet entry does not include a DOI.
