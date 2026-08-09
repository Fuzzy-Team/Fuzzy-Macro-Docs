# Stream setup

Fuzzy Macro can share a live view of your screen through a temporary link. The link is sent to Discord when the stream starts.

{% hint style="info" %}
Set up the [Discord bot](discord-bot-setup.md) first. Bot mode is the recommended way to receive the stream link and use `/stream` or `/streamurl` remotely.
{% endhint %}

## Install cloudflared

### macOS

If you do not already have Homebrew, install it from [brew.sh](https://brew.sh). Then open Terminal and run:

```bash
brew install cloudflared
```

### Windows

Open PowerShell or Command Prompt and run:

```powershell
winget install --id Cloudflare.cloudflared
```

If `winget` is not available, install it through the Microsoft Store’s **App Installer**, then run the command again.

## Enable the stream

1. In Fuzzy Macro, open **Config → Stream**.
2. Enable **Enable Stream**.
3. Start the macro. It creates the stream and posts its link to your configured Discord destination.
4. Open the link from a trusted device to view the live screen.

> ![](<../.gitbook/assets/image (12).png>)

With Discord Bot mode, you can also use `/stream enable`, `/stream disable`, `/stream status`, and `/streamurl`.

## Pinning the stream link

The **Pin Stream URL in Discord** setting requires **Use Both** delivery mode: a webhook posts the stream message and the bot pins it. Configure both the bot and webhook guides before enabling this option.

## Safety notes

Anyone with the stream link can view the shared screen. Keep it private, avoid sharing it publicly, and disable the stream when you no longer need it.

## Troubleshooting

* **The macro says cloudflared is not installed:** Install it using the command for your operating system, then fully close and reopen Fuzzy Macro.
* **No Discord link appears:** Confirm your bot or webhook delivery setup is working first, then check the macro’s Discord destination settings.
* **The link will not open:** Stop and restart the stream. Temporary links can expire after the stream stops.
