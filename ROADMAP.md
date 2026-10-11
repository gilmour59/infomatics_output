# Roadmap — Two MIT 525 Proposals

## Stage 0 — Assignment alignment (complete)
- [x] Compare the two supplied assignment PDFs (matching text and visual contents).
- [x] Extract all 14 required proposal sections and rubric (framework 15, business 25, data 25, methodology 25, ethics/feasibility 10).
- [x] Choose CRISP-DM as provisional primary framework.

## Stage 1 — Evidence-based dataset selection (in progress)
- [x] Inventory top-level Rice and HVC Drive folders.
- [x] Inspect selected native Sheets' tab layouts and sample values.
- [x] Inventory Rice immediate subfolders and nested-category names; initial annual source files located.
- [ ] Profile historical coverage, completeness, granularity and definitions of selected Rice datasets.
- [ ] Inspect HVC 2025 Excel workbook and fully decode 2024/2026 hierarchical column headings.
- [ ] Profile missingness, duplicates, invalid quantities, units, geographic/year coverage.
- [ ] Confirm source permission and permitted use in coursework.
- [ ] Record source-to-target data lineage and any transformation rules.
- [ ] Decide one feasible primary mining task per research track.

## Stage 2 — Business and data understanding (separate outputs)
- [ ] Define one actionable problem, decisions and stakeholders per track.
- [ ] Draft 2–4 measurable business objectives and corresponding mining objectives.
- [ ] Define unit of analysis, grain and target variable (if supervised).
- [ ] Build validated data dictionary and five exploratory visualizations/plans.
- [ ] Document constraints, limitations, bias, access and leakage risks.

## Stage 3 — Methodology planning (separate outputs)
- [ ] Compare baseline with 2–3 candidate models suited to the available data.
- [ ] Define data preparation, temporal/geographic validation, metrics and acceptance thresholds before modeling.
- [ ] Prepare CRISP-DM phase-to-activity/output/member mapping.
- [ ] Document evaluation-to-action flow and ethical controls.

## Stage 4 — Proposal production and QA (separate outputs)
- [ ] Draft complete 14-section proposal for Rice.
- [ ] Draft complete 14-section proposal for HVC.
- [ ] Add IEEE references, feasible timeline and appendices.
- [ ] Check all required guide tables and 16-point instructor checklist.
- [ ] Score each draft against five criteria and revise deficiencies.

## Deliverables
- **Output A:** Rice midterm research proposal (10–15 pages recommended, appendices excluded).
- **Output B:** High Value Crops midterm research proposal (10–15 pages recommended, appendices excluded).
- Two reproducible dataset-profiling reports and method-selection rationales.

Dates and responsible members should be filled in when the submission date and team assignments are confirmed.

## Explicit analyst recommendations and decision gates
### Rice (complete before title/method lock)
- [ ] Profile PSA annual production/yield/harvested area as the first-choice primary dataset; distinguish whole-year from partial 2026 observations.
- [ ] Compare PSA geography/year granularity with normalized monthly and per-season planting/harvest data; reconcile metric definitions and prevent duplicate aggregates.
- [ ] Examine disaster damage and seed utilization as **optional** covariates; include only if geographic/temporal joins, coverage and causal interpretation are defensible.
- [ ] Choose a focused Rice question only after verifying target/observation counts. Compare pattern discovery versus regression/forecasting feasibility; avoid promising forecasts with insufficient time-series depth.

### High Value Crops (feasibility gate before title/method lock)
- [ ] Inspect FY 2025 Excel source and map the hierarchical headers of all three annual workbooks.
- [ ] Define/test canonical HVC grain: year × month × province/municipality × commodity × variety × production system (only keep dimensions present in each year).
- [ ] Check comparability of bearing/non-bearing trees, farmer counts, planted/harvested area, production volume and units; separate blank, dash, zero and not-reported.
- [ ] Decide whether broad HVC clustering/pattern analysis or a narrower cacao study has enough comparable observations and coverage; regression only if a valid label and non-leaky predictors exist.

### Both tracks
- [ ] Document source-level limitations, publication/access permissions, data dictionary and at least five meaningful exploratory views per proposal.
- [ ] Fix evaluation measures and train/test strategy before fitting models; guard against time/geography leakage, and do not report proposal-stage hypothetical results as findings.
- [ ] Keep two distinct proposals, their narratives, tables, IEEE sources and independent rubric checks; keep Drive read-only and raw/sensitive data out of public GitHub.

## Updated dataset decisions — 2026-10-11
- [x] Create separate Rice working-copy folder and copy three initial LGU–DA / PSA candidate Sheets without editing original data.
- [ ] Check copied summary/index workbooks for linked external sources and obtain independent working copies of any necessary underlying LGU records.
- [ ] Assess clean Mango dataset when supplied; prefer evidence-based technique selection rather than a predetermined algorithm or class-reporting topic.

## Updated source and technique milestones (2026-10-11)
- [x] Inspect deeper normalized annual folders, containing 2016–2026 files; inspect sample municipality-level planting and harvest worksheets for 2025.
- [x] Detect external IMPORTRANGE formulas in copied monthly summary; detect internal tab references in PSA annual copy.
- [x] Audit visible-tab formula dependencies and external-source status before extraction; 2026 source dependencies remain flagged.
- [x] Copy municipality-level operational workbooks and derive value-only analytical extracts in Drive.
- [ ] Assess K-Means vs hierarchical/DBSCAN as candidate Rice clustering methods, Isolation Forest as supporting method; examine regression/forecasting only if justified.
- [ ] Assess clean Mango dataset upon upload and choose independent, suitable mining task.
- [ ] Predefine baseline models, metrics and temporal/geographic validation before experimentation.

- [x] Inspect specified 2016–2026 normalized planting and harvest directories; confirm 22 annual workbooks, municipal columns and cross-year sample schema.
- [x] Validate visible monthly tabs, municipality-only total-field extraction, and 2026 partial-year status; irrigation/seed subgroup reconciliation remains future work.
- [x] Validate visible-tab formulas, errors, keys, and total-yield arithmetic before value-only analytical export.

## Working copy milestone — 2026-10-11
- [x] Identify hidden 2026 planting extra tabs: Mar1, Mar2, March1, September1. Exclude from analyses; retain in unmodified workbook copies.
- [x] Create all 22 normalized yearly planting and harvest working copies in Drive folder: https://drive.google.com/drive/folders/1yXA352DCIfh39P6nXvECDyKENb_uoND6
- [x] Audit formulas and calculated errors across every visible tab of all 22 annual copies; 2026 external imports documented separately.
- [x] Generate municipality-only value extracts and 2016–2025 panel; check keys, missingness, yield arithmetic and 2026 incompleteness.

## Rice analytical dataset milestone — 2026-10-11
- [x] Audit 22 copied annual workbooks across all visible tabs: 190,302 formula cells, zero calculated error cells; 168 external-import formulas confined to 2026 (132 planting, 36 harvest). Hidden tabs excluded.
- [x] Create the 2016–2025 municipality × month × year value-only panel: 12,120 rows, 101 geocoded municipalities, 10 years. Maintain a separate 2026 panel (1,212 calendar slots; October sparse, November–December empty).
- [x] Preserve reproducibility with 22 compact source extracts, source cell lineage, rebuild script, audit JSON and quality checks in [private Drive derived folder](https://drive.google.com/drive/folders/1_oB4m_owiN9mxPlZMNsTacd-dVbu7mI_).
- [ ] Review six planted-area/physical-area exceedances and the consistent Sapian/Sapi-An spelling difference with a domain owner. Do not alter reported values without an approved rule.
- [ ] Choose and validate the mining task using the completed panel: season-aware municipality clustering is a candidate; anomaly screening and forecasting need missingness and temporal validation controls. Keep PSA as a separate statistical reference.
