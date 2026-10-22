# Fraud Auditor

## Work
### High-risk finding: revenue appears materially overstated

NovaCart's presentation reports 2025 revenue of $1,200,000, but the supplied
records do not support that amount. The invoice export contains $1,000,000 of
2025 invoice rows, yet three high-value invoices are repeated exactly:

| Repeated invoice | Customer | Amount per row | Rows | Duplicate overstatement |
| --- | --- | ---: | ---: | ---: |
| NC-2025-0074 | North Coast Workplace Meals | $100,000 | 2 | $100,000 |
| NC-2025-0327 | Summit Hospitality Group | $110,000 | 2 | $110,000 |
| NC-2025-0801 | Metro Campus Dining | $115,000 | 2 | $115,000 |
| **Total** |  |  |  | **$325,000** |

Removing the repeated rows leaves $675,000 of distinct 2025 invoicing
($1,000,000 - $325,000), not $1,200,000. This is a serious revenue-quality and
record-integrity concern.

### Cash does not support the revenue claim

Under the stated cash-basis policy, 2025 customer receipts were $550,000.
Another $40,000 receipt for 2025 invoice NC-2025-1103 arrived on March 3, 2026,
making total cash collected for 2025 invoices $590,000. The three open Bright
Foods invoices (NC-2025-B1, B2, and B3) total $85,000 and should not be 2025
cash-basis revenue.

The stated $1,200,000 equals the duplicate-inflated 2025 invoice-row total of
$1,000,000 plus two non-customer deposits totaling $200,000: $150,000 loan
proceeds from Lakeshore Bank and a $50,000 transfer from J. Novak. This exact
relationship is an inference from the supplied records, but it warrants an
immediate management explanation and a corrected revenue bridge.

### Profitability claim is inconsistent with bank activity

The presentation says NovaCart has been profitable since Q3 2025. Bank records
show 2025 customer receipts of $550,000 and operating outflows of $640,000,
or a $90,000 cash operating loss. Monthly operating cash flow was negative in
July ($39,002), August ($38,549), October ($43,523), November ($43,962), and
December ($38,810). September was positive by $76,164, driven by the $115,000
Metro Campus Dining receipt. The supplied cash-basis facts do not support
continuous profitability since Q3.

## Evidence
- `inputs/claims.md`: management reports 2025 revenue of $1,200,000, claims
  profitability since Q3 2025, and specifies cash-basis books.
- `inputs/invoices.csv`: NC-2025-0074 appears twice at $100,000;
  NC-2025-0327 appears twice at $110,000; and NC-2025-0801 appears twice at
  $115,000. The same export lists Bright Foods invoices NC-2025-B1 ($30,000),
  NC-2025-B2 ($28,000), and NC-2025-B3 ($27,000) as open.
- `inputs/bank.csv`: 2025 customer receipts total $550,000; operating outflows
  total $640,000. It records loan proceeds from Lakeshore Bank of $150,000 on
  2025-02-05, a $50,000 transfer from J. Novak on 2025-04-08, and the $40,000
  collection of NC-2025-1103 on 2026-03-03.
- Calculation checks: $1,000,000 - ($100,000 + $110,000 + $115,000) =
  $675,000 distinct invoicing; $30,000 + $28,000 + $27,000 = $85,000 open;
  $550,000 - $640,000 = -$90,000; and $1,000,000 + $150,000 + $50,000 =
  $1,200,000.

## Handoff
Do not rely on the $1,200,000 revenue claim or the profitability assertion for
an investment decision until management provides source contracts, corrected
invoices, and a bank-to-revenue reconciliation. Verify the three large customer
transactions directly, exclude loan and owner-transfer proceeds from revenue,
and explain the $85,000 in outstanding Bright Foods invoices.
