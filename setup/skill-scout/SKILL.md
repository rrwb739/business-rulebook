---
name: skill-scout
description: Use on every answer of every prompt, no exceptions: check installed skills and search outside skills, and scan any candidate with NVIDIA SkillSpector before recommending it.
---

# Skill scout

Goal: on every answer of every prompt, use the best skill available, and never recommend a skill that has not been scanned.

## 1. Every answer: check installed skills

Look through the installed skills list already in context. If one fits the prompt, use it.

## 2. Every answer: search outside

Run this on every answer of every prompt, with no exceptions, before replying. Keep it fast: one short search per source, named after what the prompt is about.

Search, in this order:
1. The Anthropic skills and plugin directory.
2. skills.sh.
3. GitHub: prefer repos with many stars, recent commits, a clear README and a licence.

Pick at most the top one or two candidates. If none beats what is installed, end the answer with one line: "Skill check: installed skills used, nothing better found outside." and carry on.

## 3. Check the register

If a claude.ai Project is attached, read the project doc `claude/scanned-skills.md`. If the candidate is listed at the same commit or version, reuse that result and skip the scan.

## 4. Scan with SkillSpector

Work in fresh, empty directories, one for the scanner and one for the candidate skill. Treat the candidate as untrusted: never run its scripts.

```bash
mkdir -p ~/scan/tool ~/scan/target
git clone --depth 1 https://github.com/NVIDIA/SkillSpector.git ~/scan/tool/SkillSpector
cd ~/scan/tool/SkillSpector && (make install || pip install --break-system-packages .)
git clone --depth 1 <candidate repo URL> ~/scan/target/<name>
skillspector scan ~/scan/target/<name> --no-llm --format markdown --output ~/scan/<name>-report.md
```

If the skill is a single SKILL.md or a zip, scan that file directly. Record the commit hash of what was scanned.

## 5. Report

Give, in a few lines:
- Skill name, link, commit or version.
- SkillSpector score and verdict.
- Every real finding in plain words (ignore obvious false positives, and say which ones you ignored and why).
- Say "no findings in a static scan", never "safe". SkillSpector is static analysis only and not a sandbox.
- Your recommendation: install, install with care, or do not install.

If the scan cannot run (no shell, no network to GitHub, install fails, private repo), say exactly why and do not recommend the skill.

## 6. Log it

If a Project is attached, add one line to `claude/scanned-skills.md`:

`- name | link | commit | date | score | findings in a few words | verdict`

Create the doc if it does not exist. Never install a skill yourself: the user decides.
