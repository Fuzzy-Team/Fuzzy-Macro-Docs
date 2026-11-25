---
description: The tools on the Tools tab, what each one does, and how to start and stop them.
---

# Standalone tools

The **Tools** tab holds small tools that run on their own. Stop the main macro before you use one. Every tool stops with the macro stop keybind (F3 by default).

Keybinds for starting tools are under **Config → Keybinds → Tool Keybinds**: **Start Hotbar Buff Keybind**, **Start Auto Clicker Keybind**, and **Start Auto Gifted Basic Bee Keybind**. Click a box and press the keys you want. Backspace or Delete clears it while recording.

## Auto Clicker

Left-clicks over and over.

* **Click Interval (ms)**: time between clicks. Lower is faster.
* **Start Delay (seconds)**: wait before clicking begins. Default is 3.
* Use **Start Auto Clicker** and **Stop Auto Clicker**, or the keybinds.

## Hotbar Buff

Presses hotbar slots on a timer while you play. For each slot from 1 to 7:

* **Enabled** lets the tool press that slot.
* **Use Every** sets how often, in seconds or minutes.

Click **Start**, or press the start keybind (F4 by default).

## Bond Calculator and Ticket Price Calculator

These only calculate. They do not control the game, so you can use them any time.

## Auto Gifted Basic Bee (BETA)

Rolls a Basic Bee until it becomes gifted. Press Start (or the keybind), and the tool waits for a short countdown, records where your mouse is as the bee slot, then alternates Basic Egg, Royal Jelly, Basic Egg until it finds a Gifted Basic Bee or a result you asked it to pause on.

* **Capture Delay (seconds)**: the countdown before it records your mouse position (1 to 10, default 3). Put the mouse over the bee slot before it ends.
* **Pause On Result**: also stop on **Gifted Non-Basic**, **Legendary**, or **Mythic**. Gifted Non-Basic and Mythic are on by default.

Keep Auto-Jelly off in Bee Swarm and keep Roblox visible. The tool reads each roll with OCR, so it can misread, especially at low resolution. Watch it run.

## SSA Roller (BETA)

Rolls the Supreme Star Amulet generator until a roll matches what you want, then stops with the result open so you can choose Keep or Replace in the game.

1. Stand at the generator with its E prompt showing, or leave an SSA result open.
2. Choose the **Main Passive**. Tick **Double Passive** if you roll with two (500b per roll) and pick the side passives.
3. Add up to five stats. Leave **Min %** blank to accept any value.
4. Set **Honey Limit** in trillions (0 means no limit). It counts only what this tool spends.
5. Click **Start**.

Three options change how it behaves:

* **Wait for Discord command** shows what it sees, then waits for `/ssa go` before it clicks anything. This is on by default.
* **Manual review** sends each match to Discord so you can approve (stop) or deny (keep rolling). You can also use `/ssa approve` and `/ssa deny`.
* **Safety** stops the tool if it cannot read a full roll in time.

The tool reads each roll with OCR, so watch the first few rolls.
