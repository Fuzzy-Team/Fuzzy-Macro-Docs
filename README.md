# How to Install

#### Fuzzy Macro already installed:

Press the update button in the macro, and it will detect a new version and auto-install it

#### Moving from Existance Macro/Fresh Install

**Moving from Existance Macro:**

1. Download this file: [https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/migrate\_from\_existance.command](https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/migrate_from_existance.command) (Visit link, right click, choose save as, then rename the file to `migrate_from_existance.command` this is to remove the .txt ending.)
2. Move this new file into the folder of your macro
3. Then open it by double-clicking
4. Follow the migration assistant, and all of your data from Existance will now be migrated to Fuzzy Macro. You will use the same folder, but to start the macro, you instead open a file called "run\_macro.command".

{% hint style="info" %}
**Note: When migrating, it currently does not add any of the new Fuzzy patterns**
{% endhint %}

**Fresh Install:**

To do so, open Terminal and paste this command:

Command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/fuzzy_installer.command)"
```

{% hint style="info" %}
After running the installer, go through the rest of the pages; all pages before the Discord setup section are mandatory. **The rest of the pages do not need to be done if you have used Existance Macro previously.**
{% endhint %}
