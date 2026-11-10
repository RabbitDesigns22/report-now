# report-now

**A report of right now, not of yesterday.**

`report-now` is an agent skill for Claude Code (and any agent that reads `SKILL.md` skills). When you ask "what's the status?", many agents paste the last report they wrote, hours or days old. `report-now` makes the agent read the real time, check every live source at that moment (services, numbers, queues, errors), and deliver a dated, complete report: bottom line, status by area, problems found now, what needs you, and what it could not verify.

Ask "give me the report" and get one checked at this minute, with the time on it.

## See the difference

> **You:** How is the campaign going?

**Without the skill:** it pastes the status it wrote three hours ago, as if it were current.

**With the skill:** "Let me check it right now", then it reads every live source at that minute and answers with the exact time it looked, plus what it could not verify.

**Skip it if** there is nothing live to check (no services, numbers or queues).

**Status:** in daily use in the author's own setup. Plain instructions, no scripts, no network calls. MIT. Issues and suggestions welcome.

## Install

With the [skills CLI](https://skills.sh):

```bash
npx skills add RabbitDesigns22/report-now
```

Or manually: copy `skills/report-now/` into `~/.claude/skills/` for all your projects, or into `.claude/skills/` for one project.

To make every session use it, add this line to your `CLAUDE.md`:

```
When the user asks for a report or a status, load the report-now skill.
```

## Works well with

- [`hands-on`](https://github.com/RabbitDesigns22/hands-on): the agent does every step it can and asks you only for what it cannot do.
- [`one-answer`](https://github.com/RabbitDesigns22/one-answer): one checked, final answer instead of plan, correction, plan.
- [`never-twice`](https://github.com/RabbitDesigns22/never-twice): a shared error log so the same mistake never happens twice.

## Español

**El reporte de ahorita.** Cuando preguntas "¿cómo va todo?", muchos agentes te pegan el último reporte que hicieron, de hace horas o días. `report-now` obliga al agente a ver la hora real, revisar en ese momento cada fuente en vivo (servicios, números, pendientes, errores) y darte un reporte serio con fecha y hora: lo importante primero, cómo está cada área, problemas encontrados ahora, qué necesita de ti y qué no pudo comprobar.

Instalar: `npx skills add RabbitDesigns22/report-now`

## More skills from the same setup

These come from one real workflow: a small agency run with 15+ Claude Code sessions in parallel. Each skill fixes one problem that kept happening there.

| Skill | What it fixes |
|---|---|
| [one-pass](https://github.com/RabbitDesigns22/one-pass) | get it right the first time; stop paying tokens for rework |
| [hora-exacta](https://github.com/RabbitDesigns22/hora-exacta) | real date and time in every message, so nothing lands on the wrong day |
| [hands-on](https://github.com/RabbitDesigns22/hands-on) | the agent does what it can and only asks you for codes, keys and payments |
| [easy-for-them](https://github.com/RabbitDesigns22/easy-for-them) | steps people actually follow: direct link, one action per line |
| [one-answer](https://github.com/RabbitDesigns22/one-answer) | one thought-through answer instead of plan, fix, new plan |
| [never-twice](https://github.com/RabbitDesigns22/never-twice) | a shared error log so no session repeats a known mistake |
| [sort-me-out](https://github.com/RabbitDesigns22/sort-me-out) | one ordered list of what is urgent, waiting and forgotten |
| [in-the-loop](https://github.com/RabbitDesigns22/in-the-loop) | a live board so parallel sessions know what the others changed |
| [study-first](https://github.com/RabbitDesigns22/study-first) | reads everything in full and answers point by point, no invented details |
| [session-watchdog](https://github.com/RabbitDesigns22/session-watchdog) | wakes the sessions that got stuck mid-task, leaves the rest alone |
| [skill-harvest](https://github.com/RabbitDesigns22/skill-harvest) | reads your sessions and finds the skills you are missing |
| [small-budget-ads](https://github.com/RabbitDesigns22/small-budget-ads) | Meta Ads rules for 1-5 USD a day ad sets |
| [whatsapp-closer](https://github.com/RabbitDesigns22/whatsapp-closer) | evidence-ranked rules for a WhatsApp sales assistant that closes |
| [whatsapp-number-onboarding](https://github.com/RabbitDesigns22/whatsapp-number-onboarding) | connect a number to the WhatsApp Cloud API in the safe order |
| [proposal-pdf](https://github.com/RabbitDesigns22/proposal-pdf) | short PDF proposals with every price checked against its source |
| [published-vs-planned](https://github.com/RabbitDesigns22/published-vs-planned) | says "published" only for what it saw live on the public page, Facebook and Instagram checked apart |
| [source-every-fact](https://github.com/RabbitDesigns22/source-every-fact) | every price, phone and name on a post traced to its source, nothing added |

If one of them saved you a redo, a star helps other people find it.

## License

MIT. Made by [Rabbit Designs](https://github.com/RabbitDesigns22).
