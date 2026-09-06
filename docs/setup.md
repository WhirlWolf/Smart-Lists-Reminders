# Setup

## Prerequisites

- [Tasker](https://play.google.com/store/apps/details?id=net.dinglisch.android.taskerm) 6.7.6-beta or newer
- Tasker's **Accessibility Monitor** enabled in Android Settings — required for the `@slr` keyword watcher to detect what you type in other apps

## Install

1. [Import the project](https://taskernet.com/shares/?user=AS35m8m8L9YzBV3qbzaAAqHiSYXYBbD3QfZ7hr0hRK4ojOFTCrjWh2CScbjMw4NaudRi1zKKzq85&id=Project%3ASmart+Lists+%26+Reminders) from Taskernet.
2. Grant the permissions when prompted.
3. In Android Settings, go to **Accessibility** and turn on Tasker's accessibility service if it isn't already.
4. Run the **SLR - Setup** task once to finish configuration.
5. Type `@slr` anywhere on your device to open quick-add, or from the widget.

## Updating

Note

Because Tasker projects don't diff cleanly, **updating requires deleting the old project and doing a fresh import** rather than importing over it.

1. Delete the existing "Smart Lists & Reminders" project in Tasker.
2. [Import the latest version](https://taskernet.com/shares/?user=AS35m8m8L9YzBV3qbzaAAqHiSYXYBbD3QfZ7hr0hRK4ojOFTCrjWh2CScbjMw4NaudRi1zKKzq85&id=Project%3ASmart+Lists+%26+Reminders) from Taskernet or releases.
3. Run **SLR - Setup** again.

Tip

Import the [Updater](https://taskernet.com/shares/?user=AS35m8m8L9YzBV3qbzaAAqHiSYXYBbD3QfZ7hr0hRK4ojOFTCrjWh2CScbjMw4NaudRi1zKKzq85&id=Project%3AUpdater) project to get notified automatically when a new build is available.

## Uninstall

Delete the "Smart Lists & Reminders" project in Tasker. All task data lives in Tasker, so removing the project also removes your data — export first (**☰ menu → Import / export data**) if you want to keep it.

## Next Steps

- See [USER_GUIDE.md](USER_GUIDE.md) for quick-add syntax and features.
- See [FAQ.md](FAQ.md) if something isn't working.
