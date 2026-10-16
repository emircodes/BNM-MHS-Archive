# Unavailable MHS files (22)

Snapshot 2026-10-16. These 22 of the 76,484 files listed in the Dictionary could not be retrieved as valid files from Bank Negara Malaysia's website, so they are not in the Release archive. Each URL is exactly as recorded in the Dictionary, including any double or trailing slashes.

| Failure | Count |
|---|---|
| HTTP 404 | 20 |
| Corrupt content | 1 |
| Connection dropped | 1 |

- **HTTP 404:** BNM returns *not found* for the exact URL linked from its own page.
- **Corrupt content:** BNM serves the file, but its content is not a valid spreadsheet.
- **Connection dropped:** BNM starts sending the file, then resets the connection on every attempt. A later retry may succeed.

The same data is often available in another format from the same table row (for example the PDF next to an XLS). Machine-readable copy: [`unavailable_files.csv`](unavailable_files.csv).

Six files from the original list of 27 were recovered after the snapshot, from the Wayback Machine or from another URL on BNM's site. They are in [`recovered/`](recovered/) and, from the 2026-10-16 snapshot, in the Release ZIPs.

| # | Month | Table | Filename | Original URL | HTTP | Failure | Observed reason |
|---|---|---|---|---|---|---|---|
| 1 | 2004-11 | IV.3 Leasing Companies: Statement of Assets and Liabilities | `iv_03.xls` | [https://www.bnm.gov.my/documents/20124/517360/iv_03.xls](https://www.bnm.gov.my/documents/20124/517360/iv_03.xls) | 200 | Corrupt content | BNM returns HTTP 200 with 37,888 bytes that are all zeros (no file signature), so it fails validation; a copy saved manually from a browser was identical (SHA-256 132fde08d7f788dece120e98bf6c794bafb655959764798ead053b872d097638) and has been discarded |
| 2 | 2010-02 | 1.2 Currency in Circulation by Denomination | `1.2.xls` | [https://www.bnm.gov.my/documents/20124/392355/1.2.xls](https://www.bnm.gov.my/documents/20124/392355/1.2.xls) | 200 | Connection dropped | BNM returns HTTP 200 but resets the connection mid-download (curl error 92) on every attempt |
| 3 | 2014-07 | 6. Glossary | `x_en.pdf` | [https://www.bnm.gov.my/files/publication/msb/2014/7/x_en.pdf](https://www.bnm.gov.my/files/publication/msb/2014/7/x_en.pdf) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 4 | 2020-04 | 1.3 Monetary Aggregates: M1, M2 and M3 | `1.3.xls` | [https://www.bnm.gov.my/documents/20124/933258/1.3.xls](https://www.bnm.gov.my/documents/20124/933258/1.3.xls) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 5 | 2020-04 | 3.5.4 Production of Major Agricultural and Mining Commodities | `3.5.4.xls` | [https://www.bnm.gov.my/documents/20124/933258/3.5.4.xls](https://www.bnm.gov.my/documents/20124/933258/3.5.4.xls) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 6 | 2020-11 | 6. Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/2137598/x_en.pdf](https://www.bnm.gov.my/documents/20124/2137598/x_en.pdf) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 7 | 2020-12 | 6. Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/2432443/x_en.pdf](https://www.bnm.gov.my/documents/20124/2432443/x_en.pdf) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 8 | 2021-06 | 1.9.6 Banking System: External Assets and External Liabilities (discontinued) | `1.9.6.xls` | [https://www.bnm.gov.my/documents/20124/4196742/1.9.6.xls](https://www.bnm.gov.my/documents/20124/4196742/1.9.6.xls) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 9 | 2021-06 | 5.1 List of Banking Institutions (discontinued) | `5.1.xls` | [https://www.bnm.gov.my/documents/20124/4196742/5.1.xls](https://www.bnm.gov.my/documents/20124/4196742/5.1.xls) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 10 | 2022-03 | 1.29 Banking System: Constituents of Capital | `1.29.xls` | [https://www.bnm.gov.my/documents/20124/6982294/1.29.xls](https://www.bnm.gov.my/documents/20124/6982294/1.29.xls) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 11 | 2022-05 | 1.6 Bank Negara Malaysia's Special Funds | `1.6.xls` | [https://www.bnm.gov.my/documents/20124/7587411/1.6.xls](https://www.bnm.gov.my/documents/20124/7587411/1.6.xls) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 12 | 2023-10 | 3.2 RENTAS- Foreign Holdings in Debt Securities and Sukuk | `3.2.xlsx` | [https://www.bnm.gov.my/documents/20124/12592033//3.2.xlsx](https://www.bnm.gov.my/documents/20124/12592033//3.2.xlsx) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 13 | 2023-12 | 6.1 Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/13352988/x_en.pdf](https://www.bnm.gov.my/documents/20124/13352988/x_en.pdf) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 14 | 2024-01 | 6.1 Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/13645389/x_en.pdf](https://www.bnm.gov.my/documents/20124/13645389/x_en.pdf) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 15 | 2024-05 | 6.1 Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/14880342/x_en.pdf](https://www.bnm.gov.my/documents/20124/14880342/x_en.pdf) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 16 | 2024-12 | 1.29b Banking System: Constituents of Capital (previous format) (discontinued) | `1.29b.xlsx` | [https://www.bnm.gov.my/documents/20124/17034696/1.29b.xlsx](https://www.bnm.gov.my/documents/20124/17034696/1.29b.xlsx) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 17 | 2025-03 | 3.6.13.2 Portfolio Investment (Liabilities) Position By Blocks of Countries | `3.6.13.2.xlsx` | [https://www.bnm.gov.my/documents/20124/17937204/3.6.13.2.xlsx](https://www.bnm.gov.my/documents/20124/17937204/3.6.13.2.xlsx) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 18 | 2026-04 | 1.6 Bank Negara Malaysia's Special Funds | `1.6.xlsx` | [https://www.bnm.gov.my/documents/20124/21942589/1.6.xlsx](https://www.bnm.gov.my/documents/20124/21942589/1.6.xlsx) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 19 | 2026-05 | 6.1 Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/22265698/x_en.pdf/](https://www.bnm.gov.my/documents/20124/22265698/x_en.pdf/) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 20 | 2026-06 | 6.1 Glossary | `x_en.pdf` | [https://www.bnm.gov.my/documents/20124/22576999/x_en.pdf/](https://www.bnm.gov.my/documents/20124/22576999/x_en.pdf/) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 21 | 2026-07 | 1.6 Bank Negara Malaysia's Special Funds | `1.6.xlsx` | [https://www.bnm.gov.my/documents/20124/22857146/1.6.xlsx](https://www.bnm.gov.my/documents/20124/22857146/1.6.xlsx) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
| 22 | 2026-08 | 1.6 Bank Negara Malaysia's Special Funds | `1.6.xlsx` | [https://www.bnm.gov.my/documents/20124/23200938/1.6.xlsx/](https://www.bnm.gov.my/documents/20124/23200938/1.6.xlsx/) | 404 | HTTP 404 | BNM returns HTTP 404 for the exact Dictionary URL |
