# Discord Webhook Setup

{% hint style="warning" %}
**Use a Discord bot instead unless you specifically need a webhook.** A webhook only sends one-way notifications. It cannot provide slash commands, remote controls, bot command permissions, or bot-channel delivery. See [Discord Bot Setup](discord-bot-setup.md) for the recommended setup.
{% endhint %}

## When a webhook makes sense

Choose a webhook if you only want notifications in one channel and do not want to create a Discord application. It is also useful when an existing server already manages notifications through a webhook.

Choose **Use Both** only when you need bot commands plus a webhook-specific feature, such as pinning the stream URL. Otherwise, use **Use Discord Bot** instead.

{% hint style="warning" %}
Anyone with a webhook URL can post to its channel. Keep the URL private; do not share it in screenshots, tickets, or messages. If it leaks, delete or regenerate the webhook in Discord and replace the URL in Fuzzy Macro.
{% endhint %}

## Create the webhook

{% stepper %}
{% step %}
### Choose a Discord channel

Create or select the channel that should receive macro notifications. A private channel such as `#fuzzy-macro` is recommended.
{% endstep %}

{% step %}
### Open the channel integrations

Open the channel’s settings, select **Integrations**, then select **Webhooks**. Depending on your Discord layout, you may instead reach this from **Server Settings → Integrations**.

> ![](<../.gitbook/assets/image (3).png>)
{% endstep %}

{% step %}
### Create and copy the webhook

Select **New Webhook**, give it a recognizable name, confirm its channel, and save. Choose **Copy Webhook URL**.

> ![](<../.gitbook/assets/image (4).png>)
{% endstep %}
{% endstepper %}

## Connect it to Fuzzy Macro

1. Open Fuzzy Macro and go to **Config → Discord**.
2. Set **Delivery Mode** to **Use Webhook**.
3. Paste the URL into **Webhook URL**.
4. Start the macro and wait for a notification, or trigger an event such as starting the macro to test it.

Webhook mode uses the Webhook URL as the default destination. The macro can attach screenshots, send reports, and apply the Discord ping options, but it cannot receive commands.

> ![](<../.gitbook/assets/image (5).png>)

## Optional notification routing

In **Notification Routes**, paste a webhook URL into any category you want to send elsewhere. Categories left blank fall back to the default Webhook URL.

Route values must be a full `https://` webhook URL in webhook mode. Do not paste a channel ID unless you are using the Discord bot.

## Troubleshooting

* **No messages arrive:** Verify Delivery Mode is **Use Webhook**, the URL begins with `https://`, and the webhook has not been deleted or regenerated.
* **A route does not work:** Check that its value is a complete webhook URL, not a channel ID or a copied message link.
* **Screenshots are missing:** Enable **Send Screenshots** in Config → Discord and ensure Discord allows file attachments in the destination channel.
