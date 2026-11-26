---
description: Set up a gather field, choose how the macro gets there and back, and know what each option does.
---

# Your first gather

Gathering is set up on the **Gather** tab. Each field has its own page; use **Add Field** to add more.

{% stepper %}
{% step %}
### Pick the field and turn it on

Choose the field in **Field**, then tick **Enable Task**. A field that is not enabled never runs.
{% endstep %}

{% step %}
### Pick a pattern

Under **Pattern**, choose a **Shape**, then adjust **Size** and **Width**. Size changes how much area the pattern covers. Width usually changes how many times each loop repeats. If you have your own patterns, use **Import Patterns** (see the [Pattern Creation Guide](../dev-docs/pattern-creation-guide.md)).
{% endstep %}

{% step %}
### Set when to stop

Under **Gather Until**, set **Mins** and **Backpack%**. Backpack% 95 is recommended instead of 100. **Infinite Gathering** ignores both limits and keeps gathering until something interrupts it.
{% endstep %}

{% step %}
### Choose how to return to the hive

**Return To Hive** can be Reset, Walk, Rejoin, or Whirligig. If you choose Walk, **Use Whirlwig Fallback** (spelled this way in the app) tries a whirligig when walking cannot find the hive, before it resets.
{% endstep %}

{% step %}
### Check the start location

**Start Location** picks which part of the field to gather in. **Distance** only matters when the start location is not Center.
{% endstep %}
{% endstepper %}

Check the sprinkler type and slot on the [Important settings](important-settings.md) page before you start.

## Getting to the field

By default the macro uses the cannon to reach a field. Two options under **Config → Bee Swarm** change how it travels:

* **Walk to Fields** walks from the hive to each field instead of using the cannon. It is slower, but it does not depend on finding the cannon. Mushroom always walks.
* **Faster Walk Home** uses shorter walks back to the hive from Clover, Coconut, Dandelion, Mountain Top, Mushroom, Pepper, Pine Tree (by glider), Rose, Spider, Strawberry, Stump and Sunflower. It was tested on Hive 3 only, so turn it off if the macro gets lost walking home from another hive.

## Optional extras

* **Use Goo** uses goo while gathering in this field. **Goo Interval (seconds)** sets how often (minimum 3).
* **Use Shift Lock** switches shift lock on while gathering.
* **Field Drift Compensation** moves the player back to the sprinkler (or the Supreme Saturator) between gather patterns.
* **Sprinkler Offset X / Y** moves where the sprinkler is placed. Leave these at 0 unless lag makes the sprinkler land off center.
