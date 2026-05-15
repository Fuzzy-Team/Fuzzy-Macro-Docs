---
description: Please note that this comparison is constantly updating.
---

# Fuzzy Macro vs Existance Macro

## Fuzzy Macro vs Existance Macro

| Area                    | Existance Macro                                     | Fuzzy Macro                                                              |
| ----------------------- | --------------------------------------------------- | ------------------------------------------------------------------------ |
| Operating systems       | macOS only                                          | macOS + Windows support work/beta support                                |
| Quest support           | Basic                                               | Brown Bear, Black Bear, Petal quests, expanded quest handling            |
| Boss support            | No bosses                                           | King Beetle + Tunnel Bear support                                        |
| AI support              | None                                                | AI Gather + AI sprinkler detection                                       |
| Gather logic            | Traditional patterns                                | Many patterns and AI token chasing + customizable token priorities       |
| Theme system            | None                                                | Multiple bee based themes                                                |
| Update channels         | Manual                                              | Stable + Beta channels + commit-hash updates                             |
| Update UI               | Basic                                               | Visible update progress + frontend update detection                      |
| Auto planter system     | Basic planter logic/unreliable                      | Auto Planters V2 with degradation tracking                               |
| Import/export systems   | None                                                | You can import/export Gather settings, planter settings, pattern imports |
| Scheduler systems       | Simple scheduled rejoins                            | Advanced scheduled rejoins + timed macro stop                            |
| Recovery systems        | Basic                                               | Inactive Honey Reset + whirligig fallback                                |
| Discord bot commands    | Limited                                             | Expanded slash command ecosystem                                         |
| Rich presence           | None                                                | Discord Rich Presence support                                            |
| Hotbar systems          | Minimal                                             | Hotbar Buff tool + redesigned hotbar UI                                  |
| Task management         | Simple task flow                                    | Priority queue + drag-and-drop ordering                                  |
| Debug tooling           | Minimal                                             | Debug export tools + richer diagnostics                                  |
| Installation system     | Older/manual flow                                   | Simplified installer + migration scripts                                 |
| Error reporting         | Basic                                               | Crash diagnostics + signal logging                                       |
| Scaling support         | Basic (Doesn't work on a lot of screen resolutions) | Reworked resolution/scaling handling                                     |
| Pattern systems         | Standard field patterns                             | Hive Hub Support + many new patterns + **AI gather**                     |
| Memory Match support    | Basic                                               | Rewritten logic with smarter tile tracking                               |
| AFB handling            | Broken                                              | Reworked AFB logic                                                       |
| Private server handling | Basic                                               | Share links + hive exclusion slots                                       |
| Tools                   | None                                                | Bond calculator, Ticket calculator, Auto Clicker                         |
| Blender support         | 3 slots                                             | 5-slot blender system                                                    |
| Anti-stuck systems      | Minimal                                             | Max convert timers + retry systems                                       |
| Logging systems         | Basic                                               | Better diagnostics + quieter logging                                     |
| Beta infrastructure     | None                                                | Dedicated beta update/testing system                                     |
| Ongoing development     | Discontinued                                        | Active development                                                       |

| Metric                 | Existance Macro | Fuzzy Macro |
| ---------------------- | --------------- | ----------- |
| Total files            | 568             | 627         |
| Python files           | 145             | 187         |
| Total lines            | 21,846          | 49,256      |
| Python source lines    | 10,531          | 25,451      |
| Pattern files          | 9               | 23          |
| Path files             | 104             | 107         |
| Boss path files        | 0               | 2           |
| Quest path files       | 6               | 8           |
| Discord slash commands | 9               | 46          |

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

Updated as of Fuzzy Macro version 1.2.0.
