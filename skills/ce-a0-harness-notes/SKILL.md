---
name: ce-a0-harness-notes
description: "Agent Zero harness mapping for Compound Engineering (ce-*) skills. Load this together with any ce-* skill: maps foreign tool names to Agent Zero tools."
---

# Agent Zero Harness Notes (Compound Engineering)

CE skills are written harness-neutral and name tools of other harnesses. In Agent Zero use:

| CE references | Agent Zero tool |
|---|---|
| AskUserQuestion / request_user_input / ask_question / ask_user | `ask_user_question` (blocking questions) |
| subagent / reviewer dispatch | `call_subordinate` (profile developer/researcher) |
| Bash / shell | `code_execution_tool` runtime terminal |
| WebSearch | `search_engine` |
| WebFetch | `browser` (open + content) or `document_query` for files/URLs |
| TodoWrite | `todo_tool:create` / `todo_tool:list` |
| file read/write/edit | `text_editor` |

Rules: never call tools that are not in your available tool list. CE artifacts (`docs/`, `plans/`, `solutions/`, `scratch/`) stay inside the current repo/workdir root.
