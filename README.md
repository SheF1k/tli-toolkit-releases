# TLI Toolkit

An all-in-one companion app for **Torchlight: Infinite**: a farming tracker, two minigame advisors and a small
always-on-top card that shows the advice over the game.

**[Download the latest version](https://github.com/SheF1k/tli-toolkit-releases/releases/latest)** (Windows)

## What it does

- **Farming tracker.** Reads the game's log to track every map: what dropped, what opening the map cost, your profit
  and your **FE per hour**, valued with live community prices.
- **Vorax advisor.** Enter your Surgical Preparation board and it plays every option out thousands of times to tell you
  the best potion, target, instrument or refresh. Go for the 840k rainbow or for the best average score.
- **Tartarus Prison advisor.** Enter your board and get the best move for the day.
- **Advice card.** A small card that stays on top of the game and shows the current advice, so you don't have to
  alt-tab.

## Download

1. Open the [latest release](https://github.com/SheF1k/tli-toolkit-releases/releases/latest).
2. Download `TLI-Toolkit-<version>.exe` under **Assets**.
3. Run it. It's portable: there is nothing to install. To update, download the new version and use it instead of the
   old one.

Windows 10 or 11 (64-bit) only.

The app isn't code-signed, so Windows SmartScreen may say "Windows protected your PC" the first time. Click
**More info**, then **Run anyway**. Each release lists the exe's SHA-256, so you can check your download in PowerShell
with `Get-FileHash .\TLI-Toolkit-<version>.exe`.

## First steps

1. **Turn on the game's log:** in Torchlight: Infinite, press **Esc → Settings → Other** and, under **Account Related**, turn on **Enable Log**. The game
   switches it off every time it starts, so turn it on again after each launch.
2. **Relog** (back to character selection and in again), so the game writes your character and bag to the log.
3. **Sort your bag once**, so the tracker knows every stack you're carrying.
4. **Start TLI Toolkit.** It finds the log by itself. If it can't, pick the log file in the **Settings** tab. The
   **Log** light in the top-right corner turns green once the log is being read.

Now farm as usual: every map shows up in the **Tracker** tab. When you open Vorax or Tartarus Prison, the app switches
to that advisor; enter your board and follow the advice.

## FAQ

**Is it safe? Can I get banned?**
TLI Toolkit only reads the game's log file (which the game writes itself once you enable it); boards are entered by
you. It does not read or change the game's memory, inject anything into the game, or click and type for you: every move is still
yours. It is an unofficial tool, though, so use it at your own risk.

**Why is there no source code here?**
TLI Toolkit is closed source. This repository only hosts the downloads, the release notes and the bug reports.

**Where do the prices come from?**
Community prices from [tlicompanion.com](https://tlicompanion.com), plus the prices you look up on the in-game
exchange. You can set any price by hand, or switch the price feed off in Settings.

**Does it work on Mac, Linux or Steam Deck?**
No, Windows only.

## Credits

TLI Toolkit stands on the work of others:

- **Moebing's Vorax simulator** (MIT): the base rules of the Vorax simulation.
- **[glcoder/TartarusSolver](https://github.com/glcoder/TartarusSolver)** (MIT): the Tartarus Prison solver the
  advisor is built on.
- **[Syncingoutt/Fenix](https://github.com/Syncingoutt/Fenix)** (MIT): zone and item names.
- **[tidewarden/vorax-solver](https://github.com/tidewarden/vorax-solver)**: the reference for Vorax rules and odds.
- **[tlicompanion.com](https://tlicompanion.com)**: community prices.

TLI Toolkit is a fan-made tool. It is not affiliated with or endorsed by the makers of Torchlight: Infinite.

## Reporting bugs

Found a bug or have an idea? [Open an issue](https://github.com/SheF1k/tli-toolkit-releases/issues) and include:

- the version you're running (it's in the exe's file name),
- what you did, what you expected and what happened instead,
- a screenshot if it helps.

For tracker problems, the relevant part of the game's log helps a lot (the Settings tab shows where the file is).
Note that the log contains your character name.
