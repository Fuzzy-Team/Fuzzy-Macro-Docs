---
description: What to send when you ask for help, and what the macro does when Roblox will not let it back in.
---

# Troubleshooting and getting support

## Export a debug folder

When you ask for help, send a debug folder. It saves the back-and-forth of asking for each piece separately.

1. Open the **Config** tab.
2. Find **Export Debug**.
3. Click **Export Debug Folder**. A zip file downloads.
4. Send the zip in the support channel.

The zip holds:

* your exported profile
* the recent log lines
* system info: macOS version, chip (Apple silicon or Intel), Python version, and macro version

Webhook links, Discord bot token, and private server links are blanked in the exported profile, so the zip is safe to share.

If the macro crashed, also click **Open Log Folder** in the same section and send `errors.log`. It records the crash with its stack trace.

## Rejoining and join errors

When the macro disconnects or has to rejoin, it works through your servers in order:

1. Your private server link, with up to **Rejoin Attempts Per Private Server** tries (default 5).
2. Each backup server, with the same number of tries. Set up to three under **Fallback Private Servers** (click **Manage Servers**).
3. A public server, if every private link fails.

All of these settings are under **Config → Rejoin & Recovery → Joining**. Raise **Rejoin Attempts Per Private Server** if your connection can stay down for a while.

If Roblox shows a join error, the macro reads the error code and reacts:

| Code | What it means | What the macro does |
| ---- | ------------- | ------------------- |
| 279 | Connection failure | Retries |
| 256 | Server data failure, or an active ban | Retries |
| 524 | Permission denied | Skips that link and tries the next server |
| 429 | Too many requests | Waits 30 seconds, then retries |
| 267 | Roblox shows this when you are kicked or the server restarts, during some Bee Swarm updates, and for bans | Stops the macro. Check that you can join the game yourself, then start the macro again |

If the macro reports that you are not logged in, open the Roblox app, sign in, and start the macro again. Rejoining uses the Roblox app, so it needs a signed-in account.

If you are rejoining over and over with a bad private server link, the macro logs `Invalid private server link; trying the next server`. Check the link under **Private Server Link** (see [Private Server Link](../macro-settings/private-server-link.md)).

## Importing a profile

Imported profiles never include webhook links, the Discord bot token, notification route URLs, or private server links. After you import one, set those again:

* private server link: **Config → Rejoin & Recovery → Joining**
* webhook and routes: [Discord Webhook Setup](../discord-setup/discord-webhook-setup.md)
* bot token: [Discord Bot Setup](../discord-setup/discord-bot-setup.md)

## Permission problems

If the macro will not start, or clicks and keys do nothing, see [Terminal Permissions (macOS)](terminal-permissions.md).
