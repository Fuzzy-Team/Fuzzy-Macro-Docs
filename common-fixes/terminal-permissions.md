---
description: >-
  This could be the solution if the macro is failing to detect what is on
  screen.
---

# Terminal Permissions

{% hint style="info" %}
If you don't see Terminal in the list of apps, you can add it by clicking the "+" button under the list and selecting Terminal from Applications -> Utilities.
{% endhint %}

{% hint style="info" %}
If there's no "+" button, you might have to skip this for now. You can revisit this after you run the macro, as Terminal might show up.

Note that Automation doesn't have the "+" button — if you don't see Terminal in that category, add it after you run the macro.
{% endhint %}

Enable Terminal for these categories:

* Full Disk Access (lets macro access other macro files)
* Accessibility (lets macro send keypresses)
* Screen Recording (lets macro read the screen)
* Input Monitoring (lets macro detect keypresses)

If Terminal does not show up there, it should appear after running the macro.

{% hint style="warning" %}
NOTE: On older macOS versions, some of these categories may not show up, which is normal.
{% endhint %}

<details>

<summary>Sample for older macOS versions</summary>

![](<../.gitbook/assets/image (23)>)

</details>

<details>

<summary>Sample for newer macOS versions</summary>

![](<../.gitbook/assets/image (24)>)

</details>
