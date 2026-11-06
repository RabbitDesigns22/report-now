# report-now

**A report of right now, not of yesterday.**

`report-now` is an agent skill for Claude Code (and any agent that reads `SKILL.md` skills). When you ask "what's the status?", many agents paste the last report they wrote, hours or days old. `report-now` makes the agent read the real time, check every live source at that moment (services, numbers, queues, errors), and deliver a dated, complete report: bottom line, status by area, problems found now, what needs you, and what it could not verify.

Ask "give me the report" and get one checked at this minute, with the time on it.

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

## License

MIT. Made by [Rabbit Designs](https://github.com/RabbitDesigns22).
