# Tips & Tricks

A grab-bag of things that aren't obvious from just using the app.

## Quick-Add

- **In-line badges instead of typing syntax.** Tap the priority (flag) or tag icon next to the quick-add target pill to set priority/tags from a picker — no need to remember `!high` or `#tag` by hand.
- **Autocomplete for lists and tags.** Start typing `>` or `#` and a suggestion menu pops up; if nothing matches, the top option lets you create that list/tag on the fly.
- **Tap the ⓘ help icon** in the quick-add bar any time for a live cheat-sheet of every shortcut — handy when you forget the exact repeat phrasing.
- **Edit your last-added task** immediately from the quick-add bar using the pencil icon next to the help button, without opening the full app.
- **Voice add.** Fire the `SLR=:=voice_add` command (see [USER_GUIDE.md](USER_GUIDE.md#automation-command-receiver)) to trigger Tasker's speech recognition and quick-add a task by talking — wire it to a Quick Setting tile, a shortcut, or a Bixby/Assistant routine for hands-free capture.
- **Target a specific list without typing `>`.** Tap the list pill at the bottom of quick-add to switch which list new tasks land in for that session.

## Navigating

- **Swipe from the left edge** of the screen to open the drawer (lists, tags, views) — you don't have to reach for the ☰ button.
- **Tap the sort chip's direction arrow** to flip ascending/descending without opening the sort menu.
- **Group without losing your sort.** Grouping (by date, priority, list, tag, recurring) works independently of your chosen sort order, so you can e.g. sort by priority within due-date groups.

## Managing Tasks

- **Long-press the checkbox (punch)** on a task with custom done options (e.g. `Done, Trashed, Bailed`) to choose which one applies, instead of always logging the first.
- **Long-press and drag** a task in manual sort mode to reorder it — grab the handle on the right edge of the row.
- **Snooze with plain English.** Tap "snooze" on an overdue/due-today task and type something like `next friday 3pm` or `in 3 days` instead of using the date/time pickers.
- **Undo almost anything.** Completing, deleting, or editing a task shows a toast with an **Undo** button for a few seconds — it keeps the last 5 actions if you're quick.
- **Alarm mode for recurring tasks.** By default a repeating task's due date only advances once you mark it done. Turn on **Alarm mode** in the task editor to make it advance automatically the moment it's due, whether or not you completed it — useful for "the trash goes out every Tuesday" reminders you don't want piling up.

## Quality of Life

- **Long-press the "open full app" or "back to quick add" icons** to set your default: whether tapping the SLR shortcut opens straight into quick-add-only mode or the full task list next time.
- **Slash dates respect your date-format setting.** If `3/15` keeps getting read the wrong way round, set DD/MM/YY or MM/DD/YY explicitly in **☰ → Date format** instead of relying on auto-detect.
- **Back up before big changes.** Since updates require a fresh reinstall (see [SETUP.md](SETUP.md#updating)), get in the habit of exporting via **☰ → Import / export data** before you do anything drastic.

## More

- [USER_GUIDE.md](USER_GUIDE.md) — full feature reference
- [FAQ.md](FAQ.md) — troubleshooting
