# Investment Manager

## Work

### Forecast plan and basis

- Compare the investor pitch with invoice billings, invoice settlement status, and cash transactions.
- Treat bank customer receipts, refunds, and operating payments as the cash-basis operating record described in `inputs/claims.md`. Exclude loan and personal-transfer proceeds from revenue.
- Forecast April 2026–March 2027 from the March 31, 2026 closing bank balance of $170,000.
- Use a normalized recent-activity reference case, plus three transparent sensitivities. No future funding, new growth, inflation, capital spending, or cost changes are assumed unless specified by a case.

### Does the brief add up?

| Pitch statement | Input-record result | Assessment |
| --- | --- | --- |
| Revenue grew from $300,000 to $1,200,000, or 300% | The stated amounts do imply 300% growth: ($1,200,000 ÷ $300,000) − 1. Invoice billings are $306,000 in 2024 and $1,000,000 in 2025 (+226.8%). Customer bank receipts are $306,000 and $550,000 (+79.7%), excluding financing. | The pitch arithmetic is correct for its stated numbers; neither 2025 amount is supported by the supplied registers. The invoice and bank figures also need reconciliation. |
| $1,200,000 revenue in 2025 | The invoice register totals $1,000,000. Bank customer receipts total $550,000 in 2025; the bank also records $150,000 of loan proceeds and a $50,000 personal transfer, which are financing, not sales. | Pitch is $200,000 above billings and $650,000 above recorded customer deposits. |
| Profitable since Q3 2025 | Using the exercise's cash-basis rules, Q3 operating cash was ($1,387) and Q4 was ($126,295). Full-year 2025 operating cash was ($90,000). | Not supported by the cash record; Q3 was near breakeven but negative, followed by a large Q4 cash loss. |
| 4,000 active customers | There are 1,106 invoice rows for 2025, but invoice rows are not a customer count; the brief says business invoices may consolidate scheduled deliveries. | The customer claim cannot be verified from these inputs or without a definition of “active.” |

### Historical cash bridge

All values USD. Customer receipts are positive bank entries described as `Customer receipt`. Refunds are shown separately from operating outflows. Financing is excluded from operating results.

| Period | Customer receipts | Refunds | Operating outflows | Net operating cash | Non-operating funding | Opening cash | Ending cash |
| --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| 2024 actual | $306,000 | ($6,000) | ($330,000) | **($30,000)** | $0 | $80,000 | $50,000 |
| 2025 actual | $550,000 | ($30,000) | ($610,000) | **($90,000)** | $200,000 | $50,000 | $160,000 |
| Q1 2026 actual | $40,000 | $0 | ($30,000) | **$10,000** | $0 | $160,000 | $170,000 |

Calculation: customer receipts − refunds − operating outflows = net operating cash. The 2025 $200,000 funding consists of the $150,000 “Loan proceeds - Lakeshore Bank” and the $50,000 “Transfer from J. Novak personal.” Thus cash rose $110,000 in 2025 even as operations used $90,000. The $40,000 received in March 2026 is payment for invoice NC-2025-1103, dated December 31, 2025, and is not recurring 2026 sales evidence.

Invoice status reconciliation remains open: 2025 invoices total $1,000,000, of which $915,000 is marked paid and $85,000 is open. Bank customer receipts posted in 2025 total $550,000, with another $40,000 posted in March 2026. The paid-status amount exceeds recorded receipts through March 2026 by $325,000. This could include timing, matching, or recording issues; it is not a final conclusion until invoice IDs are matched to deposits.

Q3 detail: $171,113 customer receipts − $7,500 refunds − $165,000 operating outflows = ($1,387). Q4 detail: $56,205 − $7,500 − $175,000 = ($126,295). The Q1 2026 $10,000 monthly warehouse/administration spend is the only operating cost category recorded in those three months; customer receipts are $0 in January and February and $40,000 in March against the old 2025 invoice. Sparse activity may reflect a business change or incomplete operating records, so it should not be read as a verified cost structure.

## April 2026–March 2027 forecast

Opening cash is the $170,000 bank balance at March 31, 2026. The primary reference case carries forward the April 2025–March 2026 operating pattern but removes the specifically identified $40,000 collection of a 2025 invoice from recurring receipts. It assumes no additional financing.

| Case | Customer receipts | Refunds | Operating outflows | Net operating cash | March 2027 ending cash |
| --- | ---: | ---: | ---: | ---: | ---: |
| **Primary reference: latest 12 months, excluding old-invoice collection** | $393,583 | ($22,500) | ($520,000) | **($148,917)** | **$21,083** |
| Sensitivity: repeat latest 12 months including the $40,000 old-invoice collection | $433,583 | ($22,500) | ($520,000) | **($108,917)** | **$61,083** |
| Sensitivity: repeat 2025 calendar-year operating pace | $550,000 | ($30,000) | ($610,000) | **($90,000)** | **$80,000** |
| Sensitivity: repeat Q1 2026 bank pattern, excluding the old collection | $0 recurring | $0 | ($120,000) | **($120,000)** | **$50,000** |

Primary reference calculations: recent customer receipts $433,583 less the nonrecurring $40,000 collection = $393,583; refunds $22,500; operating outflows $520,000. Net operating cash is $393,583 − $22,500 − $520,000 = ($148,917). Ending cash is $170,000 − $148,917 = $21,083. The as-posted sensitivity retains the $40,000 collection, so ending cash is $61,083. The 2025 annual-pace case repeats 2025 totals with no growth. The Q1 pattern repeats $10,000 monthly warehouse/administration payments and assumes no recurring customer receipts; it is an activity sensitivity, not an all-in operating-cost forecast.

The primary case's month-by-month cash path is shown in the forecast visualization. The recorded LTM contains large customer-receipt months in April and September 2025 and much lower deposits otherwise. Repeating one year's monthly pattern is only a reference, not evidence of seasonality. The $21,083 ending balance is particularly sensitive to whether those receipts recur and whether missing Q1 operating costs return.

## Recommendation

**Pass on the $500,000 request as presented.** The records show operating cash losses, an unresolved $325,000 paid-status-to-bank-receipt gap, and no quantified use-of-funds plan or supported growth case. Reconsider a staged investment only after:

1. Invoice IDs and cash deposits reconcile, with the $150,000 loan and $50,000 personal transfer documented separately.
2. Current customer activity and the full operating cost base are verified, especially the sparse Q1 2026 bank pattern.
3. Management supplies a monthly use-of-funds plan with measurable milestones and enough detail to test the cash runway and path to positive operating cash.

These are information and execution gates, not an accusation of misconduct. The $500,000 is not added to forecast cash because its timing, uses, and resulting operating impact are not provided.

## Handoff

- Accountant: match the invoice register to bank deposits and resolve the $325,000 paid-status difference through March 2026.
- Financial Analyst: verify cash-basis revenue, costs, growth, and the profitability claim using the transaction-level records.
- Fraud Auditor: examine the loan, personal transfer, and large receipt/invoice exceptions against the source records.
- Customer Analyst: assess whether the invoices support a recurring customer base and what the 4,000-active-customer claim means.
- Team: revisit this recommendation after those checks; use the forecast cases as transparent reference scenarios, not management guidance.

## Evidence sources

- `inputs/claims.md` — pitch figures, $500,000 ask, customer claim, profitability claim, and cash-basis reporting context.
- `inputs/invoices.csv` — invoice amounts, customer names, dates, and paid/open status.
- `inputs/bank.csv` — opening and closing balances, customer receipts, refunds, operating payments, and financing through March 31, 2026.
