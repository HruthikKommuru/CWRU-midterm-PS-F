# Five-minute presentation outline

## 1. Investment decision | 0:30
**Slide:** Pass on the $500,000 request as presented. Show 2025 net revenue of $520,000, operating loss of $90,000, and base-case March 2027 cash of $21,083.

**Talk track:** NovaCart has collected revenue, but costs outpaced revenue and the reference case leaves a thin cash buffer. The request has no monthly use-of-funds plan.

**Sources:** `inputs/claims.md`, `inputs/bank.csv`; `roles/04_investment_manager/forecast.md`.

## 2. Revenue reconstruction | 1:00
**Slide:** Bridge the $1,000,000 2025 invoice-row total to $550,000 of gross 2025 receipts, then $520,000 net revenue after refunds.

**Talk track:** Remove $325,000 of duplicate invoice copies, $85,000 of open invoices, and the $40,000 invoice collected in March 2026. The stated 300% growth math is correct for management’s figures. Reconstructed cash-basis revenue grew 73.3%.

**Sources:** `inputs/claims.md`, `inputs/invoices.csv`, `inputs/bank.csv`; `roles/02_financial_analyst/profit.md`.

## 3. Invoice-to-bank tie-out | 0:45
**Slide:** All 1,700 paid receipt IDs and amounts match bank deposits totaling $896,000 across 2024–March 2026.

**Talk track:** The apparent $325,000 paid-status gap is explained by three duplicate invoice copies. Three Bright Foods invoices totaling $85,000 remain open. A $40,000 Riverside payment arrived 62 days after invoicing. The Accountant found no unmatched receipts or amount differences.

**Sources:** `inputs/invoices.csv`, `inputs/bank.csv`; `roles/01_accountant/matching.md`.

## 4. Operating performance | 0:55
**Slide:** Revenue grew 73.3%, costs grew 84.8%, and the annual loss widened from $30,000 to $90,000.

**Talk track:** Q1 and Q2 2025 were profitable; Q3 lost $1,387 and Q4 lost $126,295. The supplied cash-basis records do not support profitability since Q3. The $1.2 million claim equals $1.0 million of raw invoice rows plus $200,000 of financing, a coincidence requiring explanation but not proof of intent.

**Sources:** `inputs/claims.md`, `inputs/bank.csv`, `inputs/invoices.csv`; `roles/02_financial_analyst/profit.md`, `roles/03_fraud_auditor/red_flags.md`.

## 5. Twelve-month cash cases | 0:55
**Slide:** Four ending-cash sensitivities range from $21,083 to $80,000, starting at $170,000.

**Talk track:** The reference case carries forward recent activity after removing the old-invoice collection. It assumes no new funding or growth. The Q1 pattern is a sparse-activity sensitivity, not a complete cost forecast. The $500,000 request is excluded because its timing and use are unspecified.

**Sources:** `inputs/bank.csv`; `roles/04_investment_manager/forecast.md`.

## 6. Customer evidence and reconsideration | 0:55
**Slide:** The 2025 export shows 1,100 invoiced names; five business accounts generated 66.7% of adjusted billings. Household accounts grew 83.4%, while household invoiced value fell 26.2%.

**Talk track:** The export ends in December 2025, so it cannot verify the 4,000 active-customer claim at the April 2026 pitch date. All 600 accounts from 2024 invoiced again in 2025, but that is annual invoicing retention, not proof of frequent orders or current engagement. Pass now. Reopen after a dated customer roster and definition, major-account continuity evidence, Bright Foods collection support, corrected records, and a monthly plan to reach break-even.

**Sources:** `inputs/claims.md`, `inputs/invoices.csv`, `inputs/bank.csv`; `roles/05_customer_analyst/customers.md`, `roles/01_accountant/matching.md`, `roles/02_financial_analyst/profit.md`, `roles/03_fraud_auditor/red_flags.md`, `roles/04_investment_manager/forecast.md`.
