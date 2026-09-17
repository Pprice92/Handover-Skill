---
description: Write full working memory to a handover file before ending a session
user-invocable: true
disable-model-invocation: true
---

Write a complete handover document to `.claude/memory/handover.md` (overwrite it, don't append).
Include:
- Current goal and where the project stands right now
- Key decisions made so far and the reasoning behind them
- Files touched, with a one-line note on what changed and why
- Open questions, blockers, and anything unresolved
- Explicit next steps for the following session, in order

Then run these commands in the terminal:

```
git add .claude/memory/handover.md
git commit -m "chore: handover checkpoint"
git push
```

Confirm the push succeeded before finishing.
