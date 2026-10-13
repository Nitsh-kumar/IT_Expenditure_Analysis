# IT Expenditure Analysis — Power BI

A Power BI report for exploring actual, forecast, and planned IT expenditure across geography, business area, and cost categories.

**Status:** report case study. The report artifact is present; refresh, model definitions, and calculations still need reproducibility evidence.

## Files

- [IT_spend_analysis.pbix](IT_spend_analysis.pbix): Power BI report.
- [IT Expenditure dataset.xlsx - Data.csv](IT%20Expenditure%20dataset.xlsx%20-%20Data.csv): included tabular data.

The supplied review identified three report pages: IT spend, cost variance, and business-area drilldown.

## Inspecting the report

Open the PBIX in a compatible Power BI Desktop version.

1. Save a working copy.
2. Inspect Power Query sources and change local source paths if required.
3. Inspect relationships, date fields, and measures.
4. Refresh using the intended dataset snapshot.
5. Reconcile actual, forecast, and plan totals before using slicers or publishing findings.

The included CSV alone does not prove that every PBIX data source can refresh without adjustment.

## Screenshots

### IT spend

![IT spend report screenshot](https://github.com/user-attachments/assets/71e7f255-36f5-4566-a50e-ad2ca6ef20b0)

### Cost variance

![Cost variance report screenshot](https://github.com/user-attachments/assets/4b2fbff6-7dfe-4010-a9f2-b069da21ad4b)

### Business-area drilldown

![Business-area report screenshot](https://github.com/user-attachments/assets/0c93e0be-53c7-4a04-95ef-7211ce6c651e)

These are existing screenshots, not evidence of a fresh refresh.

## Calculation documentation

For each measure, record its actual model definition, units, filter context, and handling of missing or zero plan values. Variance direction must be explicit: actual minus plan and plan minus actual have different meanings.

The previous README's DAX snippets were not an exported model definition. Verify measures inside the PBIX rather than treating example formulas as authoritative.

## Data handling and next work

Establish the source period, provenance, and reuse rights before publication. Export inspectable model/report definitions where supported and document refresh steps without replacing the PBIX.

See [project status](docs/PROJECT_STATUS.md).

## Validation

This documentation was checked against repository files on 13 October 2026. Notebooks, application runs, refreshes, and test suites were not executed during this documentation pass. Saved outputs are historical evidence, not a fresh run.
