---
description: Please note that this comparison is not yet done.
---

# Fuzzy Macro vs Existance Macro

## Fuzzy Macro vs Existance Macro

| Area                         | Existance Macro                                                    | Fuzzy Macro                                                                                                                                                                               |
| ---------------------------- | ------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Project status / direction   | Original macOS Bee Swarm macro baseline                            | Continuation project built on Existance; actively maintained with added systems/modules                                                                                                   |
| Platform                     | macOS only                                                         | macOS and Windows                                                                                                                                                                         |
| Core macro functionality     | Field gathering, mob killing, collecting items, converting         | Same core functionality, plus more automation modules                                                                                                                                     |
| Language / architecture      | Python backend + HTML/CSS/JS GUI                                   | Same general architecture; expanded feature set and GUI tooling                                                                                                                           |
| Patterns / paths             | Uses pattern files for field gathering + path files for navigation | Same pattern/path approach; more patterns/behavior supported                                                                                                                              |
| Settings compatibility       | Baseline settings structure                                        | Designed to feel familiar; “transition is easy” (settings/config idea remains similar)                                                                                                    |
| Private server support       | Yes                                                                | Yes                                                                                                                                                                                       |
| Discord webhooks             | Yes                                                                | Yes, plus more granular ping categories and more event coverage                                                                                                                           |
| Discord remote control       | Limited / not a focus                                              | Major feature: remote control via Discord bot commands; more command surface and status views                                                                                             |
| Discord commands (examples)  | N/A / fewer                                                        | More commands and remote actions (examples you listed: `/start`, `/stop`, `/pause`, `/resume`, `/screenshot`, `/fields`, `/quests`, `/mobs`, `/collectibles`, `/swapfield`, `/taskqueue`) |
| Collectibles & tasks         | Core set                                                           | Same core set + improvements on pathing and new honeystorm collection                                                                                                                     |
| Task scheduling / priority   | None                                                               | Task Priority System with drag-and-drop task ordering                                                                                                                                     |
| Profiles                     | Single main config                                                 | Profile System for multiple configurations                                                                                                                                                |
| Pause/Resume                 | Stop/start focused                                                 | Pause/Resume added as well as Start/Stop                                                                                                                                                  |
| Reliability / error handling | Baseline                                                           | Better error handling, improved recovery, clearer messages                                                                                                                                |
| Update system                | Manual / less streamlined                                          | Custom update script that isn't confusing                                                                                                                                                 |
| Performance                  | Baseline                                                           | Optimization work (slightly reduced resource usage)                                                                                                                                       |
| GUI themes                   | Single look                                                        | GUI Theme Switcher                                                                                                                                                                        |
| Anti-stuck safety            | Baseline                                                           | Max Convert Timer to prevent getting stuck converting (ex: balloon at 0)                                                                                                                  |
| Mobs / stinger hunt          | Regular mobs + Vicious Bee stinger hunt at night                   | Same mobs + stinger hunt;                                                                                                                                                                 |
| Credits / lineage            | Created by Existance                                               | Built on Existance’s original code; developed by Logan (LaganYT) with additional contributors                                                                                             |

### Credits

#### Macro Inspiration:

* [Natro Macro](https://github.com/NatroTeam/NatroMacro)
* [Stumpy Macro](https://github.com/alaninnovates/bss-macro)
* [Existance Macro](https://github.com/existancepy/bss-macro-py)
* Developers: [Logan](https://github.com/LaganYT)
  * Based off code written by: [Existance](https://github.com/existancepy/bss-macro-py)
* Pattern Makers: Existance, NatroTeam, tvojamamkajenic, sev, dully176, chillketchup, Electro

### Notes

* This Macro is for MacOS only. Linux and Windows support are not planned, for Windows use [Natro Macro](https://github.com/NatroTeam/NatroMacro), for Linux use [BeeTuxMacro](https://github.com/painvision/BeeTuxMacro).
* Fuzzy Macro is built on top of Existance Macro, meaning you can easily transitition to Fuzzy Macro. The settings and config works the same, think of Fuzzy Macro as a continuation project of Existance Macro.
* The macro backend is written in Python while the frontend uses HTML/CSS/JS with eel as a communication layer.
* Version system uses the format Major.Minor.Bugfix, with an optional letter at the end for test versions. (Ex: 1.1.0 is newer than 1.1.0a - 1.1.0a is a beta version in this case)
