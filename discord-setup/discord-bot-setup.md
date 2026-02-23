# Discord Bot Setup

## Installing certificates

{% stepper %}
{% step %}
Run these commands (copy and paste the whole thing into the terminal):

```
python3 -m pip install --upgrade certifi
source $HOME/fuzzy-macro-env/bin/activate
python3 -m pip install --upgrade certifi
```
{% endstep %}
{% endstepper %}

## Creating a Discord bot

{% stepper %}
{% step %}
### Create a new application

![image](<../.gitbook/assets/image (3)>)

Go to [https://discord.com/developers/applications](https://discord.com/developers/applications) and click on “New Application” (top right).

Put in a name, tick the checkbox, and create.

![image](<../.gitbook/assets/image (1) (1)>)
{% endstep %}

{% step %}
### Copy the application ID

Copy the application ID (it is required later).
{% endstep %}

{% step %}
![image](<../.gitbook/assets/image (2) (1)>)

### Configure the bot

In the “Settings” sidebar, click on Bot.

![image](<../.gitbook/assets/image (3) (1)>)

Scroll down to “Privileged Gateway Intents,” check all of them, and save changes.
{% endstep %}

{% step %}
![image](<../.gitbook/assets/image (4)>)

### Generate the invite link

Edit and copy the following link into a web browser (replace with your application ID):

https://discord.com/oauth2/authorize?client\_id=**APPLICATIONID**\&permissions=537390144\&scope=bot

{% hint style="info" %}
For example: https://discord.com/oauth2/authorize?client\_id=1238906\&permissions=537390144\&scope=bot
{% endhint %}
{% endstep %}

{% step %}
### Add the bot to your server

Add your bot to the server and ensure that it has permissions to view the channels you want to use it in.
{% endstep %}

{% step %}
### Reset and copy the bot token

Returning to the application page, reset the bot's token and copy it.
{% endstep %}

{% step %}
![image](<../.gitbook/assets/image (5)>)

### Configure the macro

Launch the macro and copy the token into the 'Discord Bot Token' setting (config -> discord -> Discord Bot).&#x20;

![image](<../.gitbook/assets/image (6)>)

{% hint style="info" %}
NOTE: NEVER share this token; it is like a password for a discord bot.
{% endhint %}
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Note: When you first setup the bot commands make sure you fully close and reopen discord or else the commands wont show up right away (Only happens the first time you setup the bot)
{% endhint %}

#### Current bot commands - Updated 2/23/26

* `/ping` — Check if the bot is online
* `/screenshot` — Send a screenshot of your screen
* `/start` — Start the macro
* `/stop` — Stop the macro
* `/rejoin` — Make the macro rejoin the game
* `/reset` — Reset the character and return to hive
* `/logs` — Show recent macro actions (optionally specify count)
* `/status` — Get the current macro status
* `/nectar` — Show current nectar percentages (current + estimated)
* `/amulet` — Choose to keep or replace an amulet
* `/battery` — Get your current battery status
* `/streamurl` — Get stream URL
* `/close` — Close the macro and/or Roblox
* `/mute` — Mute your Mac.
* `/unmute` — Unmute your Mac.
* `/disablegoo` — Disable goo for a specific field
* `/enablegoo` — Enable goo for a specific field
* `/goostatus` — Check goo status for a specific field
* `/privateserver` — Get or set the configured private server link
* `/settings` — Open settings panel
* `/hiveslot` — Change hive slot number
* `/fields` — View field configuration
* `/field` — Enable or disable a field
* `/swapfield` — Swap one field for another
* `/quests` — View quest configuration
* `/quest` — Enable or disable a quest
* `/collectibles` — View collectibles configuration
* `/collectible` — Edit collectibles configuration
* `/mobs` — View mobs configuration
* `/mob` — Edit mobs configuration
* `/hiveslot` — Change your hiveslot
* `/hourlyreport` — Sends the current hourly report
* `/usehotbar` — Use a hotbar slot (1-7)
* `/macromode` — Set macro mode (normal, quests, or field)
* `/help` — Show available commands
