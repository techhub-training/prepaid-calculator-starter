# Spec: prepaid amortization calculator

## Inputs
* Prepaid ID (text, e.g. PP-09)
* Total cost in dollars (more than 0)
* First month, as YYYY-MM
* Number of months, a whole number from 1 to 120

## Rules
1. Monthly amortization = total cost ÷ number of months, **rounded to the cent** (1182.857 → 1182.86).
2. The **last month takes the rounding difference**, so the months add up to exactly the total cost and the
   remaining balance ends at 0.00.
3. Months run one after another from the first month and roll over into the next year (2026-12 is followed by 2027-01).

## Output
* A table: Month, Amortization, Remaining balance (after that month).
* A **Download CSV** button. The file has exactly these columns, in this order:

```
Month,Amortization,RemainingBalance
```

Months as `YYYY-MM`; amounts with two decimals and no `$` or thousands separators.

## Test case (this is what the TechHub checker asks for)
PP-09, a snow removal contract: **8280.00** over **7** months, first month **2026-11**.
Check: the amortization column adds up to 8280.00, the months run 2026-11 to 2027-05, and the last remaining balance is 0.00.
