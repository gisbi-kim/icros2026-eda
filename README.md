# ICROS 2026 Institution & Author Analytics

Static dashboard for the 2026 제41회 제어·로봇·시스템학회 학술대회 institution and author participation summary.

## Links

- Hosted dashboard: https://gisbi-kim.github.io/icros2026-eda/
- Conference site: https://2026.icros.org
- Source workbook: [`source_data.xlsx`](source_data.xlsx)

## What This Shows

The dashboard summarizes conference participation by institution and author:

- institution ranking by participating paper count
- institution ranking by unique author count
- institution type summary
- scatter plot of participation scale
- searchable author database with paper IDs, paper titles, sessions, and affiliations

## Counting Notes

- Paper IDs in the `Pxxxxx` format are used as the paper/presentation unit.
- Unique authors are counted per institution.
- If the same paper includes multiple institutions, each listed institution receives one participating-paper count.
- For that reason, institution-level or type-level paper-count sums can be larger than the number of globally unique papers.
- Author and institution normalization is based on the source workbook and may still reflect spelling or affiliation variants present in the submitted metadata.

## Files

- `index.html`: single-file static dashboard
- `source_data.xlsx`: source workbook used for the exported dashboard
- `.nojekyll`: keeps GitHub Pages from applying Jekyll processing

## Local Preview

```bash
python3 -m http.server 8765
```

Then open:

```text
http://127.0.0.1:8765/
```
