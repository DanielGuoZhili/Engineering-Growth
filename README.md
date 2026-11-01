# Engineering Growth

A measurable, weekly-updated engineering development program aimed at software engineering roles in Japan-based global technology companies.

## Goal
Build transferable skills for Software Engineer, Frontend Engineer, and later AI Application Engineer roles, with Google Japan, Microsoft Japan and Amazon Japan as reference employers rather than the only targets.

## Operating principles
- Plan **one week at a time**. Do not pre-fill months of tasks.
- Prioritize independent coding, debugging, testing, system design, communication, and shipping.
- Distinguish **solo / AI-assisted / AI-generated** work. Commits are evidence of changes, not proof of independent ability.
- Record measurable outcomes: time spent, tests, decisions, blockers, explanations, and artifacts.
- Check official job descriptions and interview guidance weekly; avoid reacting to unverified rumors.
- Never upload client source code, confidential information, or credentials.

## Workflow
1. Read [ROADMAP.md](ROADMAP.md), the current [weekly plan](weeks/2026-W43.md), and [AGENTS.md](AGENTS.md).
2. Complete a task and link the evidence (commit, test result, or written explanation).
3. Record baseline observations in [assessments/baseline.md](assessments/baseline.md).
4. Perform a weekly retrospective using [reviews/2026-W43.md](reviews/2026-W43.md).
5. Only after the review, create the next week's plan.

## Current stage
Week 0 (2026-10-21 to 2026-10-25): measure baseline skill, not maximize output.

> Repository name suggestion: `engineering-growth`. Rename the repository in GitHub Settings -> General -> Repository name; until then, files remain under `SelfStudyDemo`.

## Dual-language algorithm practice

Practice one shared coding-interview problem in **JavaScript and Python**, at least once per week (initial budget: 2–3 hours). Use [Grind 75](https://www.techinterviewhandbook.org/grind75/) to select problems and LeetCode for submissions. Save both independent first attempts and compare them in [practice/algorithms/](practice/algorithms/README.md). Do not pre-fill results or publish AI-authored work as a solo attempt.

### Clone to your Mac (VS Code / Cursor)

Run once in Terminal (change `~/Developer` to your preferred parent folder):

```bash
mkdir -p ~/Developer
cd ~/Developer
git clone https://github.com/DanielGuoZhili/Engineering-Growth.git
cd Engineering-Growth
open Engineering-Growth.code-workspace
```

After the clone, your local folder and this GitHub repository are linked through the `origin` remote. Before each session, run `git pull --ff-only`; after editing, use `git add`, `git commit`, and `git push origin main`. For an existing checkout, use `git pull --ff-only` instead of cloning again. GitHub authentication is required to push.
