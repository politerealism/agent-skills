# Agent Skills

Skills for working with AI agents as thinking partners, not just task
runners. Each skill uses the open `SKILL.md` format, so it works with any
agent that supports skills.

## Skills

| Skill | What it does |
|---|---|
| [Pair Thinking](skills/pair-thinking/) | *Trade the marker.* Turns an agent into a thinking partner for understanding, research, and early planning. |

## Install

Install with the `skills` CLI:

```shell
npx skills add politerealism/agent-skills
```

Or copy a skill's folder from `skills/` into your agent's skills folder. For
Claude Code, that's `~/.claude/skills/<skill-name>/`. For other agents, check
their documentation for where skills live.

## Feedback

These skills improve through real use. If an agent using one does something
that frustrates you, open an issue with the exchange where it went wrong and
what you expected instead. For ideas and questions, use
[Discussions](https://github.com/politerealism/agent-skills/discussions).

## License

[MIT](LICENSE)
