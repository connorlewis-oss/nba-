A machine‑learning model that classifies NBA players into Elite, Starter, or Role tiers using performance and efficiency metrics.
NBA front offices need fast, data‑driven tools to evaluate player roles, optimize rotations, and avoid misallocating salary. This project provides a reproducible modeling pipeline that predicts player tiers using publicly available performance data. Stakeholders include analysts, coaches, and decision‑makers responsible for roster construction.

Row Definition: One row = one NBA player’s full 2017–2018 regular season. Time Span: October 2017 – April 2018 Filters:

Players with more than 500 minutes played

Consolidated stats for traded players

Removed incomplete or anomalous entries Sources: Publicly available NBA box score and advanced metrics datasets.

From CP4 to CP7, the workflow progressed through a full analytics pipeline:

CP4: Data cleaning, validation, and feature selection

CP5: Exploratory analysis and correlation structure

CP6: Multiple linear regression to estimate continuous “tier scores”

CP7: Gradient Boosted Classification to assign Elite/Starter/Role labels

This combination balances interpretability with predictive accuracy.

How to View or Reproduce
Cleaned dataset: /data/NBA_2017_2018_cleaned.csv

Sample slice (if needed): /data/sample_slice.csv

Figures: /figures only hiccup is figures is reports and vice cersa

Reports: /reports

Workbook or notebook: /project_notes

Limitations:

Only one season of data used

Role labels partially subjective

No cross‑season validation

Next Steps:

Expand to multiple seasons for robustness

Validate on current‑season data

Build an interactive dashboard for analysts and coaches
