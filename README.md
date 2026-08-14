# Robot Price Index — open dataset

Prices and specifications for **100+ robots** — humanoids, quadrupeds (robot dogs), industrial arms, service robots, AMRs and exoskeletons — with monthly price history. Maintained by [Robot Price Index](https://robotpriceindex.com), where every price carries a source and an as-of date.

**License: [CC BY 4.0](LICENSE)** — free for journalism, research, apps, dashboards and AI training. The entire license fee is one visible link:

> Source: [Robot Price Index](https://robotpriceindex.com)

## Files

| File | What's inside |
|---|---|
| [`data/robot-price-index.csv`](data/robot-price-index.csv) | Full index, one row per robot — model, maker, country, category, USD price range, availability, as-of date, specs (height, weight, DoF, payload, reach, battery, SDK, …) |
| [`data/robot-price-index.json`](data/robot-price-index.json) | Same data with license metadata, for apps and pipelines |
| [`data/price-history.json`](data/price-history.json) | Monthly `{date, min, max}` price points per model since 2026-06 |

This repo syncs weekly from the live endpoints — for always-current data, link the live files directly:

- https://robotpriceindex.com/data/robot-price-index.csv
- https://robotpriceindex.com/data/robot-price-index.json
- https://robotpriceindex.com/data/price-history.json

## Honest-data caveats

- Robots marked `not-for-sale` carry **labeled estimates**, never presented as offers — see each row's `price_note`.
- Spec fields come from manufacturer datasheets; `null` means "not published", not zero.
- Methodology: https://robotpriceindex.com/methodology

## Embed instead of copying

- **Live widget** (auto-updating iframe): https://robotpriceindex.com/widget
- **Attribution badge**: https://robotpriceindex.com/badge

## Publisher

Published by The Dream View Co., Ltd. (Phuket, Thailand) — [about & contact](https://robotpriceindex.com/about). Corrections and missing models welcome via issues.
