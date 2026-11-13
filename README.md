Business rulebook version: v142 | index: instructions.md | rule text: the rules files named in the index | updated: 2026-11-11

# Business rulebook

A general rulebook for running and growing a business with Claude. It holds methods only: offers, leads, sales, money models, delivery, team, writing, the scaling roadmap and legal basics. Your business's own facts and decisions stay in your own project, never in this repo.

## What is in here

- instructions.md: the method Claude follows on every prompt.
- instructions-index-1.md, instructions-index-1b.md, instructions-index-2.md and instructions-index-2b.md: the index of every rule, one line each.
- rules-*.md: the full text of each rule, one or more files per section.
- rules-cases.md and rules-cases-b.md: case patterns (K), strategies that worked for one kind of business, written in general words so any business can borrow them.
- templates/instructions-box.md: what to paste into your project's instructions box.
- templates/business-filters.md: the F33 questions to answer before choosing a business.
- prompts/: the first message for each chat tab.
- tools.md: the tools register, reviewed tools listed by the roadmap stage they're for.
- CHANGELOG.md: what changed in each version.

## Set up a business project

1. In Claude, create a new project for your business.
2. In the project's files, choose Add from GitHub and add this repository (all files).
3. If no business is chosen yet, answer templates/business-filters.md first (F33). Then open templates/instructions-box.md, copy it into the project's instructions box, and fill in the fields. Write "not decided" for anything you don't know yet. Claude will propose those and mark them "Proposed, not decided" until you confirm them.
4. Create one chat per tab and name them: Strategy, Daily numbers, Offer and money models, Marketing, Sales, leads and delivery, Weekly review.
5. Start in Strategy. Paste the first message from prompts/strategy.md. It sets your roadmap stage and fills the gaps in your instructions box. Then open the other tabs in the order above, each with its own first message from prompts/. From then on, start every working day in Daily numbers: paste the day's figures and it gives you the ratio and the one next action.
6. When Claude proposes a fact or decision you agree with, paste the line it gives you into the instructions box yourself. The box is the only place your business's decisions live.

## Updating

Business projects pick up each new version from GitHub automatically; there is nothing to sync. The version line at the end of every answer shows which version the chat used, and CHANGELOG.md lists what changed. Your instructions box is never touched by an update.

## Ground rules

- Legal rules are marked [Fixed] and always win. They are general guidance, not legal advice: confirm with a qualified adviser for your country.
- Rules tagged [shape: ...] fit only that kind of business; rules tagged [stage: ...] apply only from that roadmap stage.
- Every answer ends with "The 20% that gets 80%", the rules applied, the rules considered but not applied, the number of passes, and the version line. If an answer doesn't, ask Claude to follow instructions.md.
