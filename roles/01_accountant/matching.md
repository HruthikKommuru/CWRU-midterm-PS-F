# Accountant

## Work
### Plan
1. Match each `invoice_id` in `inputs/invoices.csv` to the invoice ID embedded in each `Customer receipt` description in `inputs/bank.csv`.
2. Check that each matched pair has the same amount, then compare invoice and deposit dates.
3. Identify invoice IDs that are duplicated, have no receipt, or are deposited unusually late.

### Reconciliation results

| Result | Invoice records | Bank customer-receipt deposits | Invoice amount | Deposit amount | Difference |
| --- | ---: | ---: | ---: | ---: | ---: |
| Exact ID-and-amount matches | 1,700 distinct paid invoice IDs | 1,700 | $896,000 | $896,000 | $0 |
| Normal deposit timing (one day after invoice) | 1,699 | 1,699 | $856,000 | $856,000 | $0 |
| Matched but late deposit | 1 | 1 | $40,000 | $40,000 | $0 |
| Open invoices without deposits | 3 | 0 | $85,000 | $0 | ($85,000) |
| Duplicate invoice records | 3 extra records | 0 extra deposits | $325,000 | $0 | ($325,000) |

All 1,700 bank customer-receipt deposits match a distinct paid invoice by invoice ID and amount. The exported invoice total is $1,306,000. Removing the three duplicated invoice rows ($325,000) leaves $981,000 of unique invoices; subtracting the three open invoices ($85,000) reconciles to the $896,000 deposited in the bank.

Duplicate invoice rows represent **24.9%** of the exported invoice value ($325,000 ÷ $1,306,000).

## Evidence
Sources: `inputs/invoices.csv` (`invoice_id`, `date`, `customer`, `amount`, `status`) and `inputs/bank.csv` (`date`, `description`, `amount`).

### Items that do not match cleanly

| Issue | Invoice ID | Invoice date | Invoice amount | Bank deposit date / amount | Finding |
| --- | --- | --- | ---: | --- | --- |
| Duplicate invoice record | NC-2025-0074 | 2025-01-24 | $100,000 (appears twice) | 2025-01-25 / $100,000 | One deposit supports one invoice; the second invoice row is unsupported. |
| Duplicate invoice record | NC-2025-0327 | 2025-04-02 | $110,000 (appears twice) | 2025-04-03 / $110,000 | One deposit supports one invoice; the second invoice row is unsupported. |
| Duplicate invoice record | NC-2025-0801 | 2025-09-01 | $115,000 (appears twice) | 2025-09-02 / $115,000 | One deposit supports one invoice; the second invoice row is unsupported. |
| No bank deposit; status open | NC-2025-B1 | 2025-03-19 | $30,000 | — | No matching customer receipt in the bank records. |
| No bank deposit; status open | NC-2025-B2 | 2025-06-19 | $28,000 | — | No matching customer receipt in the bank records. |
| No bank deposit; status open | NC-2025-B3 | 2025-09-19 | $27,000 | — | No matching customer receipt in the bank records. |
| Late deposit | NC-2025-1103 | 2025-12-31 | $40,000 | 2026-03-03 / $40,000 | Amount matches, but the deposit occurred 62 days after invoicing; every other matched receipt was deposited one day later. |

There are no bank customer-receipt deposits without an invoice ID and no matched pairs with an amount difference.

## Handoff
The claimed growth is not fully supported by the invoice export. Bank receipts support $896,000 of cash collections. The invoice export adds $325,000 through three repeated paid invoice rows, and $85,000 remains open without bank deposits. Treat the repeated records and the delayed $40,000 receipt as items requiring management support before relying on the growth claim.
