# FAQ

**Nothing happens when I type `@slr`.**
This relies on Tasker's **Accessibility Monitor**, so make sure it's turned on in Android Settings (Settings → Accessibility → Tasker). Also confirm the **SLR - commandReceiver** and **SLR - monitorStart** profiles are enabled, and that Tasker isn't battery-restricted — check [dontkillmyapp.com](https://dontkillmyapp.com) for your device brand.

**My widget/notification looks stale after adding a task elsewhere.**
Run the **SLR - maintainance** task, or reopen the widget — data syncs from the same shared Tasker variable.

**Can I drive SLR from my own Tasker tasks?**
Yes — see the **SLR - commandReceiver** profile and the `SLR=:=action,params` command format in [USER_GUIDE.md](USER_GUIDE.md#automation-command-receiver) for available actions (`add`, `edit`, `toggle`, `select_view`, etc.).

**Updating erased my tasks.**
This is expected — Tasker projects don't diff cleanly, so updates require a full delete + fresh import (see [SETUP.md](SETUP.md#updating)). Export your data first via **☰ → Import / export data** if you want to carry it over, then load it back in after updating.

**Where is my data stored?**
Entirely on-device, in a single Tasker global variable (`tasks_data`). Nothing is sent off your device. See [Privacy](README.md#privacy).

**How do I back up my tasks?**
**☰ → Import / export data**, then copy the JSON somewhere safe. Use **Load** in the same dialog to restore it.

**Something else is broken.**
[Open an issue](https://github.com/WhirlWolf/Smart-Lists-Reminders/issues) with what you tried, what happened, and your Tasker version.

See also: [TIPS.md](TIPS.md) for lesser-known shortcuts that might already solve what you're running into.
