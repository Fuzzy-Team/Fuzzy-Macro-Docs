---
description: Choose a planter mode, set when planters are harvested, and keep nectar up with Auto planters.
---

# Set up and maintain planters

Planters are set up on the **Planters** tab. Use the **Planter mode** slider to pick one of three modes:

* **Off**: the macro does not plant or harvest anything.
* **Manual**: you choose the planters and fields.
* **Auto**: the macro chooses planters and fields to keep your nectars up.

Planters only run in macro modes that include them (see [Macro modes and task order](macro-modes.md)).

## Settings in both modes

* **Harvest Every X Hours**: how often to collect planters. 2 to 3 is recommended.
* **Harvest When Full**: collect planters when they are fully grown. This overrides Harvest Every X Hours.
* **Collect Planter Loot**: collect the tokens a planter drops when harvested. Turn it off to harvest without sweeping up the loot.
* **Fast Planter Paths**: walk straight from one planter field to the next after placing a planter. Turn it off to reset and use the cannon to every field instead.
* **Planter check**: after looting, check your inventory to make sure the planter was collected.
* **Clear Planter Timers**: click **Reset** to clear the macro's tracking of your planters. Use it if the macro thinks a planter is still growing when it is not.
* **Selected Planters**: set the hotbar slot for each planter. Slot 0 uses inventory search instead.

## Manual planters

The macro places and collects up to 3 planters each cycle. Under **Planter Cycles**, pick a planter and field for each slot. Set a slot's field or planter to `none` to skip it.

## Auto planters

Auto mode decides what to plant based on your nectar targets.

* **Presets**: recommended nectar priority and field settings for **Blue**, **Red**, and **White** hives, or **Custom**.
* **Nectar Priority**: the macro keeps nectars above their minimum percentage. A nectar higher in the list has higher priority.
* **Nectars to Upkeep**: how many nectars from the top of the list get planters (1 to 5). Lower it if you cannot keep all five up.
* **Auto Harvest**: the macro decides when to harvest. This overrides Harvest Every X Hours.
* **Max Planters**: the most planters that can be out at once.
* **Gather in Planter Fields**: gathers in the planter's field right after placing it, so you collect while it grows.
* **Degradation Weight**: raise it to spread planters across more fields for more loot. It does not change how long planters grow.
* **Planters Allowed & Restrictions** and **Allowed Fields**: limit which planters and fields Auto can use.

### Wax and bonus loot drops

Two options plant the planter and field pairs that drop extra items when their cooldown is up. These go before the other planters and grow fully. They use the planters and fields you allowed.

* **Monthly Waxes**: Caustic and Swirled Wax.
* **Bonus Loot**: other loot such as Glue, Oil, Blue Extract and Neonberries.

If an option is greyed out with a hint, enable a planter that gives that drop under **Planters Allowed & Restrictions**. The **Wax from Planters** chart on the tab shows which planters drop which wax.

## Share your settings

**Export Settings** copies your planter setup to the clipboard. **Import Settings** opens a box where you paste it to load it.
