# Lion Trans — website redesign concept

Two design directions for [liontrans.com](https://liontrans.com), built from the site's own content.

| | |
|---|---|
| **[index.html](https://sallylomtadze-cmyk.github.io/liontrans-redesign/)** | Dark "control room" direction — interactive globe with the holding's 22 offices, live shipping-lane readout, scale car-carrier, animated buying instruction, live auction lots |
| **[clean.html](https://sallylomtadze-cmyk.github.io/liontrans-redesign/clean.html)** | Light editorial direction — wide margins, large type, photography-led |

Bilingual (ქართული / English). Switch with the toggle in the header.

## Where the content comes from

- **Copy** — the live site's own i18n bundle (`main.*.chunk.js`), 1005 strings per language, so KA and EN stay in sync
- **Offices** — all 22 offices in 14 countries with coordinates, addresses and phones, from the site's own data module
- **Lots** — 8 live lots (photos, prices, specifications) from `api.liontrans.com/api/Product/GetPublicOneLotPageData`
- **Logo** — the company's own mark
- **Car render** — generated for this mock-up; not a real vehicle photograph

Nothing on these pages is invented: numbers, addresses and specifications are taken from Lion Trans's own site and API.

## Build

Single-file pages. Every asset (map geometry, logo, photographs) is inlined as a data URI; the only external dependencies are d3 and Google Fonts.
