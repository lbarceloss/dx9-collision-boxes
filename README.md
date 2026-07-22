# PangYa Collision Boxes Viewer (DirectX9)

A lightweight DirectX 9 overlay for PangYa that renders collision boxes directly in-game.

This DLL is intended as a debugging tool to help map developers visualize collision boxes while testing newly created maps and verifying their in-game behavior.

> **Version:** 1.0 (Initial Release)

---

## Features

- DirectX 9 in-game overlay
- Collision box visualization
- Useful for map development and debugging
- Simple injection-based setup

---

## How to Use

1. Start PangYa.
2. Inject the DLL while the game is running.
3. Press **F10** to open the menu.
4. Enable the visualization options you want.
5. Place the `collboxes` folder inside your PangYa directory.
6. Make sure the folder is **extracted** (not inside a ZIP or RAR archive).

---

## Recommended Injector

Recommended:

- **Extreme Injector v3.7.3**

However, any DLL injector should work.

For best compatibility, keep the following files in the same directory:

- Injector
- This DLL
- Any additional DLLs included with the release

---

## Technical Notes

Although the current build uses a MinHook-compatible trampoline approach, it is **not** linked against the MinHook library.

The objective is to completely remove this dependency and replace it with a custom trampoline implementation written specifically for PangYa.

That implementation is still under development, but due to community requests, this first version is being released ahead of schedule.

The custom trampoline will be introduced in a future release.

---

## Known Issues

This is only **Version 1**, so there are still a few known issues.

### Map Detection

Sometimes the overlay fails to detect the currently loaded map.

### Workaround

Simply:

1. Close the current map.
2. Open it again.

Usually it starts working immediately after reloading the map.

---

## Planned for Version 2

- Better map detection
- General bug fixes
- Source code release
- Code cleanup and documentation

---

## Disclaimer

This project is intended **only** as a development/debugging utility for PangYa map creators.

Use it responsibly.
