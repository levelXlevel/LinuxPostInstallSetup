# Latte

It's very nice, but not my taste. I do like the general setup so I will borrow from it and mimic it using Plasma native panels.

# Before you start

- You will lose the use of the META key used to launch the application launcher. There's fix for this described at the end.
- Quit Latte
  - This is to keep Latte out of the way while the new layout is being setup.
  - In the event you're not happy with the setup, you will have something to work with until you sort things out or get rid of the native panels.
  - Be prepared for a mess of a UI if you've setup some new panels as Latte may overlap them when it loads.

# Setup

- Add a default panel to the bottom.
- Add an empty panel to the top.

## Default panel

- Configure to your liking
- My personal choices
  - Dashboard launcher
  - Virtual Desktop pager
  - Icons only task manager
  - Peek at desktop

## Empty panel

- Configure to your liking
- My personal choices
  - Window Title
  - Spacer
  - Thermal monitor
  - System Monitor: Network Speed
  - Network Speed widget
  - Media Player
  - System Tray
  - Event Calendar

# Finalize & Clean Up

- Uninstall Latte
- Restore use of `meta` key to trigger application launcher.
- Restore window titlebars

## Uninstall Latte

- Use you preferred package manager and remove Latte

## Restore META key

- Back up the file `~/.config/kglobalshortcutsrc`.
- Use your preferred editor and modify the file.

Before:

```
Meta=org.kde.lattedock,/Latte,org.kde.LatteDock,activateLauncherMenu
```

After:

```
# Meta=org.kde.lattedock,/Latte,org.kde.LatteDock,activateLauncherMenu
```

N.B. The line **will** get removed from the file on next reboot.

## Restore window title bars

- Back up the file `~/.config/kwinrc`.
- Use your preferred editor and modify the file.

Before:

```
BorderlessMaximizedWindows=true
```

After:

```
BorderlessMaximizedWindows=false
```
