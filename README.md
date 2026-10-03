# Portable Context

A skill for keeping useful context in a store you own, so another AI assistant can pick up the work without making you explain everything again.

## Why this exists

As assistants become more persistent and capable of acting on our behalf, the cost of switching grows. An assistant learns preferences, remembers corrections, and accumulates the history behind decisions. Some of that context lives in explicit notes; some lives in provider memory; much of it stays buried in conversations.

A personal knowledge base (such as Obsidian or Notion) helps, but it only contains what makes it into the knowledge base. The missing piece is a habit for assistants: read the relevant context before working, then preserve the meaningful changes as work happens.

The goal is to make trying another assistant practical. You should be able to choose a service for its capabilities without rebuilding your working relationship from scratch. Your decisions, constraints, and unfinished work should remain understandable outside the service that first recorded them.

Portable Context makes that habit explicit. It preserves more than facts about you: why an option was rejected, if any decisions were made, where an artifact lives, and what would make the next conversation useful.

## How it works

The [skill](SKILL.md) reads relevant notes, saves meaningful decisions and stopping points, reconciles corrections, and verifies changes. It follows your existing organization, preserves sources and rationale, and keeps proposals distinct from decisions.

## Setup

1. Put this repository where your assistant can read it.
2. Adapt the [context map](examples/context-map.example.md) in your private store, or use existing vault instructions. Specify locations, routing, and capture scope.
3. Add the [standing instruction](examples/standing-instruction.md) to each assistant's persistent instructions, replacing the placeholders. Explicitly enable automatic capture for your chosen scope.
4. Confirm access, then test whether a fresh conversation can recover a saved decision, its reason, and the next step.

Each assistant needs its own access. Keep personal notes and filled-in configuration outside this public repository.

## Limits

This skill provides instructions, not storage or synchronization. It cannot read hidden provider memories, transfer permissions or running jobs, or guarantee compliance. Your storage handles concurrent writes; deletion is limited to accessible, authorized records. Capture does not authorize external actions, historical backfills, or schedules. No-save requests still apply.

## Contributing

Improvements, fictional test cases, and host setup examples are welcome. Keep contributions free of personal data and credentials.

## License

[MIT](LICENSE).
