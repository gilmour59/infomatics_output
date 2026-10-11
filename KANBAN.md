# Kanban / TODO

Status as of 2026-10-11. Mark tasks individually when evidence is verified.

| ID | Track | Task | Status | Priority | Evidence / exit criteria |
|---|---|---|---|---|---|
| G01 | Shared | Align assignment outline/rubric | Done | High | Fourteen sections and 100-point rubric captured |
| G02 | Shared | Maintain CRISP-DM mapping templates | To do | High | Each phase has activity, output, owner |
| R01 | Rice | Inventory top-level Drive folder | Done | High | Top-level datasets identified |
| R02 | Rice | Inspect normalized monthly/seasonal and PSA source structure | In progress | High | Tab headings and grain verified |
| R03 | Rice | Review supplementary subfolders and disaster/seed/budget datasets | In progress | Medium | Access/variable/coverage matrix |
| R04 | Rice | Check 2026 partial-year status and source consistency | Done | High | Comparable time windows validated |
| R05 | Rice | Recommend objective and mining task | To do | High | Supported by quality-profile evidence |
| H01 | HVC | Inventory 2024–2026 workbooks | Done | High | Three files located |
| H02 | HVC | Compare hierarchical 2024–2026 schemas | In progress | High | Verified canonical field mapping |
| H03 | HVC | Inspect 2025 Excel and month/province/commodity coverage | To do | High | Cross-year comparability documented |
| H04 | HVC | Decide broad crop vs cacao-focused proposal | To do | High | Sufficient observations and viable task |
| H05 | HVC | Recommend objective and mining task | To do | High | Supported by quality-profile evidence |
| P01 | Shared | Draft two independent 14-section proposals | To do | High | All instructor requirements completed |
| P02 | Shared | Rubric QA and IEEE references | To do | High | Criteria and checklist checked |

## Workflow
To do → In progress → Review → Done. Put blockers in the task evidence column or open a GitHub Issue. No dataset modifications in Drive; no raw dataset commits in this public repository.

## Recommendation-specific cards (research gates)

| ID | Track | Task | Status | Priority | Evidence / exit criteria |
|---|---|---|---|---|---|
| R06 | Rice | Profile PSA annual data as primary candidate | To do | High | Year/province coverage, variable types, missingness, outlier and aggregate checks |
| R07 | Rice | Verify annual versus partial 2026 values | To do | High | Comparable reporting window documented |
| R08 | Rice | Reconcile PSA, monthly and seasonal grain/definitions | To do | High | Join feasibility, duplicate prevention and unit mapping |
| R09 | Rice | Evaluate optional disaster and seed datasets | To do | Medium | Include/exclude decision with temporal/geographic join evidence |
| R10 | Rice | Select focus and suitable mining task | To do | High | Observation counts, target feasibility, baseline and validation rationale |
| H06 | HVC | Decode 2024–2026 headers and inspect 2025 Excel | To do | High | Year-by-year canonical schema mapping |
| H07 | HVC | Normalize commodity/province/month/variety/system grain | To do | High | Cross-year sample and reconciliation checks |
| H08 | HVC | Test crop and metric consistency across years | To do | High | Coverage, units, blanks/dashes/zeros, duplicates documented |
| H09 | HVC | Compare broad HVC vs cacao-focused studies | To do | High | Evidence-backed feasibility and task decision |
| G03 | Shared | Confirm permission, confidentiality and public repo policy | To do | High | Only safe metadata/code/proposal text committed |
| G04 | Shared | Define baseline, validation, metrics and leakage safeguards | To do | High | Pre-specified independently for both tracks |
| P03 | Shared | Perform two separate rubric and checklist reviews | To do | High | Each proposal scores against all five rubric categories and 16 checklist items |

| R11 | Rice | Create safe working copies of selected initial source workbooks | Done | High | Three copies in dedicated Drive folder, originals untouched |
| R12 | Rice | Inspect links/formulas and copy underlying operational fact tables if required | Done | High | Self-contained, verified observation-level working data |
| H10 | HVC | Receive and profile clean Mango dataset | Blocked | High | Await user-supplied dataset and verify unit of analysis and task |

## Explicit technique and dependency cards (2026-10-11)

| ID | Track | Task | Status | Priority | Exit criteria |
|---|---|---|---|---|---|
| R13 | Rice | Profile municipality-level normalized planting and harvest 2016-2026 | Done | High | Confirm municipality-month-year grain, irrigation/seed fields and usable observations |
| R14 | Rice | Fully audit copied workbook formula and external references | Done | High | Monthly summary IMPORTRANGE confirmed; trace links/errors and validate frozen values |
| R15 | Rice | Copy selected municipality-level raw reporting sheets to working Drive folder | To do | High | Working copies only; extract independent validated analytical values |
| R16 | Rice | Evaluate K-Means vs hierarchical/DBSCAN clustering | To do | High | Feature set, baseline, silhouette, stability and expert interpretation |
| R17 | Rice | Evaluate Isolation Forest anomaly detection | To do | Medium | Seasonality adjusted, expert-validated abnormal patterns |
| R18 | Rice | Assess regression and time-series feasibility | To do | Medium | Time-aware predictors, suitable horizon and held-out validation |
| H11 | Mango | Profile clean Mango data and choose mining methods | Blocked | High | Await dataset; evaluate clustering versus regression based on evidence |
| G05 | Shared | Specify final model selection and leakage/evaluation controls | To do | High | Clear pre-specified metrics and validation |

| R19 | Rice | Verify all normalized 2016–2026 annual source workbooks | Done | High | 22 files inventoried, 2016/2024/2025/2026 examples checked; full schema/coverage audit remains |
| R20 | Rice | Exclude regional/provincial totals and resolve extra 2026 tabs | Done | High | Consistent municipality-year-month rows, no duplicates |
| R21 | Rice | Cross-check area planted, harvested, production and yield computations | Done | High | Per-source definitions, plausibility and arithmetic verified |

## 2026-10-11 Working-copy and hidden-tab update
- R15: **Done** — copied all 22 municipality-level yearly normalized Rice workbooks (11 planting + 11 harvesting, 2016–2026) into the separate Google Drive working folder. Originals unchanged.
- R14: **Done for visible tabs** — scanned all 22 annual copies. 2026 has 168 external import formulas; 2016–2025 has none detected. Source snapshots for 2026 remain dependency-bearing.
- R20: **Done** — excluded all hidden tabs and annual/aggregate rows from the municipality-month panel; 2026 extras remain untouched.
- R22: **Done for visible tabs** — audited 190,302 formulas and all calculated cells; zero errors, 168 external imports in 2026 only. Hidden tabs intentionally excluded.
- R23: **Done for extracts and aggregate handling** — 2016–2025 panel and separate 2026 snapshot delivered in Drive with lineage and reproducibility package. Original-to-copy equivalence was not checked byte for byte.

## Derived Rice dataset status — 2026-10-11

| ID | Track | Task | Status | Priority | Evidence / exit criteria |
|---|---|---|---|---|---|
| R22 | Rice | Visible-tab formula and calculated-error audit of 22 copies | Done | High | 190,302 formulas; 0 calculated errors; 168 external imports only in 2026; hidden tabs excluded |
| R23 | Rice | Municipality-only value extracts and joined panel | Done | High | 12,120 historical rows; 101 municipalities; no duplicate keys; separate 2026 snapshot; [Drive deliverables](https://drive.google.com/drive/folders/1_oB4m_owiN9mxPlZMNsTacd-dVbu7mI_) |
| R24 | Rice | Review six planted-area exceedances and Sapian spelling | Review | Medium | Domain owner validates without silently changing source values |
| R25 | Rice | Select and evaluate a defensible mining method | To do | High | Seasonal coverage treatment, simple baseline, stability and temporal validation |

No operational CSVs or row-level extracts are stored in this public repository.
