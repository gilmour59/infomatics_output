# Dataset Inventory and Preliminary Feasibility — 2026-10-11

**Status:** Initial inventory and selected native Google Sheets metadata/sample-row inspection only; not a complete statistical data audit. Source folders are read-only.

## Rice — source folder
https://drive.google.com/drive/folders/1LoTjXaEkn69dNkXF-kReowymCqu7T7PB

| Source | Initial suitability | Caveat |
|---|---|---|
| PSA AnnualProduction_Harvested-WesternVisayas | High: year/province/irrigation-type harvested area, yield and production; additional quarterly/geographic tabs | Confirm reporting completeness, annual aggregation and geographic revisions |
| NORMALIZED - Monthly Planting, Harvesting and Yield Data - All Seed Types 2019-2026 | Promising for seasonality | Despite filename, inspected sheet contains 2016 onward; wide format and multirow headings; verify relationships before use |
| Monthly Planting, Harvesting and Yield Data - All Seed Types 2019-2026 | Potential provenance/cross-check | Check duplication versus normalized copy |
| NORMALIZED - Per Season Harvest and Production, Planting | Promising supplementary seasonal source | NORMALIZED tab sampled is an index/link table, not a ready tidy fact table; check summary tabs |
| Rice Program Budget Summary from CY-2019-2026 | Optional explanatory/context data | Avoid implying causation from ecological/time-series correlations |
| Summary of Disaster Damages in Western Visayas (RICE) C.Y. 2010-Present.xlsx | Optional risks/anomaly factor | Excel not yet profiled; test location/date comparability |
| Seed Utilization 2016-2024 LGU Report | Optional explanatory/context data | Validate location/year matching |
| Sufficiency Level 2018-2026 | Potential outcome/context | Folder not yet traversed |
| Annual/Normalized planting and harvest/production folders | Potential panel sources | Folder contents not yet traversed |
| Cost Structure (Rainfed and Irrigated) | Optional economic study | Folder not yet traversed |

**Observed annual sheet fields:** Year, Province, irrigated/rainfed and total harvested area (ha), yield (Mt/ha), production (Mt). Sample shows 2026 lower than 2025; may be partial-period reporting—must verify before drawing trends.

**Tentative research angle:** Agricultural production/yield pattern discovery, then evaluate clustering/regression/forecasting based on verified observation count and quality. Do not claim predictions are feasible before quality checks.

## High Value Crops — source folder
https://drive.google.com/drive/folders/1WL307G7M2ARRC55f3_OlXOUdiRqN4_6Q

| Source | Initial suitability | Caveat |
|---|---|---|
| FRUIT TREES and OTHERS_FY 2024 (Google Sheets) | Potential baseline for geographic/monthly crop patterns | 11 tabs, mixed consolidated/province layouts, complex multirow headers |
| FY 2025_FRUIT TREES and OTHERS.xlsx | Cross-year evidence needed | Excel file; data not yet inspected |
| FY 2026_FRUIT TREES and OTHERS (Google Sheets) | Promising recent commodity detail | Eight tabs, extremely wide sheets (974 columns), multiple header levels, summary rows |

**Observed 2026 columns:** province/municipality, month; crop types such as cacao Criollo and Forastero; commercial/backyard production; male/female/total farmers; bearing/non-bearing/mortality tree counts; newly/existing/total planted area (ha); harvested area (ha); production volume (MT); remarks.

**Observed 2024 fruit-trees columns:** province, month, commodities such as mango, avocado, guyabano, jackfruit, lanzones, mangosteen, rambutan, tamarind and chico with bearing trees, non-bearing trees, area planted/harvested, and volume produced.

**Key feasibility gate:** Normalize a record to (year, month, province/municipality, crop, production system/category) if those dimensions can be consistently recovered, preserving original definitions. Verify 2025 first; check whether 2024 vs 2026 commodity and metric definitions are genuinely comparable. Consider focused cacao study only if adequate coverage.

## Safeguards
- No source edits, no re-sharing and no raw data uploaded to GitHub.
- Confirm institutional permission before sharing any derivative outputs.
- Data discrepancies and unsupported claims stay flagged, not silently repaired.
- Model selection, metrics and minimum thresholds will be set before final model evaluation.

## Follow-up inventory (2026-10-11)
Immediate Rice subfolders examined: Sufficiency Level contains two PSA Excel files (WV 2018–2025, Panay 2018–2026); Annual Planting contains 2016–2025 yearly Sheets and seasonal subfolder; Annual Harvest and Production contains 2016–2025 yearly Sheets and seasonal subfolder; normalized Planting and Harvest/Production groups each contain three deeper folders (season, quarterly/semester/annual, monthly/annual); Cost Structure contains regional 2025 and six provincial Excel workbooks. These are filename/metadata observations, not verified row-level suitability.
