---
title: "SOLSTICE — feed the light, hold back the night (an ode to Alan Turing)"
published: false
tags: devchallenge, gamechallenge, gamedev, javascript
cover_image:
---

*This is a submission for the [June Solstice Game Jam](https://dev.to/challenges/june-game-jam-2026-06-03)*

## What I Built

**SOLSTICE** is a juicy, single-file browser arcade game about the longest day of the year — and a tribute to **Alan Turing**, born in June, the man who turned the longest nights of a war toward dawn.

You **are** a spark of light. Move with your mouse (or finger) and the whole world responds: the sky shifts from blazing noon to deep night, the sun rises and sets with your daylight, particles burst and the music speeds up as the danger climbs.

- 🌗 **Daylight is your health.** Gather the sun's **motes** to keep it burning; touch a **shadow** and the night creeps in. Let it hit zero and the screen pulses red as night falls.
- 🌀 **The Solstice Turn.** At the midpoint the world flips — the longest *day* becomes the longest *night* (exactly the prompt's "longest day for half the world, shortest for the other"). The sky goes cold, the sun becomes a moon, and light becomes precious.
- 🌑 **Two bosses.** *The Longest Night* at day 10, and the bigger, faster, bullet-spitting **Eclipse King** at day 20 — each with a phase-2 rage mode and a **codebreaking finisher**.
- ☄ **Power-ups & a stockpile-able Nova.** Time Warp, Light Magnet, Freeze, Sun Fragment — plus the Sun Nova you can bank ×3 and unleash to wipe the screen.

It connects to the theme on every axis: **the solstice** (longest day, the Turn), **light vs. dark** as the core mechanic, and **Alan Turing** woven into the story and the boss fights.

**▶ Play it live:** https://stackmasteraliza.github.io/solstice-cipher/

{% embed https://stackmasteraliza.github.io/solstice-cipher/ %}

## Video Demo

{% embed https://youtu.be/n6lRqo1CBSo %}

▶ Watch the demo: https://youtu.be/n6lRqo1CBSo

## Code

The whole game is one `index.html` — no build step, no dependencies, no external assets.

{% embed https://github.com/stackmasteraliza/solstice-cipher %}

## How I Built It

Plain **HTML5 Canvas + vanilla JavaScript**. A few decisions I'm happy with:

- **One variable drives the whole atmosphere.** The sky, the sun's arc, the glow and the star field are all tied to a single value (`--night`, 0 = blazing noon → 1 = full dark). The game loop just sets it from your remaining daylight and everything follows — the sun literally sinks as you run out of light.
- **All audio is synthesized live with the Web Audio API** — no sound files. There's a kick/hi-hat/bass **beat track that speeds up every level**, a separate **furious minor-key boss track**, win/lose stingers, and reactive SFX whose pitch rises with your combo.
- **20 levels, two bosses, a power-up economy, and four enemy types** (normal, fast *darters*, heavy *tanks*, and *splitters* that break in two) — all from a compact entity loop.
- **Honest Mastermind scoring** for the Turing finisher, with correct duplicate-glyph handling (the classic trap), unit-tested against the tricky cases.
- **Onboarding built in:** a guided **practice with tooltips** the first run, and a **boss briefing** before each beast, so a new player (or a judge) is taught every mechanic right before they need it.
- **Accessible & portable:** fully keyboard + touch playable; colour *and* shape pairing for enemies; runs from a single file anywhere.

## Prize Category

**🎯 Best Ode to Alan Turing.**

June is Turing's birth month, so the game is built around the thing he's famous for — **code-breaking and the triumph of logic over darkness**:

- **Mechanic:** each boss can't just be hit to death. At zero HP it's *exposed*, and **Turing's Bombe** reveals a cipher — you **"Decode the Dawn"** by repeating the sequence to break the night for good. Code-breaking *is* the finishing move.
- **Narrative:** between-level "transmissions" trace his arc — Bletchley, the Enigma, his persecution for who he loved, "never granted his own daylight." The win screen, **DAWN**, is a tribute: *"For Alan Turing (1912–1954) — who broke the world's hardest cipher and was never allowed his own daylight."*
- **Design:** the Enigma rotor motif and the light-vs-shadow (1s and 0s) framing run throughout.

*Not submitting to Best Google AI Usage — no Google AI is used in this build.*

<!-- Solo submission. -->

Thanks for running the jam — happy solstice! ☀
