# Stream setup

The stream allows the macro to stream your screen in real-time through a link. This lets you watch your macro from other devices, such as your phone while you are away.

{% stepper %}
{% step %}
### Download Homebrew

Download Homebrew:

https://brew.sh/
{% endstep %}

{% step %}
### Install cloudflared

Open a new terminal and run one of the commands below (only one of them will work on your system):

{% hint style="info" %}
Run only the command that matches your Homebrew installation path.
{% endhint %}

{% code title="Command (Apple Silicon / Homebrew installed in /opt/homebrew)" %}
```
```
{% endcode %}

{% code title="Command (Intel / Homebrew installed in /usr/local)" %}
```
```
{% endcode %}
{% endstep %}
{% endstepper %}

### Enable stream setting

In your macro GUI, under Config → Stream, check the "Enable stream" option.

![](<../.gitbook/assets/image (25)>)

### Getting the stream link

When you start the macro, it will start the stream. Once the stream is ready, it will send the link via the webhook.

![](<../.gitbook/assets/image (26)>)
