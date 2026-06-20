# Privacy & safety

Trash Panda is designed as a local-first skill.

## Principles

- No separate Trash Panda backend.
- No SaaS account required.
- The den is plain markdown.
- Nothing is written until the haul is approved.
- Every rescued item should keep a source pointer where possible.

## Export mode

In export mode, your `conversations.json` lives locally in:

```text
den/imports/
```

Trash Panda scans the export, proposes a haul, and writes approved items to markdown files.

## Live mode

In Claude live mode, Trash Panda runs inside your existing Claude Code / Cowork environment and uses the chat/context access available there.

## What not to store

Do not save sensitive secrets, API keys, private credentials, or personal data into your den unless you intentionally want it there.

If a haul contains something sensitive, reject it or edit before saving.
