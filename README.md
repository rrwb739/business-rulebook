Business rulebook version: v449 | index: instructions.md | rule text: the rules files named in the index | updated: 2026-11-18

# Business rulebook

A general rulebook for running and growing a business with Claude. It holds methods only: offers, leads, sales, money models, delivery, team, writing, the scaling roadmap and legal basics. Your business's own facts and decisions stay in your own project, never in this repo.

## What is in here

- instructions.md: the method Claude follows on every prompt.
- instructions-index-1.md, instructions-index-1b.md, instructions-index-2.md, instructions-index-2c.md and instructions-index-2b.md: the index of every rule, one line each.
- rules-*.md: the full text of each rule, one or more files per section.
- rules-cases.md and rules-cases-b.md: case patterns (K), strategies that worked for one kind of business, written in general words so any business can borrow them.
- templates/instructions-box.md: what to paste into your project's instructions box.
- templates/business-filters.md: the F33 questions to answer before choosing a business.
- prompts/: the first message for each chat tab.
- setup/skill-scout.zip: the skill-scout skill to install on your Claude account (step 3).
- tools.md: the tools register, reviewed tools listed by the roadmap stage they're for.
- CHANGELOG.md, CHANGELOG-1.md, CHANGELOG-2.md and CHANGELOG-3.md: what changed in each version (newest first in CHANGELOG.md; older entries in CHANGELOG-1.md, then CHANGELOG-2.md; oldest in CHANGELOG-3.md).

## Set up a business project

1. In Claude, create a new project for your business.
2. In the project's files, choose Add from GitHub and add this repository (all files).
3. Install the skill-scout skill once on your Claude account: download setup/skill-scout.zip from this repo, upload it in Claude's settings where skills are managed, and make sure it is switched on. It works in every project you have, now and later.
4. If no business is chosen yet, answer templates/business-filters.md first (F33). Then open templates/instructions-box.md, copy it into the project's instructions box, and fill in the fields. Write "not decided" for anything you don't know yet. Claude will propose those and mark them "Proposed, not decided" until you confirm them.
5. Create one chat per tab and name them: Strategy, Daily numbers, Offer and money models, Marketing, Sales, leads and delivery, Weekly review.
6. Start in Strategy. Paste the first message from prompts/strategy.md. It sets your roadmap stage and fills the gaps in your instructions box. Then open the other tabs in the order above, each with its own first message from prompts/. From then on, start every working day in Daily numbers: paste the day's figures and it gives you the ratio and the one next action.
7. When Claude proposes a fact or decision you agree with, paste the line it gives you into the instructions box yourself. The box is the only place your business's decisions live.

## Updating

The version line at the end of every answer shows which version the chat used, and CHANGELOG.md lists what changed. If the version line is behind the top of CHANGELOG.md, sync the GitHub files in your project. Your instructions box is never touched by an update; when the instructions-box template's Method block changes (as in v426), copy the new Method block into your box once, keeping your facts and decisions.

## Ground rules

- Legal rules are marked [Fixed] and always win. They are general guidance, not legal advice: confirm with a qualified adviser for your country.
- Rules tagged [shape: ...] fit only that kind of business; rules tagged [stage: ...] apply only from that roadmap stage.
- Every answer runs F34's five steps, then F31's 80/20 method, and gives mainly "The 20% that gets 80%" (one to three actions, how to do each, each with its number), then one closing line with the rules applied, the rules considered but not applied, the number of passes, the Skill check line and the version line. If an answer doesn't, ask Claude to follow instructions.md.
