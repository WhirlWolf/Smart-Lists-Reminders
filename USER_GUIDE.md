# User Guide

## Quick Add

Type naturally in the quick-add bar (or after `@slr`) — SLR parses out the structure and leaves the clean title behind.

| Type | Syntax | Example |
| --- | --- | --- |
| List | `>listname` | `>Work` |
| Tag | `#tagname` | `#errand` |
| Priority | `!high` `!med` `!low` `!none` (or `!h` `!m` `!l` `!n`) | `!high` |
| Repeat | `daily`, `weekly`, `monthly`, `yearly`/`annually`, `weekdays`, `every 2 days`, `every 3 weeks`, `every 4 hours`, `every 15 min` | `every 2 days` |
| Date | `today`, `tonight`, `tomorrow`/`tmrw`, `fri`, `next fri`, `this weekend`, `next weekend`, `mar 15`, `3/15`, `in 3 days`, `in 2 weeks` | `next fri` |
| Time | `3pm`, `3:30pm`, `15:00`, `noon`, `midnight`, `morning`, `afternoon`, `evening`, `night` | `3pm` |
| Subtask | Start a new line with `-` | `- pick up milk` |
| Escape a symbol | Prefix with `\` to keep it literal | `\!important` |

Example: `Call mom tmrw 3pm #family !high`

Slash dates like `3/15` follow the date-format setting in the drawer menu (**☰ → Date format**) — auto-detected from your device by default, or force DD/MM/YY or MM/DD/YY.

### `@slr` anywhere

Type `@slr` in any text field on your device (a message, a note, a browser search box) and SLR pops open quick-add, using the Accessibility Monitor to detect the keyword and clear it from the field. See [SETUP.md](SETUP.md) if this isn't working.

### Share to SLR

Share text, a link, or a file from any app using Android's share sheet and choose **"Add as Task"** — the shared content becomes the task title.

## Views & Organization

- **Smart views**: Today, Upcoming, All, Starred, Completed
- **Lists**: custom lists, each with its own color and optional icon
- **Tags**: custom tags, each with its own color
- **Sorting**: manual, due date, priority, title, creation date, starred, subtask count, recurring status, or list — with ascending/descending toggle
- **Grouping**: group any view into sections by date, priority, list, tag, or recurring status
- **Search**: matches both task text and notes

## Working with Tasks

- **Subtasks** — add via the `-` shortcut in quick-add, or the task editor
- **Notes** — free text per task
- **Custom done options** — e.g. `Done, Trashed, Bailed`; the first is the quick tap, hold the checkbox for the rest
- **Starring** — pin important tasks regardless of sort
- **Recurrence** — daily/weekly/monthly/yearly, weekdays, custom intervals down to the minute, specific days of week or month; optional **alarm mode** rolls the due date forward as soon as it's due, whether or not you complete it
- **Snoozing** — quick presets (later today, tomorrow, this weekend, next week, in a month) or type a snooze time in plain English
- **Stats** — tasks completed today, in the last 7 days, and your current streak (**☰ → Stats**)
- **Import/export** — your task data as portable JSON (**☰ → Import / export data**)

## Automation (Command Receiver)

SLR exposes a command interface so other Tasker tasks and profiles can drive it directly. Fire the `SLR - commandReceiver` event with a `SLR=:=` prefixed command:

```
SLR=:=add
SLR=:=edit/toggle
SLR=:=toggle
SLR=:=select_view
```

The part before `=:=` is the command; everything after is passed as parameters (`%command`, `%par`, `%command_parameter`, `%command_parameters()`). See the **SLR - commandReceiver** profile's relevant variables for the full list, and the **SLR - actions** task for how each command is handled internally.

## Widget & Notification

- **Widget** — drop the SLR widget on your home screen for at-a-glance task access; tap a task to mark it done, long-press for quick-add
- **Notification** — persistent notification view of your tasks, driven by the **SLR - Timed Tasks** and **SLR - allDayTasks** profiles

## More

- [SETUP.md](SETUP.md) — installation and updates
- [TIPS.md](TIPS.md) — tips, tricks, and hidden shortcuts
- [FAQ.md](FAQ.md) — troubleshooting
