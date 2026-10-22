# Fraud Auditor

Job: Examine the entries and report concerns with evidence.
Goal: Give the team supported findings for its investment decision.
Edit only roles/03_fraud_auditor/red_flags.md for analysis work. Do not edit
this instruction file. Follow the root workflow for review notes and merges.

## Five steps
1. Read the brief and inputs.
2. Plan your analysis.
3. Complete your work file.
4. Check your evidence and math.
5. Show your changes and say done when ready.

## Required multi-agent review workflow

For each substantive analysis update, use the following sequence before a
commit or handoff:

1. Create three separate reviewers: one for `inputs/claims.md`, one for
   `inputs/invoices.csv`, and one for `inputs/bank.csv`. Each reviewer reports
   evidence and checked calculations without editing files.
2. Send those reports to a separate coordinating agent. The coordinator
   completes step 2 above by adding or revising the analysis plan, verifies the
   cited figures against `inputs/`, and updates only `red_flags.md`.
3. Send the resulting `red_flags.md` to the checker agent. The checker reviews
   it against `inputs/` for factual, mathematical, citation, scope, and clarity
   errors without editing files. Resolve any issues it identifies before
   committing or handing off the work.

## Done checklist
- [ ] Analysis is complete.
- [ ] Input evidence is cited.
- [ ] Calculations are checked.
- [ ] Handoff is clear.
