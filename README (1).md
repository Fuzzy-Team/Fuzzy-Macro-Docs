---
description: This is how to install the macro on macOS or Windows.
---

# How to Install

{% hint style="danger" %}
Guide for migrating from Existance macro (macOS) has been moved to here: [https://fuzzy-team.gitbook.io/fuzzy-macro/getting-started/migrating-from-existance-macro](https://fuzzy-team.gitbook.io/fuzzy-macro/getting-started/migrating-from-existance-macro)
{% endhint %}

## **Installing on macOS:**

To do so, open Terminal and paste this command.

Command:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/fuzzy_installer.command)"
```

## Installing on Windows (beta):

Open up PowerShell (as Administrator) and paste this command:

```ps1
& ([ScriptBlock]::Create((irm "https://raw.githubusercontent.com/Fuzzy-Team/macro-auto-install/refs/heads/main/windows/installmacrob.ps1")))
```

{% hint style="warning" %}
Windows is not yet 100% working or supported. More info here: [https://discord.gg/c4XM7XJjrP](https://discord.gg/c4XM7XJjrP)
{% endhint %}

{% hint style="success" %}
After running the installer, go through the remaining pages; all pages before the Discord setup section are mandatory. **The rest of the pages do not need to be done if you have used Existance Macro previously.**
{% endhint %}

