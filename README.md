# Is This Startup Lying?

NovaCart, an online grocery startup, says it grew 300% last year and wants $500,000 from your investor.

Recommend invest, pass, or invest with conditions, using the books.

## Inputs
- inputs/claims.md: management pitch and reporting context.
- inputs/invoices.csv: 2024–2025 invoice register.
- inputs/bank.csv: bank transactions from 2024 through March 2026.

## Roles
| Role | Work file | Job |
| --- | --- | --- |
| Accountant | roles/01_accountant/matching.md | Match each invoice to a bank deposit. List what does not match. |
| Financial Analyst | roles/02_financial_analyst/profit.md | Calculate revenue, costs, profit, and growth for 2024 and 2025. |
| Fraud Auditor | roles/03_fraud_auditor/red_flags.md | Examine the entries and report concerns with evidence. |
| Investment Manager (leader) | roles/04_investment_manager/forecast.md | Build a next-12-month forecast and recommend an investment decision. |

## Rules
Edit your own role folder. Keep inputs/ and shared/ read-only. Follow AGENTS.md for branches, review, and merging. The Investment Manager is the team leader.

Hidden problems are in the inputs. Finding them is part of your score.
Use only files in inputs/. Prove your answer is right.

## Timeline
- 0–10 minutes: read and make branches.
- 10–50: do your role.
- 50–60: merge.
- 60–80: leader builds final/, team reviews.
- 80–90: rehearse.

## Final work
The leader creates final/memo.md: one page with the decision, numbers, and every red flag; and final/presentation_outline.md: a five-minute presentation.
