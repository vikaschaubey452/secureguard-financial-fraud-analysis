# SecureGuard Financial Fraud Analysis

An interactive Power BI portfolio project that explores patterns in labeled credit card fraud. The report helps an analyst see how often fraud appears in the sample, how much money is associated with flagged transactions, and which time periods and transaction segments warrant closer review.

## Dataset and baseline

The report uses an embedded sample of credit card transactions from January 2019 through June 2020. Transaction amounts are in USD. The model retains fields used for analysis, including time, merchant category, state, gender, amount band, and fraud label. It excludes names, card numbers, street addresses, exact coordinates, and transaction IDs.

| Metric | Baseline |
| --- | ---: |
| Transactions | 20,000 |
| Transactions labeled as fraud | 112 |
| Fraud rate | 0.56% |

**Fraud rate** is the number of transactions labeled as fraud divided by the number of transactions in the current filter selection. **Flagged amount** is the sum of transaction amounts associated with those labels. The report uses historical labels for exploratory analysis. It does not generate live alerts or predict fraud.

## Dashboard pages

| Page | What you can investigate |
| --- | --- |
| **Fraud Overview** | Review the transaction count, labeled fraud cases, fraud rate, and flagged amounts. |
| **Fraud Patterns** | Explore how flagged transactions vary over time and across transaction segments. |
| **Geography & Spend** | Compare states and examine transaction amount distributions by category and gender. |

Use the **Month**, **Category**, **State**, and **Gender** slicers to narrow the analysis. Select a chart bar or data point to cross-filter compatible visuals on the same page. When comparing segments, review fraud rate alongside transaction volume to give each rate context.

## Tools and skills

- **Power BI Desktop** for interactive report authoring and visualization
- **Power Query and DAX** for data preparation, KPI calculations, and filter-aware reporting
- **Power BI Project format** for the report and semantic model files

## Open the report

1. Open [SecureGuard-PowerBI-Project.zip](./SecureGuard-PowerBI-Project.zip) on GitHub and download it.
2. Extract the archive into a single folder on Windows, keeping the report and semantic model folders together.
3. Open `SecureGuard.pbip` in Power BI Desktop. If your version requires it, enable Power BI Project and the enhanced report format under **File → Options and settings → Options → Preview features**, then restart Power BI Desktop.
4. If visuals are blank on first open, select **Home → Refresh** to load the embedded sample.
5. To keep a single local Power BI file, choose **File → Save As** and save as `.pbix`.
