# Clubbox — User guide

Unofficial desktop studio for Clubhouse. **Not affiliated with Clubhouse.** Personal, non-commercial use only.

| | |
| --- | --- |
| Download | [Releases](https://github.com/yusufsahin/clubbox-app/releases) |
| VB-Cable / music setup | [VB_CABLE.md](./VB_CABLE.md) |
| Current version | **2.2.0** |

---

## Install (Windows)

1. Open the [latest Release](https://github.com/yusufsahin/clubbox-app/releases/latest).
2. Download `Clubbox-*-setup.exe` (installer) or `Clubbox-*-portable.exe` (no install).
3. The build is **not code-signed**. If Windows SmartScreen or Smart App Control blocks it, use **More info → Run anyway**, allow the app in Windows Security, or run from the portable / unpacked build you trust.
4. Launch **Clubbox** from the Start Menu (or the portable exe).

macOS: a `.dmg` is not published here yet (build on a Mac from the private source repo).

---

## First run

1. Accept the first-run notice (unofficial / personal use).
2. Prefer **Sandbox** to explore the UI without a live Clubhouse session.
3. For live rooms: sign in when Clubbox opens the Clubhouse sign-in surface.  
   **Never** share tokens, cookies, SMS codes, or phone numbers.
4. After sign-in, use Explore / Hallway to find rooms, or start your own.

---

## Rooms

| Action | Where |
| --- | --- |
| Join a room | Hallway / Explore → open a room |
| Leave | Room controls → Leave (does **not** end the room for others) |
| Raise hand / join stage | Cockpit bar (when the room allows it) |
| Mute / quality / sounds | Cockpit + Room details › Audio |
| Live details | Click the room title in the bar |
| Chat / reactions | Cockpit (when chat is enabled) |
| Open on phone | Room header — link + QR for the Clubhouse phone app |

### Moderation (important)

Invite to speak, mute others, move to audience, make moderator, remove, and **end room** are **Clubhouse app only**. Clubbox shows those actions disabled with that message.

Use **Open on phone** (or the help card) and moderate from the official app.

---

## Audio (short)

- Recommended path for music + mic: **Setup 1 — Clubbox mix** with VB-Cable. Full steps: [VB_CABLE.md](./VB_CABLE.md).
- Open **Music & external audio setup** from Settings › Audio, the hallway, or the room. Nothing changes until **Apply**.
- Quality levels (Normal / High / Music) live in **Room details › Audio**. Use **Music** for external stereo music (headphones recommended — echo cancellation is off).
- Cockpit **send-quality** chip and Live details › My audio show bitrate / stereo while you are publishing.
- **Audio check** (local only): from Live details or the send-quality chip — 5s meters, nothing sent to the room.

---

## Sandbox vs live

| Mode | Purpose |
| --- | --- |
| Sandbox | Mock rooms and UI; no live Clubhouse traffic |
| Live | Your Clubhouse web session; real rooms and voice |

Switch carefully. Live mode needs a signed-in session.

---

## Privacy & safety

- Do not paste tokens, cookies, or SMS codes into chat or issues.
- Recording / clips are local opt-in features where available; respect room and Clubhouse rules.
- This app may conflict with Clubhouse Community Guidelines. You are responsible for how you use it.

---

## Help links

- [Download / Releases](https://github.com/yusufsahin/clubbox-app/releases)
- [VB-Cable integration](./VB_CABLE.md)
- [README](./README.md)
