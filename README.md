<div align="center">

# ☀ SOLSTICE

### feed the light · hold back the night

**A juicy 20-level arcade game for the [June Solstice Game Jam](https://dev.to/devteam) — and an ode to Alan Turing.**

*The longest day of the year, and the dark wants it back. Glide your light, gather the sun's motes,*
*grab power-ups, survive the Solstice Turn, and break two beasts of night.*

[**▶ Play it live**](https://stackmasteraliza.github.io/solstice-cipher/) · [**🎬 Watch the demo**](https://youtu.be/n6lRqo1CBSo) · [Power-ups](#-power-ups) · [How it's built](#-built-with)

</div>

---

## ✨ Why it's fun

You **are** a spark of light. Move with the mouse (or your finger) and the whole screen responds —
the sky shifts from blazing noon to deep night, the sun rises and sets with your daylight, particles
burst, combos chime, and the music speeds up as the danger climbs.

- 🌗 **The light is the game.** Daylight is your health bar. Gather motes to keep it burning; touch a
  shadow and the night creeps in. Let it hit zero and the screen pulses red as night falls.
- 🌀 **The Solstice Turn.** At the midpoint the world flips — the longest *day* becomes the longest
  *night*, the sky goes cold, the sun becomes a moon, and light becomes precious.
- ⚙ **An ode to Alan Turing.** Born in June, the man who broke the Enigma. Each boss ends not with a
  hit but with **"Decode the Dawn"** — repeat the cipher, Bombe-style, to break the night for good.
- 🌑 **Two bosses.** *The Longest Night* at day 10, and the bigger, faster, bullet-spitting
  **Eclipse King** at day 20 — each with a phase-2 rage mode.

## ☄ Power-ups

Pick them up mid-run for a clutch advantage:

| | Power | Effect |
|---|-------|--------|
| ⏳ | **Time Warp** | Slows every shadow to a crawl |
| 🧲 | **Light Magnet** | Vacuums all motes toward you |
| ❄ | **Freeze** | Freezes shadows solid for a few seconds |
| ☀ | **Sun Fragment** | Instantly refills your daylight |

…plus the **Sun Nova** ☀ — charge it by collecting motes, **stockpile up to 3**, and unleash it
(Space / Click) to wipe every shadow, shield yourself, and blast the boss.

## 🎮 How to play

- **Move** — mouse or finger guides your light
- **Collect** glowing **sun motes** — light + score, and they build your **combo multiplier**
- **Avoid shadows** — normal, fast *darters*, big *tanks*, and *splitters* that break in two
- **Space / Click** — fire a stocked **Nova**
- Clear each day's **task** (collect / score / survive / combo) to advance
- A **guided practice** teaches the controls on first run, and a **boss briefing** preps you before each beast
- Beat all 20 days to reach **DAWN** — then take on **♾ Endless mode**

Difficulty: **Easy / Normal / Hard** — pick your fight.

## ▶ Run it

No build step, no dependencies — it's a single `index.html`.

```bash
# clone, then just open it
open index.html        # macOS
start index.html       # Windows
# …or serve the folder
python -m http.server 8000   # then visit http://localhost:8000
```

## 🛠 Built with

Plain **HTML5 Canvas + vanilla JavaScript**, no frameworks, no assets, no build.

- The entire sky, sun, glow and star field are driven by **one CSS/JS variable** (`--night`).
- All audio is **synthesized live with the Web Audio API** — kick/hat/bass beat tracks that speed up
  per level, a **furious minor-key boss track**, win/lose stingers, and SFX. No audio files.
- Honest **Mastermind-style** cipher scoring with correct duplicate handling for the Turing finisher.
- Fully keyboard- and touch-playable; colour + shape pairing for accessibility.

## 📜 Story

> *Every long day bends toward the dark. Alan Turing taught machines to reason in light and shadow —
> ones and zeros — and broke the cipher that turned a war's longest nights toward dawn. He was
> persecuted for who he loved, and never granted his own daylight. Here, you carry the light he
> couldn't keep. Break the night, and let the morning win.* ☀ 🏳️‍🌈

## 📄 License

MIT — see [LICENSE](LICENSE). Built during the June Solstice Game Jam (June 3–21, 2026).
