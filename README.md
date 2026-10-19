# Jumia Sales Dashboard

## Overview

This project analyzes Jumia product listings using prices, discounts, customer review counts, and ratings. The dashboard summarizes product performance and shows how discounts and ratings relate to review activity.

## Workbook contents

- **Dashboard** — six summary charts.
- **jumia_sales** — product-level source data.
- **Analysis and PT tabs** — supporting summaries, rankings, pivot-style tables, and chart inputs.

The source sheet contains 109 product records in rows 2–110 and a final `TOTAL` summary row. Exclude the `TOTAL` row from product-level comparisons.

## Data fields

| Field | Description |
| --- | --- |
| Product | Product name |
| Current Price | Current selling price in Kenyan shillings (KSh) |
| Old Price | Original price in KSh before the discount |
| Discount amount (KSh) | Old Price minus Current Price |
| Discount | Discount percentage; confirm Excel’s number format when working with the underlying value |
| Discount category | Low, Medium, or High discount group |
| Review | Number of customer reviews |
| Rating | Average customer rating out of 5 |
| Rating Category | Poor, Average, or Excellent rating group |

## Category definitions

### Rating

- **Poor:** below 3
- **Average:** 3 to below 4.5
- **Excellent:** 4.5 or higher

### Discount

- **Low Discount:** below 20%
- **Medium Discount:** 20% through 40%, inclusive
- **High Discount:** above 40%

## How to use the dashboard

1. Open the **Dashboard** sheet for the summary charts.
2. Use the analysis tabs to review rating and discount breakdowns, review relationships, and product rankings.
3. Check the source data on **jumia_sales** when you need to confirm an individual product’s values.

## Refreshing summaries

In Excel, select **Data > Refresh All** to refresh connected PivotTables and charts. If you add product rows, first confirm that the data source range or table includes them, then refresh and check the dashboard totals.

## Notes for interpretation

- The review-versus-discount and review-versus-rating charts show associations in this dataset. They do not establish that discounts or ratings caused more reviews.
- Some records have a rating of `0` and are grouped as **Poor**. Confirm whether zero means an actual rating or a missing/unrated product before interpreting rating results.
- The workbook does not show a data collection or reporting date.
