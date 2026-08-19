# Compound Engineering

![icon](webui/thumbnail.webp)

Agent Zero port of [EveryInc/compound-engineering-plugin](https://github.com/EveryInc/compound-engineering-plugin): 34 skills that make each unit of engineering work easier than the last — brainstorm, plan, debug, review, commit, and compound learnings.

## Skills

All 33 upstream `ce-*` skills (v3.22.4) bundled 1:1, plus `ce-a0-harness-notes`, a thin bridge skill that maps foreign harness tool names (`AskUserQuestion`, `WebFetch`, subagent dispatch, …) to Agent Zero tools (`ask_user_question`, `search_engine`, `call_subordinate`, …). No upstream files are modified.

## Installation

Install from this repository (Plugins dialog → Install → Git URL), or copy this folder to `usr/plugins/compound_engineering/`.

Every skill is toggleable per agent, project, or chat through the built-in `_skills` settings UI.

## Update

Re-copy `skills/` from upstream, keep `ce-a0-harness-notes/`.

## License

MIT — upstream code © Every Inc. (Kieran Klaassen, Trevin Chow), bundled under the same license; see [LICENSE](LICENSE). Port packaging adds no additional restrictions.
