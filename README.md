# claude-verification-rules

A Claude Code plugin that injects mandatory verification rules at the start of every session — before CLAUDE.md and all other rules load.

## What it does

Forces Claude to:

1. **Verify before touching files** — every technical claim must have evidence first
2. **Do one complete review pass** — not incremental passes that miss issues
3. **Avoid the confident-assertion anti-pattern** — look hard before implementing, not after being challenged

## Install

```bash
claude plugin install github.com/tedin7/claude-verification-rules
```

## How it works

Uses a `SessionStart` hook to inject the rules as a `<system-reminder>` before any other context loads.
