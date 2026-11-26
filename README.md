# Saxophone Society: Agent Skill and MCP

Official agent skill, MCP configuration and agent rules of the [Saxophone Society by Marjan Markelj](https://marjanmarkelj.de), online saxophone coaching for adults in German.

With it, an AI assistant can answer questions about learning the saxophone as an adult with sources: the programs Academy (beginners) and Circle (advanced players), workshops in Hilden near Düsseldorf, articles on fingerings, sheet music and embouchure, and all 33 saxophone fingerings. With the person's consent it can also reserve the free first call, send a message to Marjan or request a workshop seat. The person always confirms by email.

## Install

Skill (skills.sh):

```
npx skills add MarjanMarkelj/saxophone-society-agents
```

MCP server, for example in Claude Code:

```
claude mcp add --transport http saxsoc https://marjanmarkelj.de/wp-json/saxsoc/v1/mcp
```

The repository is also an [Agent Plugin](https://agent-plugins.org) (`plugin.json`, `mcp.json`, `skills/`).

## Contents

| File | Purpose |
| --- | --- |
| [`AGENTS.md`](AGENTS.md) | Rules for coding agents that build on the API and MCP |
| [`skills/saxsoc-public-info/SKILL.md`](skills/saxsoc-public-info/SKILL.md) | Agent skill, identical to https://marjanmarkelj.de/SKILL.md |
| [`plugin.json`](plugin.json), [`mcp.json`](mcp.json) | Agent Plugin manifest and MCP servers |
| [`.mcp.json`](.mcp.json), [`.cursor/mcp.json`](.cursor/mcp.json) | MCP servers for Claude Code and Cursor |

## Links

- Developer docs: https://marjanmarkelj.de/ki-dokumentation/
- OpenAPI: https://marjanmarkelj.de/wp-json/saxsoc/v1/openapi
- llms.txt: https://marjanmarkelj.de/llms.txt
- MCP Registry: `de.marjanmarkelj/saxsoc-public-info`

## Auf Deutsch

Offizieller Agenten-Skill und MCP-Zugang der Saxophone Society von Marjan Markelj. KI-Assistenten beantworten damit Fragen zum Saxophon lernen als Erwachsener mit Quellen und können mit Zustimmung der Person das kostenlose Erstgespräch vormerken. Fest wird es erst, wenn die Person den Link in ihrer Mail bestätigt. Preise nennt die Schnittstelle nicht.

Die Inhalte entstehen im Website-Projekt und werden von dort hierher übertragen. Änderungen bitte nicht direkt hier, sondern über das Kontaktformular: https://marjanmarkelj.de/kontakt/
