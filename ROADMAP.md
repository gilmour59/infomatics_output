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
- [ ] Audit complete workbook formula dependencies and external-source status before editing/preparing data.
- [ ] Copy selected municipality-level operational fact files as source-preserving working copies and derive verified standalone analytical extracts.
- [ ] Assess K-Means vs hierarchical/DBSCAN as candidate Rice clustering methods, Isolation Forest as supporting method; examine regression/forecasting only if justified.
- [ ] Assess clean Mango dataset upon upload and choose independent, suitable mining task.
- [ ] Predefine baseline models, metrics and temporal/geographic validation before experimentation.

- [x] Inspect specified 2016–2026 normalized planting and harvest directories; confirm 22 annual workbooks, municipal columns and cross-year sample schema.
- [ ] Validate all year/month tabs (especially additional 2026 revision-looking tabs), explicit municipality-only extraction, reconciled irrigation/seed definitions, and 2026 partial-year status.
- [ ] Validate formulas and sample value consistency before creating immutable analytical exports of the appropriate working copies.

## Working copy milestone — 2026-10-11
- [x] Identify hidden 2026 planting extra tabs: Mar1, Mar2, March1, September1. Exclude from analyses; retain in unmodified workbook copies.
- [x] Create all 22 normalized yearly planting and harvest working copies in Drive folder: https://drive.google.com/drive/folders/1yXA352DCIfh39P6nXvECDyKENb_uoND6
- [ ] Complete formula-reference audit over all tabs (only representative samples audited so far).
- [ ] Generate validated municipality-only value extracts without modifying any copied source sheets; check totals, duplicate reports and incomplete 2026 months.
