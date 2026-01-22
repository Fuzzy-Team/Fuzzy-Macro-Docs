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

![image](../.gitbook/assets/image)

Go to [https://discord.com/developers/applications](https://discord.com/developers/applications) and click on “New Application” (top right).

Put in a name, tick the checkbox, and create.

![image](<../.gitbook/assets/image (1)>)
{% endstep %}

{% step %}
### Copy the application ID

Copy the application ID (it is required later).
{% endstep %}

{% step %}
![image](<../.gitbook/assets/image (2)>)

### Configure the bot

In the “Settings” sidebar, click on Bot.

![image](<../.gitbook/assets/image (3)>)

Scroll down to “Privileged Gateway Intents,” check all of them, and save changes.
{% endstep %}

{% step %}
![image](<../.gitbook/assets/image (4)>)

### Generate the invite link

Edit and copy the following link into a web browser (replace with your application ID):

https://discord.com/oauth2/authorize?client\_id=**APPLICATIONID**\&permissions=68608\&scope=bot

{% hint style="info" %}
For example: https://discord.com/oauth2/authorize?client\_id=1238906\&permissions=68608\&scope=bot
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

{% hint style="info" %}
Note: When you first setup the bot commands make sure you fully close and reopen discord or else the commands wont show up right away (Only happens the first time you setup the bot)
{% endhint %}

Discord Bot Commands

#### 🔧 Basic Controls

* `/ping`: Check if the bot is online and responsive.
* `/start`: Start the macro gathering process.
* `/stop`: Stop the macro entirely.
* `/pause`: Temporarily pause the macro at the next checkpoint.
* `/resume`: Continue running the macro from a paused state.
* `/skip`: Skip the current task (e.g., skip a field or a specific quest).
* `/rejoin`: Force the macro to rejoin the game.
* `/close`: Close both the macro application and Roblox.

#### 📊 Status & Monitoring

* `/status`: Get the current state of the macro (Running, Paused, etc.) and the active task.
* `/logs`: Show a list of the most recent macro actions and events.
* `/taskqueue`: Display the current queue of enabled tasks with the active one highlighted.
* `/screenshot`: Send a real-time screenshot of the game window.
* `/streamurl`: Retrieve the current public stream URL if streaming is enabled.
* `/battery`: Check the battery percentage and charging status of the host computer.

#### 🌾 Field & Quest Management

* `/fields`: View which fields are currently enabled for gathering.
* `/enablefield <field>`: Enable a specific field in your gathering list.
* `/disablefield <field>`: Disable a specific field in your gathering list.
* `/swapfield <current> <new>`: Replace an existing field in your list with a new one.
* `/macromode <mode>`: Switch between "Normal" (all tasks), "Quests" (only quests), and "Field" (only gathering) modes.
* `/quests`: View the current quest configuration status.
* `/enablequest <quest>`: Enable quests from a specific NPC (Polar Bear, Honey Bee, etc.).
* `/disablequest <quest>`: Disable quests from a specific NPC.

#### 🎁 Collectibles & Mobs

* `/collectibles`: View which dispensers and collectibles are currently enabled.
* `/enablecollectible <item>`: Enable a specific collectible or dispenser task.
* `/disablecollectible <item>`: Disable a specific collectible or dispenser task.
* `/mobs`: View the current mob run configuration.
* `/enablemob <mob>`: Enable a specific mob (e.g., Werewolf, Spider) for your bug runs.
* `/disablemob <mob>`: Disable a specific mob from your bug runs.

#### 🧪 Goo & Advanced Settings

* `/enablegoo <field>`: Enable the use of goo in a specific field.
* `/disablegoo <field>`: Disable the use of goo in a specific field.
* `/goostatus`: Check the current goo status across all fields.
* `/settings`: View a comprehensive list of all current macro settings grouped by category.
* `/hiveslot <slot>`: Change your hive slot number (1-6).
* `/amulet <keep/replace>`: Remotely choose to keep or replace an amulet during the selection process.

#### 📁 Profile Management

* `/profiles`: List all available configuration profiles.
* `/currentprofile`: Show the name of the profile currently in use.
* `/switchprofile <name>`: Switch to a different saved configuration profile.
* `/createprofile <name>`: Create a new profile based on your current settings.
* `/deleteprofile <name>`: Delete a specific profile (cannot delete the active one).

#### ❓ Help

* `/help`: Display a summarized list of all available commands and their usage categories.
