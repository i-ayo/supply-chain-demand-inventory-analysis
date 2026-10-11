# Supply Chain Demand & Inventory Risk Analysis

## Overview

A self-directed operations analytics project using synthetic consumer-electronics data to investigate demand variance, inventory coverage and potential fulfilment risk.

The objective was to identify where actual demand diverged from forecast, assess the potential operational impact, and propose practical next steps for investigation.

**Tools:** SQL Server, Excel and GitHub  
**Dataset:** 720 synthetic records across 12 weeks, 5 markets, 3 channels and 4 product categories.

## Business Question

Where is demand diverging from forecast, what does this mean for inventory coverage, and what should an operations team investigate before deciding how to respond?

## Key Findings

The initial analysis focuses on Germany's Online Store smartphone segment.

- Actual demand was approximately **24.7% above forecast** across Weeks 9–12.
- Inventory coverage in Week 12 was approximately **0.52 weeks**, based on ending inventory divided by actual demand for that week.
- The demand gap developed over several weeks rather than appearing as a single isolated spike in the scenario.
- The dataset identifies a potential fulfilment risk but does not establish the cause of the demand increase.

These results apply only to the synthetic scenario, not to Apple's actual supply chain.

## Method

1. Checked the dataset structure and row count.
2. Compared actual demand with forecast by week, market, channel and product.
3. Investigated the segment with the largest sustained demand variance.
4. Calculated inventory coverage using ending inventory divided by the latest week's actual demand.
5. Considered whether the pattern appeared isolated or more widespread.
6. Developed recommendations while separating data evidence from assumptions requiring stakeholder confirmation.

## Recommended Next Steps

- **Sales / Finance:** Validate whether a promotion, pricing change or other commercial activity could explain the demand uplift.
- **Planning:** Review the latest demand forecast and assess whether the increase is likely to persist.
- **Logistics:** Investigate feasible stock reallocation or earlier supply options, including timing and constraints.
- **Operations:** Continue monitoring demand variance and inventory coverage before committing to a supply decision.

## Files

- `data/operations_supply_chain_data.xlsx` — synthetic dataset.
- `sql/analysis.sql` — SQL queries for demand variance, weekly trends, inventory coverage and segment comparison.
- `report/operations-brief.pdf` — optional exported copy of the Operations Brief, if included.

## Limitations

This project uses synthetic data created for analytical practice. It does not represent Apple's actual operations or include verified supplier constraints, real promotions, allocation rules or confirmed transfer lead times.

The findings indicate where further investigation may be warranted; they are not sufficient on their own to authorise a real supply decision.

## What I Learned

This exercise helped me apply structured problem-solving and data analysis to an operations scenario, connect numerical findings to business risks, and consider what additional information stakeholders would need before acting.
