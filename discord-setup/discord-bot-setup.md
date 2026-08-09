# Discord Bot Setup

{% hint style="success" %}
**Recommended for almost everyone.** The Discord bot can send all macro notifications to a normal Discord channel *and* gives you remote slash commands. Use a webhook only when you only want one-way notifications.
{% endhint %}

## Before you start

You need a Discord server where you have permission to add a bot and create or manage channels. A small private server is the simplest and safest choice.

{% hint style="warning" %}
Your bot token is a password. Never share it, post it in screenshots, or put it in a support message. If it is exposed, reset it immediately in the Discord Developer Portal and update the macro with the new token.
{% endhint %}

## Create and invite the bot

{% stepper %}
{% step %}
### Create an application

Open the [Discord Developer Portal](https://discord.com/developers/applications), select **New Application**, give it a name, accept Discord’s terms, and create it.

> Screenshot placeholder: New Application screen
{% endstep %}

{% step %}
### Add a bot user

In the new application, select **Bot** in the sidebar, then choose **Add Bot** if Discord shows that option.

Under **Privileged Gateway Intents**, enable all three toggles—**Presence Intent**, **Server Members Intent**, and **Message Content Intent**—then save your changes. Fuzzy Macro currently starts its Discord bot with Discord’s full intent set, so leaving a privileged intent disabled can prevent the bot from connecting.

> Screenshot placeholder: Bot settings screen
{% endstep %}

{% step %}
### Generate an install link

Open **Installation** in the Developer Portal. Under **Guild Install**, add these scopes:

* `bot`
* `applications.commands`

For bot permissions, grant the minimum needed for the channel you will use:

* View Channels
* Send Messages
* Embed Links
* Attach Files
* Read Message History

If you plan to enable **Pin Stream URL in Discord**, also grant **Manage Messages** so the bot can replace the old pinned stream link.

Copy the generated install link, open it, select your server, and authorize the bot.

> Screenshot placeholder: Guild Install scopes and permissions
{% endstep %}

{% step %}
### Create or choose a macro channel

Create a private channel such as `#fuzzy-macro`, or choose an existing channel. The bot needs access to it.

Enable Discord **Developer Mode** (User Settings → Advanced), right-click the channel, and choose **Copy Channel ID**.

> Screenshot placeholder: Copy Channel ID menu
{% endstep %}

{% step %}
### Copy the bot token

Return to **Bot** in the Developer Portal. Select **Reset Token** or **Copy** (Discord may require you to reset it first), then copy the token.

Treat the token like your Discord password.
{% endstep %}
{% endstepper %}

## Connect it to Fuzzy Macro

1. Open Fuzzy Macro and go to **Config → Discord**.
2. Set **Delivery Mode** to **Use Discord Bot**.
3. Paste the token into **Discord Bot Token**.
4. Paste the channel ID into **Channel ID**.
5. Start or restart the macro, then run `/ping` in that Discord channel. `Pong!` confirms that the bot is online.

The bot uses the Channel ID as its default destination for macro notifications. You do not need a webhook URL in bot-only mode.

> Screenshot placeholder: Fuzzy Macro Discord Delivery settings

## Keep remote control private

By default, a blank command-permission category lets anyone who can use the bot in the server run that category’s commands. For a private server with only you, that may be fine. For any shared server, restrict the categories.

1. With Developer Mode still enabled, right-click your Discord user and choose **Copy User ID**.
2. In **Config → Discord → Bot Command Permissions**, paste your user ID into each category you want to protect. Separate multiple user IDs with commas.
3. At minimum, restrict **Macro Control**, **Task Interrupts**, **Configuration**, **System Actions**, **Profile Access**, and **Streaming**.

The permission categories are designed around risk: observation commands include `/status` and `/screenshot`; control and configuration categories can start, stop, rejoin, or change macro settings.

## Useful commands

Type `/help` in Discord for the command list that matches the current macro version. Common commands include:

* Monitoring: `/status`, `/screenshot`, `/logs`, `/tasklist`, `/nectar`, `/battery`
* Control: `/start`, `/stop`, `/pause`, `/resume`, `/rejoin`, `/reset`, `/skip`
* Configuration: `/settings`, `/fields`, `/field`, `/quests`, `/quest`, `/planters`, `/mobs`, `/hiveslot`, `/macromode`
* Reports and stream: `/hourlyreport`, `/session`, `/stream`, `/streamurl`

## Optional notification routing

The **Notification Routes** section can send categories such as Macro, Reports, Gathering, Combat, Activities, and System to different places. In bot mode, enter a Discord **channel ID** in any route you want to override; leave it empty to use the default Channel ID.

Use this only if you want separate channels. Most people should leave every route blank.

## Troubleshooting

* **`/ping` does not respond:** Make sure Delivery Mode includes Discord Bot, the token is current, the macro is running, and the bot has access to that channel.
* **The slash commands are missing:** Confirm the bot was invited with both `bot` and `applications.commands`, then fully restart Discord. It may take a short time for Discord to refresh commands.
* **Notifications do not arrive:** Confirm that Channel ID is numeric, has no extra spaces, and points to a channel the bot can view and send messages in.
* **“Missing Access” or “Missing Permissions”:** Check the channel’s permission overrides for the bot, especially View Channel, Send Messages, Embed Links, and Attach Files.
