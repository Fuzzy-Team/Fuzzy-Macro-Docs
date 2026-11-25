---
description: What each macro mode runs, and why an enabled task may be skipped.
---

# Macro modes and task order

## Changing the mode

Use the **Macro Mode** dropdown on the Home tab. You can also use the `/macromode` command in Discord (see [Discord Bot Setup](../discord-setup/discord-bot-setup.md)). The mode is saved in your profile.

## What each mode runs

| Mode          | What it does                                                                                                   |
| ------------- | -------------------------------------------------------------------------------------------------------------- |
| **Normal**    | Runs every enabled task in your task order: gathering, collecting, killing, planters, quests, and the rest.    |
| **Alt**       | For an account that follows a main account. It waits until it is sent a field, then gathers only that field. It ignores your task list. |
| **Field**     | Gathers only. It runs the enabled gather fields in your task order and skips everything else.                  |
| **Quest**     | Hands in finished quests, then works on quest objectives.                                                      |
| **Bug Run**   | Runs only kill tasks (mobs and bosses), Ant Challenge, and Stinger Hunt.                                       |
| **Boost**     | Runs only gather fields, Auto Field Boost, the blue, red and mountain boosters, and Guiding Star taps.         |
| **Resources** | Runs only kill and collect tasks, plus Ant Challenge, Stinger Hunt, and the Mondo Buff.                        |
| **Vic Hop**   | Runs the Vicious Bee hunt over and over.                                                                       |

## Task order

Your task order is under **Config → Task Priorities**. Drag tasks to change which one the macro tries first.

A task only runs when both of these are true:

* It is switched on in its own tab (for example, a gather field is enabled on the Gather tab, or a mob is enabled on the Kill tab).
* The current mode includes that kind of task.

If a task you enabled never runs, check the mode first. For example, a planter or a quest will not run in Field, Bug Run, Boost, or Resources mode, and a gather field will not run in Bug Run or Resources mode.

{% hint style="info" %}
In Bug Run mode only the tasks that appear in your task order run. A mob that is enabled but missing from Task Priorities is skipped.
{% endhint %}
