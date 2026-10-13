# Clubbox — VB-Cable integration

How to play Spotify / browser / DAW audio into a Clubhouse room **with your real microphone**, using [VB-Audio Virtual Cable](https://vb-audio.com/Cable/).

Also see: [USER_GUIDE.md](./USER_GUIDE.md) · [Releases](https://github.com/yusufsahin/clubbox-app/releases)

---

## What you need

1. Install **VB-Cable** from [vb-audio.com/Cable](https://vb-audio.com/Cable/) (free Virtual Cable is enough for Setup 1).
2. Restart Windows once after install so all apps see the new devices.
3. Clubbox **2.2.0+** ([download](https://github.com/yusufsahin/clubbox-app/releases/latest)).

If Device Manager lists **two** VB-Cable instances and one is broken, remove the broken one and keep the working `N-` copy (e.g. `2-`).

---

## Setup 1 — Clubbox mix (recommended)

| Role | Device |
| --- | --- |
| Clubbox **Microphone** | Your real mic (e.g. Realtek, USB mic) |
| Other apps **output** (Spotify, Chrome, …) | `Speakers (N- VB-Audio Virtual Cable)` or CABLE Input |
| Clubbox **External input** | `CABLE Output (N- VB-Audio Virtual Cable)` — **same N-** |
| Clubbox **Speakers** | Your headphones / real speakers — **not** the cable |

Effects:

- Clubbox mixes mic + external and can **duck** music under your voice.
- Muting the mic does **not** stop the music. Cut music with the cockpit **Music** button (or Live details › Mute external). Soundboard stays under Sounds › Stop.
- Local recording includes the mix.

### In Clubbox

1. Open **Music & external audio setup** (Settings › Audio, or from the hallway / room).
2. Choose **Setup 1 — Clubbox mix**.
3. Set Mic / External / Speakers as in the table → **Apply**.
4. In the room: Room details › Audio → quality **Music** for stereo music (use headphones).
5. Step 4 of the wizard: **Run VB-Cable check** (pass/fail + fixes). Result also appears under Live details › My audio.

Nothing is applied until you press **Apply**.

---

## Windows format (stereo / 48 kHz)

Most “no stereo” problems are Windows defaults.

1. Right‑click speaker icon → **Sounds** → **Recording** → **CABLE Output** → Properties → **Advanced**  
   → **2 channel, 48000 Hz** → Apply.
2. Same for **Playback** → **CABLE Input** / Speakers (N- VB-Cable).

Then reopen External in Clubbox (or re-run the VB-Cable check).

---

## VB-Cable check (in the app)

Wizard step 4 → **Run VB-Cable check**:

| Step | Meaning |
| --- | --- |
| Cable found | VB-Cable seen (warns if duplicate instances) |
| Signal | Tone into Speakers (N-) heard on CABLE Output (local only — **not** sent to the room) |
| Format | 2 ch / 48 kHz |
| Loop guard | Clubbox Speakers is not the same cable as External |
| Send path | External can reach the publish path (or was proven locally) |

Fix lines under each failed step tell you what to change.

---

## Setup 2 — Mixer as microphone (optional)

For Voicemeeter / Loopback / BlackHole:

- Clubbox **Microphone** = mixer output (e.g. VoiceMeeter Output).
- **External** = off.
- Clubbox **Speakers** = VoiceMeeter **Aux** Input (not the main VAIO that feeds B1).
- Mute mutes **everything**, because the mixer *is* the mic.

Room audio must never loop back into the mic bus.

---

## Common mistakes

| Mistake | Result |
| --- | --- |
| Mic and External both set to the same cable | Double signal / phasing — Clubbox blocks Apply |
| Clubbox Speakers = Speakers (N- VB-Cable) | Feedback loop; stage may stay blocked |
| Apps not playing into Speakers (N-) | No music in External / check fails on Signal |
| Quality left on Normal with loud music | Prefer **Music** + headphones |
| Trying to mute/invite others in Clubbox | App-only — use [Open on phone](./USER_GUIDE.md#moderation-important) |

---

## Quick link map

| Doc | |
| --- | --- |
| [USER_GUIDE.md](./USER_GUIDE.md) | Install, sign-in, rooms, moderation |
| [README.md](./README.md) | Short download + disclaimer |
| [Releases](https://github.com/yusufsahin/clubbox-app/releases) | Installers |
| [VB-Audio Cable](https://vb-audio.com/Cable/) | Driver download |
