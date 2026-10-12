# Clubbox

Unofficial desktop studio for Clubhouse. **Not affiliated with Clubhouse.** Personal, non-commercial use only — use at your own risk.

## Local build output

On this machine, `npm run dist` in the private source repo writes installers to:

`C:\Projects\clubdeck-app\release\`

That folder is gitignored. Public downloads still go through GitHub Releases.

## Download (Windows)

Installers are on the [Releases](https://github.com/yusufsahin/clubbox-app/releases) page (not in this git tree — files are too large for git).

| File | Use |
| --- | --- |
| `Clubbox-*-setup.exe` | Installer (choose folder, Start Menu shortcut) |
| `Clubbox-*-portable.exe` | No install — run directly |

Current version: **2.2.0**

## Install

1. Open the latest [Release](https://github.com/yusufsahin/clubbox-app/releases/latest).
2. Download `Clubbox-2.2.0-setup.exe` (or the portable build).
3. Run it. The build is **not code-signed**. If Windows SmartScreen or Smart App Control blocks it, use **More info → Run anyway**, or run the portable build / allow the app in Windows Security (personal use of a build you trust).
4. Launch **Clubbox** from the Start Menu (or run the portable exe).

## First run

1. Accept the first-run notice (unofficial / personal use).
2. Prefer **Sandbox** to explore the UI without a live session.
3. For live rooms: sign in with your Clubhouse web session when the app asks — do not share tokens, cookies, or phone codes.
4. Host moderation (mute, invite, end room, …) is **Clubhouse app only** — use **Open on phone** in the room header when you need to moderate.

## macOS

A macOS `.dmg` is not published here yet. It must be built on a Mac (`npm run dist` in the private source repo).

## Support / source

This repository distributes **binaries and usage notes only**. Source code is not published here.

## Disclaimer

Not affiliated with Clubhouse or Alpha Exploration Co. May conflict with Clubhouse Community Guidelines. You are responsible for how you use it.
