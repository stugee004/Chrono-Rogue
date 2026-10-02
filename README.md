# Chrono Rogue: Rise of Humanity

A turn-based roguelike that runs in the browser. Fight through nine eras of
human history, from the Stone Age to the Information Age, then reach the Chrono Age
and activate the Time Machine. Winning sends you back to 2,500,000 BCE to do it
all again, with the echoes of your last run to spend and a harder world waiting.

## How it works

- Each era is one floor with a guardian. Beat it to open the portal.
- Gear and levels carry between eras. Every era drops a new weapon and armor tier.
- Press Q for the era's invention (an area blast, 18-turn recharge). Press E to use a remedy.
- Dying restarts you in the Stone Age. Echoes you earned stay with you and buy permanent upgrades.
- Winning raises the loop count: enemies get tougher each time history repeats.

## Controls

| Action | Keys |
| --- | --- |
| Move | Arrows, WASD, vi-keys (hjklyubn), numpad |
| Wait | `.`, Space, or `5` |
| Era invention | `Q` |
| Use remedy | `E` |

Touch devices get an on-screen pad.

## Hacking on it

- Eras, enemies, and gear names live in the `ERAS` array. Add an object to add an era;
  the last entry is treated as the finale.
- Permanent upgrades are in `UPS`.
- Difficulty scaling is in `mkMon()`.
- Progress is stored in `localStorage` under `chrono-rogue-v1`.
