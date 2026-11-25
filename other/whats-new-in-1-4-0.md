---
description: A plain-words summary of what changed in Fuzzy Macro 1.4.0.
---

# What's new in 1.4.0

## Settings and look

* Settings are regrouped. Config now has Bee Swarm, Task Priorities, Rejoin & Recovery, App Settings, Discord, and User Profiles.
* Turn on **Top Navigation** (Config → App Settings → Appearance) to show the tabs in a bar across the top instead of the sidebar.
* New themes: Beesmas, and a Custom theme where you choose six colors yourself.
* Stream settings now live inside Config → Discord.
* The Home tab has two new macro modes: **Boost** and **Resources**.
* Pick the item for each hotbar slot, and set a sprinkler offset per field.
* Add a reorderable blender craft queue with up to 20 slots.
* Badge mode gathers fields until a badge is complete.

## Moving around

* **Walk to Fields** walks from the hive to each field instead of using the cannon.
* **Faster Walk Home** uses shorter walks back to the hive from many fields. It was tested on Hive 3 only.
* Planters can walk straight from one field to the next after placing a planter.
* An optional **1080p virtual display** keeps detection consistent on Retina screens (macOS 13 or later).

## Gathering and fights

* Stump Tap and Pine Tap.
* Mondo Chick: the macro can hop servers to find more Mondos, walks over before the hour, and fights by reading the health bar.
* AI Gathering can pick up Honey Storm tokens, and the token list has Select all and Select none.
* Moon Sprouts are planted at night.

## Planters

* Auto planters have a Degradation Weight and a Nectars to Upkeep setting.
* Monthly wax drops and bonus loot planters are planted before other planters.
* Planter placement and harvest are confirmed before they are recorded.

## Discord

* The bot only needs **Message Content Intent** now. Presence and Server Members intents can stay off.
* New commands: `/standby`, `/cooldowns`, `/performance`, `/ssa`, `/vicstats`, `/finditem`. The `/planters`, `/setmaxplanters`, and `/setplantermode` commands are gone; use `/plantertimers`, `/planterreset`, and `/collectplanter`.
* Notification routes have a Badges category.
* Stream and server links sent by commands are visible only to you.

## Reports

* Item reports count Battle Points, and stats track boss kills and disconnects.
* Buff Uptime shows Pine Tree, Bamboo, and Blue Flower boosts.
* The hourly honey graph and rate are more accurate.

## Safety and reliability

* The macro checks Accessibility and Screen Recording permissions when you start it.
* Imported profiles leave out your tokens and webhooks.
* The stream only listens on your own Mac, and the macro rejects requests from other websites.
* Many fixes make Pause and Stop work in more places, and release held keys when something is interrupted.

## Install and platform

* The installer uses the framework Python, installs libraries in one step, and stops if certificate setup fails.
* Fuzzy Macro 1.4.0 supports macOS. Windows support is still in development.
