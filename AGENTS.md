# Team workflow

1. At the start of every session, if the branch is role/<role>-<firstname>, greet the student by name. Otherwise ask one question at a time: full name; role (Accountant, Financial Analyst, Fraud Auditor, Investment Manager); whether they are the team leader. The leader takes Investment Manager. Run `git fetch`. Role names in branches and review filenames use accountant, financial_analyst, fraud_auditor, investment_manager. Check local and origin role branches; if a branch for that role already exists, say it is taken and ask for an available role. Create role/<role>-<firstname> from origin/main and push it. Use a lowercase first name.
2. Students edit only their own role folder. Never edit inputs/, shared/, other roles, or AGENTS.md. If asked, explain that doing so would cause merge conflicts. The workflow may update only that student's review file. The leader may build final/ after all roles are DONE.
3. Use only inputs/ for facts. No web search.
4. Plan before big changes. Show what changed after each step.
5. When a student says done, commit their work, push their branch, update their review file using the format below, and commit and push that note before merging into main: `git checkout main && git pull && git merge <their branch> && git push`. If a push is rejected, run `git pull` (no rebase), then push again. Never force-push. If a conflict appears, stop and tell the leader.
6. Every session, run `git fetch`. A role counts as DONE only when, on origin/main, BOTH are true: (a) its role file is different from the starting template, and (b) its .review/<role>_<firstname>.md file exists. A pushed branch with no work does NOT count. The starting template is the role file in the repository's first commit (find it with `git rev-list --max-parents=0 origin/main`). Check both the changed role file and matching review file on origin/main, not just the current branch. Tell the student in one line, e.g. '3 of 4 done. Waiting on: Accountant.' Only when all 4 are DONE, tell the leader: 'Everything is merged. Start final/.' The leader works in final/ only, on a branch from main, then merges it back when the team agrees.
7. Keep one review file per student at .review/<role>_<firstname>.md and update it when they say done. Do not mention it unprompted. If asked, honestly say short session notes are saved for the instructor. Base notes only on observed work; write n/a if not observed. Maximum 12 lines.

## Review format
# <Name> - <Role>
Worked: YES / PARTIAL / NO (commits: N, role file filled: yes/no)
S1 Model limits: x/5 - <few words of evidence>
S2 Prompting (role, context, format, iterating): x/5 - <evidence>
S3 Git & Codex use (branch, commits, reads diffs): x/5 - <evidence>
S4 Verification & context (checks inputs, plan first): x/5 - <evidence>
S5 Workflow (breaks work down, teamwork handoffs): x/5 - <evidence>
Overall: x/25
Strength: <one line>
Improve: <one line>
