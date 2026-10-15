# BNM Monthly Highlights & Statistics (MHS) archive

An archive of the data files published in Bank Negara Malaysia's *Monthly Highlights & Statistics*
(formerly *Monthly Statistical Bulletin*), January 1998 to August 2026. Snapshot taken 2026-10-15.

This is an unofficial archive and is not affiliated with or endorsed by Bank Negara Malaysia.

## Contents

| What | Where |
|---|---|
| Download-link dictionary: every file linked from each monthly page (344 months, 76,321 links, 76,314 unique files) | [`Dictionary/`](Dictionary/) |
| The data files themselves: 29 annual ZIPs, 2.64 GiB in total | [Release `mhs-archive-2026-10-15`](../../releases/tag/mhs-archive-2026-10-15) |
| Files that could not be retrieved (21) | [`unavailable_files.md`](unavailable_files.md) / [`.csv`](unavailable_files.csv) |
| Files recovered after the snapshot (6 entries, 8 files), not yet in the Release | [`recovered/`](recovered/) |

### Dictionary

- `Dictionary/<YYYY>/MHS_Links_<MM>.csv`: one row per download link on that month's page, in page
  order, with columns `row` (the table row's text), `filename`, `linkText` and `url` (exactly as linked).
- `Dictionary/MHS_Links_status_<YYYY>.csv`: the article page each month was read from and its link count.
- `Dictionary/MHS_Links_audit_2025.csv` and `Dictionary/mapping/`: records from early catalogue runs, kept
  for provenance.

### Archive (Release assets)

- `MHS_<YYYY>.zip`: every valid file for that year at `MHS/<YYYY>/<MM>/<filename>`. Unzipping several
  years into one folder merges them into a single `MHS/` tree.
- `SHA256SUMS`: SHA-256 of each ZIP. Check with `shasum -a 256 -c SHA256SUMS` (macOS) or
  `sha256sum -c SHA256SUMS` (Linux).
- `MHS_manifest.csv`: size and SHA-256 of every file inside the ZIPs.

All 76,287 archived files passed file-signature checks (PDF, Excel 97-2003, or Excel
workbook with an intact ZIP container). Error pages and challenge pages were rejected. Files that
could not be retrieved are listed, not substituted.

## Source and terms

Source: Bank Negara Malaysia. Data compiled by Bank Negara Malaysia is reused under its
[Terms of Use for BNM Datasets](https://www.bnm.gov.my/terms-of-use-bnm-datasets). Some tables name
another compiler as their source (for example the Department of Statistics, Malaysia). Those remain
subject to the [Terms of Use for the BNM website](https://www.bnm.gov.my/terms-of-use) and to their
compiler's terms. Check the source shown in each table before reusing it.
