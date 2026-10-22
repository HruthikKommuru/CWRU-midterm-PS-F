# NovaCart customer analysis — draft for review

## Conclusion for the investment team
**Main message agreed with Ridhika:** NovaCart’s customer base is growing, but its billings depend heavily on a few business accounts, while household billings are weakening.

The records support a larger customer-account base in 2025, but do not substantiate management's 4,000 active-customer claim under our agreed annual definition. Growth is heavily dependent on five business accounts; household invoiced value declined despite more household accounts. Duplicate invoices, unpaid business invoices, and a receipt arriving in 2026 weaken the headline growth story. Customer evidence supports requiring clarification and verification before investing; the leader should combine this with the other roles' findings.

## Scope and method
Sources: `inputs/claims.md`, `inputs/invoices.csv`, and `inputs/bank.csv` only. Active customer account means a distinct customer name with at least one invoice dated in the calendar year. Names are stable according to claims.md. Count accounts, not individuals, orders, or deliveries. Business invoices may consolidate deliveries. Household means a name beginning `Household `; the remaining named accounts are classified as business accounts.

Group invoices by invoice-date year and stable customer name. Report raw export rows separately from unique invoices. Three invoice IDs each appear twice with identical fields; count each once for the adjusted analysis, pending the accountant's confirmation. Inputs are unchanged. All dollar values below are invoiced value, not cash-basis revenue. Status is as of March 31, 2026.

## Customer metrics
| Metric | 2024 | 2025 |
| --- | ---: | ---: |
| Active customer accounts | 600 | 1,100 |
| Household accounts | 597 | 1,095 |
| Business accounts | 3 | 5 |
| Raw invoice rows | 600 | 1,106 |
| Unique invoice IDs | 600 | 1,103 |
| Raw invoiced value | $306,000 | $1,000,000 |
| Invoiced value counting each ID once | $306,000 | $675,000 |
| Household invoiced value | $304,534 | $224,887 |
| Mean household invoice value | $510.11 | $205.38 |
| Business invoiced value, counting each ID once | $1,466 | $450,113 |

Source: all rows of inputs/invoices.csv, grouped as described above. Cross-checks: 597 + 3 = 600; 1,095 + 5 = 1,100; $224,887 + $450,113 = $675,000. Customer-account growth is (1,100 / 600 - 1) = 83.33%. Management's 4,000 claim exceeds the observed 2025 count by 2,900 accounts. This is an unsupported claim under our definition, not proof of fraud: management must explain its definition and provide a reconciliation. The export ends in December 2025, so it cannot establish the active count at the April 2026 pitch date.

## Returning customers and purchasing patterns
All 600 accounts invoiced in 2024 also appear in 2025: observed annual account retention is 100%. Another 500 accounts first appear in 2025 (498 household and two business accounts). This is annual invoicing retention, not evidence of frequent ordering or current engagement.

After duplicate removal, no household account has more than one invoice in either year. Only two accounts have multiple distinct 2025 invoices: Riverside Senior Living (two) and Bright Foods LLC (three). Bright Foods' invoices remain open, so repeated billing is not evidence of repeat payment. Invoice frequency cannot establish delivery frequency, particularly for consolidated business billing.

Household accounts increased 83.42%, while their total invoiced value fell 26.15%. Mean household invoice value fell approximately 59.74%. More household accounts therefore did not translate into higher household billings. We cannot infer why spending fell or measure customer acquisition cost or lifetime value from these inputs.

Returning accounts generated $372,807 of adjusted 2025 invoiced value; new accounts generated $302,193. These sum to $675,000. The two new business accounts, Metro Campus Dining and Bright Foods LLC, account for $200,000 of the new-account value; $85,000 of that remains unpaid.

## Customer concentration
| 2025 customer | Unique-invoice value | Share of $675,000 |
| --- | ---: | ---: |
| Metro Campus Dining | $115,000 | 17.04% |
| Summit Hospitality Group | $110,000 | 16.30% |
| North Coast Workplace Meals | $100,000 | 14.81% |
| Bright Foods LLC | $85,000 | 12.59% |
| Riverside Senior Living | $40,113 | 5.94% |
| All other accounts | $224,887 | 33.32% |

Source: inputs/invoices.csv, unique IDs aggregated by customer. Top three accounts represent 48.15% and all five business accounts represent 66.68% of adjusted 2025 invoiced value, despite being only five of 1,100 accounts. Losing or failing to collect from one major account could materially affect the business. These percentages describe billings, not collected revenue.

## Evidence requiring handoff
1. **Duplicate large invoices inflate totals by $325,000.** NC-2025-0074 (North Coast Workplace Meals, January 24, $100,000), NC-2025-0327 (Summit Hospitality Group, April 2, $110,000), and NC-2025-0801 (Metro Campus Dining, September 1, $115,000) each occur twice identically in invoices.csv. Bank.csv contains one matching receipt per ID: January 25, April 3, and September 2, respectively. The raw top-three share is misleadingly inflated to 65%; the adjusted share is 48.15%. Ask the accountant and fraud auditor to confirm treatment. Duplicate rows are not repeat purchases.
2. **Bright Foods LLC: $85,000 uncollected.** NC-2025-B1 ($30,000, March 19), B2 ($28,000, June 19), and B3 ($27,000, September 19) are all open as of March 31, 2026. No bank narrative references these IDs. This indicates collection risk; absence of a reference alone would not prove nonpayment, but the open statuses support the concern. Seek customer verification and collection evidence.
3. **Riverside payment crosses calendar years.** NC-2025-1103 is a $40,000 invoice dated December 31, 2025, marked paid in the March 2026 status snapshot. The matching bank receipt is March 3, 2026. Under the cash-basis policy in claims.md, that payment is 2026 cash revenue, not 2025 revenue. Hand off to the financial analyst and accountant.
4. **Growth requires reconciliation.** Unique-invoice value grew 120.59% from $306,000 to $675,000; this is not cash-revenue growth. The leader must use the financial analyst's reconciled cash figures to assess management's 300% revenue-growth claim. Do not use raw export sums as revenue.

## Recommended handoff and questions
- Leader: require reconciliation of 4,000 active customers with 1,100 observed 2025 accounts and the difference in reporting dates; assess dependence on major business contracts.
- Accountant / fraud auditor: verify duplicates and collection evidence for the named invoice IDs.
- Financial analyst: reconcile cash revenue and the $40,000 received in 2026; assess household decline alongside operating costs.
- Before funding, request evidence of major-account contract continuity, explanation of falling household billings, and resolution of Bright Foods balances. These requests are proposed conditions, not facts present in the inputs.

## Student verification
Ridhika checked NC-2025-0074 in inputs/invoices.csv and confirmed two identical $100,000 paid entries. She also checked inputs/bank.csv and confirmed one matching receipt. This supports treating the duplicate as one invoice pending the accountant’s reconciliation. Other calculations and the draft were prepared by Codex; this source check covers the named invoice only.

## Limits
The files do not show demographics, customer acquisition cost, individual deliveries, contracts, or reasons for reduced spending. An invoice is not an order; a customer account is not necessarily one person. Annual return does not establish frequent purchasing. Conclusions about fraud, profitability, cash runway, or the final investment decision require the other roles' work.
