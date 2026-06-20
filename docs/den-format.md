# Den format

The den is a folder of plain markdown files.

Recommended structure:

```text
den/
├── index.md
├── inbox.md
├── imports/
│   └── conversations.json
├── hauls/
│   └── 2026-06-19.md
└── projects/
    ├── trash-panda.md
    ├── ai-product-club.md
    └── toloka.md
```

## `den/index.md`

Dashboard of the den:

- last dig
- recent hauls
- active projects
- open To Do’s
- untriaged inbox items

## `den/inbox.md`

For rescued items that do not clearly belong to a project yet.

## `den/hauls/YYYY-MM-DD.md`

The raw haul from a dig session.

A haul should include:

- number of chats scanned
- items found
- items approved / rejected
- source links where possible

## `den/projects/<project>.md`

A project file should include:

```md
# Project name

## 📝 To Do’s

- [ ] Task with source link. [↗ source]

## 💎 Shiny

- Idea worth revisiting. [↗ source]

## 🗺️ The Plan

- Current direction / route / next steps. [↗ source]

## 📜 Loot

- Reusable draft, spec, prompt, note. [↗ source]
```

## Design rules

- Prefer artifacts over summaries.
- Preserve backlinks.
- Deduplicate aggressively.
- Respect hand edits.
- Keep markdown readable without any app.
