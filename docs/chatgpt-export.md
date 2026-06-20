# ChatGPT / Claude export mode

Trash Panda can work in two modes:

- **Claude live mode** — `/dig` reads available recent chats inside Claude Code / Cowork.
- **Export mode** — you export your chat history and drop the file into the den.

v0 is honest: ChatGPT uses export mode.

## ChatGPT export flow

1. Open ChatGPT settings.
2. Go to data controls / export data.
3. Request an export.
4. Download the archive when it arrives.
5. Find `conversations.json`.
6. Put it here:

```text
den/imports/conversations.json
```

7. Run:

```bash
/dig export den/imports/conversations.json
```

Trash Panda will scan the export, show a haul, and wait for your approval before writing to project files.

## Claude export flow

If you have a Claude export, use the same pattern:

```text
den/imports/conversations.json
```

Then:

```bash
/dig export den/imports/conversations.json
```

## What gets written?

Approved items are appended to:

```text
den/projects/<project>.md
```

Unclear items go to:

```text
den/inbox.md
```

Each item should keep a source pointer where possible.

## Privacy note

Export mode is designed to be local-first. The export file lives in your local den. Trash Panda does not require a separate backend.
