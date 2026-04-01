---
description: Find where something is implemented or used — usage: /search <query>
subtask: true
---

Search the codebase for: $ARGUMENTS

Steps:
1. Search for the term as a symbol (function, class, variable, type name).
2. Search for it as a string literal or comment if the symbol search yields nothing.
3. Look at each match in context — don't just list file names.

Report:
- Where it is defined or implemented (file and line)
- Where it is called or referenced, if relevant
- A one-line summary of what it is, based on what you find

If the query is ambiguous and matches unrelated things, group the results by meaning.
