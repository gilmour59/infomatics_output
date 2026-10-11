# Dataset Inventory and Preliminary Feasibility — 2026-10-11

**Status:** Historical preliminary inventory retained below; a complete visible-tab audit and municipality-month extract is documented in the final section. Source folders and copied source spreadsheets remain unchanged.

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

## Rice working copies created — 2026-10-11
Working folder: https://drive.google.com/drive/folders/1yXA352DCIfh39P6nXvECDyKENb_uoND6

| Source ID | Working copy | Working ID | Role |
|---|---|---|---|
| 1KXZ8SnlwLq_vAVh2cOnxeuONZHYKFDWWPqzh5nQL838 | LGU DA Monthly Planting Harvest Yield | 12vUzNBnU0CzGsp_DjThjog-g57T_1oTWfBxJRiwZaUc | Candidate operational primary |
| 1R0t4rbQexbLnhHyX6sODcNKZMeRAoeH7hCBSew43RYM | LGU DA Per Season Planting Harvest Production | 1n_L0ePHdi3h-ZRmzH1rIkaelG_d5aFcip2zs1PJcO8E | Candidate seasonal supplement |
| 1V2Xt-4Zxho_gVKx9GqzJj_h7a6hWjYVNJeYAL1N4-_I | PSA Annual Production Harvested Western Visayas | 11_gqRmervJAk5CT9bTbPrLuRJRWgAwVPMPDc2GHqGhI | Independent reference |

**Caution:** The monthly and season-level workbooks contain indexes or summaries and external/source links; investigate whether actual LGU observation-level records must be copied separately. Google Sheets copies may retain formulas linking to sources. Original datasets were not edited.

## Nested normalized files / sample formula audit — 2026-10-11
- Planting and harvesting NORMALIZED subdirectories contain annual workbooks for 2016–2026.
- Sample **Annual Planting 2025** has month tabs; January contains 114 rows and 37 columns, region/province/municipality and irrigated/rainfed area-planted fields by seed category.
- Sample **Harvest and Production 2025** has month tabs; January contains 113 rows and 91 columns, region/province/municipality, harvested area, yield and production by seed category.
- Both contain aggregate rows alongside municipality rows; filter explicitly to the chosen observation grain.
- Copied monthly summary contains IMPORTRANGE dependencies (sample: NORMALIZED A1:BA7): NOT fully self-contained.
- Copied seasonal summary sample A1:K8 has CONCATENATE formulas; full audit pending.
- Copied PSA annual sample A1:M12 uses internal Panay Island (Quarterly) worksheet references; full audit pending.
- Keep sources read-only, preserve formulas in source copies, and derive value-only analysis tables after provenance and reconciliation checks.

## Direct normalized folders confirmed (2026-10-11)
- Planting: https://drive.google.com/drive/folders/1CvizHCIClkHkMf4pVYSDCGv8ElNg8Uy2 — 11 yearly Google Sheets, 2016–2026. Sampled 2016/2024/2026 month tabs ~114×37, region/province/municipality, irrigation, seed class, area planted (ha).
- Harvest: https://drive.google.com/drive/folders/1xbwS5Jc-itN_65YRB1U41mxk0pkuJq_X — 11 yearly Google Sheets, 2016–2026. Sampled 2016/2024/2026 month tabs ~113×91, region/province/municipality, irrigation/seed category, harvested area, yield MT/ha, production MT.
- Both mix regional/provincial totals with municipality rows. 2026 planting contains extra tabs named Mar1, Mar2, March1; exclude until validated.
- Sample structures are broadly compatible but do not prove full year-level schema or source-quality consistency; 2026 annual data is incomplete until established otherwise.
- Recommended analysis grain: municipality × month × year, with explicit irrigation/seed definitions; possible mining tasks clustering, anomaly detection, and supervised tasks only after confirming valid target/independent predictors.

## Working folder verification and formula-audit scope (2026-10-11)
Folder: https://drive.google.com/drive/folders/1yXA352DCIfh39P6nXvECDyKENb_uoND6
Contains **25 files**: 11 copied normalized planting annual books + 11 copied normalized harvest/production annual books (2016–2026), plus 3 earlier summary/reference copies.
2026 planting extra tabs Mar1, Mar2, March1, September1 explicitly have hidden=true; exclude them from analytical processing, do not delete them from workbook copies.
Representative January sampled formula checks for 2016, 2025 and 2026 show within-sheet sum and ratio calculations (not a full formula audit). Original summary copy separately contains IMPORTRANGE external dependencies. The 22 normalized copies are **working source copies, not certified standalone feature tables**. Full monthly/annual formula and error audit, cross-year checks, and value-only extracts are pending.

## Completed normalized Rice audit and analytical panel — 2026-10-11

**Derived Drive folder:** https://drive.google.com/drive/folders/1_oB4m_owiN9mxPlZMNsTacd-dVbu7mI_

The 22 copied annual planting and harvest/production Google Sheets (2016–2026) were audited cell by cell across every **visible** tab. There are 190,302 formula cells and no calculated spreadsheet error cells in that scope. No external-reference formula was detected in the 2016–2025 visible tabs. The two 2026 copies have 168 external-import formulas (132 planting, 36 harvest), all pointing to another operational spreadsheet; 2026 is therefore a separate, dependency-bearing snapshot. Hidden annual tabs in some years and the four extra hidden 2026 planting tabs were excluded from extraction and from the formula-audit scope. Formula counts and examples for each workbook are in the private Drive reproducibility package.

The value-only 2016–2025 panel has **12,120 unique municipality × month × year rows**: 101 geocoded municipalities, five provinces, 12 months, and 10 years. Source row and workbook identifiers accompany every record. A separate 2026 CSV has 1,212 calendar slots. Its October totals are sparse and November–December totals empty as of the extraction; do not compare it as a complete annual observation. Regional/provincial aggregate rows and annual summary tabs were excluded. The stable monthly source columns used are planting total all ecosystems (AF), rice physical area (AG), harvest total palay area (CJ), total production (CL), and reported yield (CK). Seed and ecosystem subtotals were not added to these totals.

Historical missingness: 2,595 / 12,120 planted-area cells and 2,658 / 12,120 harvested-area, production, and reported-yield cells are blank. Blanks were preserved, not filled with zero. Both source families have the same municipality-month keys, no duplicate keys, and no negative values in the selected measures. For present positive harvested area, production / area matches reported yield within 0.02 MT/ha. Six historical municipality-months have planted area exceeding the source's rice physical-area field; retained and flagged for domain review. The spelling Sapian (planting) versus Sapi-An (harvest) differs for one shared geocode in each month, but the geocode and province agree.

**Technique feasibility:** Descriptive seasonal/geographic profiling is immediately feasible. Clustering municipalities is feasible after coverage-aware seasonal or annual feature construction, scaling, and stability review; K-means and hierarchical methods are reasonable first comparisons. Anomaly detection is a screening method requiring seasonal adjustment and source follow-up. Forecasting/regression remains conditional because the panel has substantial blanks and crop timing differs between planting and harvest; use chronological holdouts and simple seasonal baselines. No claim of causal effects or PSA-LGU equivalence follows from this panel. PSA is a separate independent reference, not merged into the operational rows.

The package in Drive contains the two CSV panels, 22 value-only source extracts, a standard-library Python rebuild script, `formula_audit.json`, `data_quality.json`, and an explanatory README. None of the row-level operational data was added to this public GitHub repository. Byte-for-byte equivalence of each working copy to its original source was not independently verified, and source-level 2026 external dependencies remain open.
