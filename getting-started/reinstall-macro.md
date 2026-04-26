---
description: >-
  This will keep your settings and patterns; this is mostly used to undo beta
  updates that were buggy.
---

# Reinstall macro (macOS)

{% hint style="danger" %}
Please note: this command will act like you are migrating from existance macro, even though this is not true please play pretend for me.
{% endhint %}

**This is just the same command as migrating from Existance Macro**

To do so, open Terminal and paste this command.

Command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/migrate_from_existance.command)"
```

{% hint style="warning" %}
**PLEASE make sure you select the folder of your old macro folder when prompted by Finder.**
{% endhint %}



## Reinstall old version

If you need to, for whatever reason, reinstall an old version, you can run this command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/update_from_commit.command)"
```

And then provide a commit ID/beta tester ID to roll back your macro to that version. You can get a tester ID from the Discord server.
