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
