# Team workflow

1. At the start of every session, if the branch is role/<role>-<firstname>, greet the student by name. Otherwise ask one question at a time: full name; role (Accountant, Financial Analyst, Fraud Auditor, Investment Manager, Customer Analyst); whether they are the team leader. The leader takes Investment Manager. Run `git fetch`. Role names in branches and review filenames use accountant, financial_analyst, fraud_auditor, investment_manager, customer_analyst. Check local and origin role branches; if a branch for that role already exists, say it is taken and ask for an available role. Create role/<role>-<firstname> from origin/main and push it. Use a lowercase first name. Explain once at onboarding: Saved means committed on your laptop. Uploaded means pushed to GitHub. Merged means added to the team's main. Silently create the student's review file at joining with an ISO join time; keep that time and reminder flags on return visits.
2. Students edit only their own role folder. Never edit inputs/, shared/, other roles, or AGENTS.md. If asked, explain that doing so would cause merge conflicts. The workflow may update only that student's review file. The leader may build final/ after all claimed roles are DONE and the leader confirms the team is complete.
3. Use only inputs/ for facts. No web search.
4. Plan before big changes. Show what changed after each step.
5. If a student says "done", "looks good", "finished", "I'm done", "submit", or similar, ask: "Ready to submit your work to the team? Reply yes." On yes, ask: "Which input file did you check your work against?" Record their answer, or "unable to answer", in their review file; never block submission if they cannot answer. Then commit their work, push their branch, update their review file using the format below, and commit and push that note before merging into main: `git checkout main && git pull && git merge <their branch> && git push`. If a push is rejected, run `git pull` (no rebase), then push again. Never force-push. If a conflict appears, stop and tell the leader.
6. Every session, run `git fetch`. A role counts as CLAIMED when its role/<role>-<name> branch exists on origin. A claimed role counts as DONE only when, on origin/main, its role file differs from the template AND its matching .review/<role>_<name>.md file exists. Count each known role once. The template is that file's first-added version on origin/main, including files added after the repository's first commit. Compare files and look for reviews on origin/main, not a working folder or role branch. An empty pushed branch or a review alone does not count as DONE. Show: "X of Y done. Waiting on: <roles>" (Y = claimed roles; this team expects 5). List only claimed, unfinished roles; use "none" when all are done. When Y is greater than zero and all claimed roles are DONE, ask the leader: "Y people have joined. Is that everyone on your team?" Replace Y with the count. Only after the leader says yes, say: "Everything is merged. Start final/." If someone else joins, recheck the count and ask again before final/. The leader works in final/ only, on a branch from main, then merges it back when the team agrees.
7. Keep one review file per student at .review/<role>_<firstname>.md and update it when they say done. Do not mention it unprompted. If asked, honestly say short session notes are saved for the instructor. Base notes only on observed work; write n/a if not observed. Score only what the student typed, decided, or checked. Note work Codex produced without student input as "Codex-led" within an existing evidence line; do not credit it to the student. Maximum 12 lines.
8. After every Git action, show: "Saved on your laptop ✅/❌ · Uploaded to GitHub ✅/❌ · Added to team's main ✅/❌". Choose one truthful emoji for each state of the student's current work; an empty branch is not submitted work.
9. On each student turn, use the review file's join time. At 30+ minutes, say once: "About 15 minutes left for your part. Aim to say done by minute 45." At 40+ minutes, suggest finishing what they have and submitting. Save each reminder flag in the Session line; preserve flags on return visits.

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
Session: joined <ISO time>; reminded30: yes/no; reminded40: yes/no
Source check: <input file named by student, or unable to answer>
