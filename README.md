# Shivam Kapoor

Product manager for platform and AI products. I started as a software engineer.

I build and run AI agent systems in my own time. I manage them like a product: each part gets a goal, a number that measures it, a check that fails loud, and a written rule for every mistake I catch. The case studies show where that holds and where it does not yet.

## Start here

| Repo | What it shows |
|---|---|
| [ai-workflows](https://github.com/DadyByte/ai-workflows) | How I run AI agents as a system: a nightly job that files what my AI sessions learned, search over my own notes with a benchmark that keeps it honest, model choice by evaluation, and multi-agent review. Written as case studies, with the numbers and the failures. |
| [claude-skills](https://github.com/DadyByte/claude-skills) | Skills and subagents I designed for Claude Code. Claude Code wrote most of the text under my direction. Several keep the dated rules I added after a run failed. |
| [apollo-paints](https://github.com/DadyByte/apollo-paints) | A live catalog site for an industrial paint maker, [apollopaintsglobal.com](https://apollopaintsglobal.com). First screens from Google Stitch, the React app generated in Google AI Studio and adapted with Claude, served from Cloudflare Workers. |

## How I work with AI

- **Evaluate before trust.** A nightly job that files what my AI sessions learned went live only after a five-night trial that proposed changes without making them, and after it met a pass bar I set on a gold set. I lowered that bar twice on the way, and the case study shows each setting and what still fails. [The night shift](https://github.com/DadyByte/ai-workflows/blob/main/workflows/03-night-shift.md)
- **The right model for each step.** The top model plans and reviews. Cheaper models execute. In a four-way test for that nightly job, Sonnet found 49 of 70 reachable gold items. Opus found 48 at 1.8 times the price. Haiku was the cheapest but found fewer of the decisions and tasks (56.7% against 70.0%). The job runs on Sonnet. [Model routing](https://github.com/DadyByte/ai-workflows/blob/main/playbook/model-routing.md), [the test](https://github.com/DadyByte/ai-workflows/blob/main/workflows/03-night-shift.md)
- **Read before deriving.** Each session is set up to read what my notes already hold before it works, and to write back what it learned. I track how many sessions query my notes first: 55% in the last measured week. That is the number I work to move. [The session loop](https://github.com/DadyByte/ai-workflows/blob/main/workflows/01-session-loop.md)
- **Fail loud.** A gate with no model in it re-indexes search and runs a retrieval benchmark each time a session is wrapped up, and it prints a red line when a step fails. A weekly audit checks what the documentation claims against what is on disk. [Gate and audits](https://github.com/DadyByte/ai-workflows/blob/main/workflows/05-gate-and-audits.md)
- **Every correction becomes a rule.** A mistake is written down once, with its date. Where a written note keeps failing, a hook, a check or a scheduled job enforces it. [Operating rules](https://github.com/DadyByte/ai-workflows/blob/main/playbook/operating-rules.md)
- **Review before it ships.** Narrow reviewers read the same change in parallel, and a skeptic tries to refute each finding before it reaches me. These repos went through that review before I published them, and the page records what it found. [Multi-agent review](https://github.com/DadyByte/ai-workflows/blob/main/workflows/07-multi-agent-review.md)

## About me

- Product Manager at Microsoft since 2021. Platform and AI products.
- MBA from IIM Calcutta. B.Tech in Computer Engineering from DTU.
- I write on [Medium](https://medium.com/@shivamkapoor1607).
- [LinkedIn](https://www.linkedin.com/in/shivamkapoor1607)

<sub>These are personal projects, built on my own time with my own tools. Views are my own.</sub>
