# Stream setup

The stream allows the macro to stream your screen in real-time through a link. This lets you watch your macro from other devices, such as your phone while you are away.

{% stepper %}
{% step %}
### Download Homebrew

Download Homebrew:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```
{% endstep %}

{% step %}
### Install cloudflared

Open a new terminal and run the command below:

{% code title="Command (Apple Silicon / Homebrew installed in /opt/homebrew)" %}
```
brew install cloudflared
```
{% endcode %}
{% endstep %}
{% endstepper %}

### Enable stream setting

In your macro GUI, under Config → Stream, check the "Enable stream" option.

![](<../.gitbook/assets/image (25)>)

### Getting the stream link

When you start the macro, it will start the stream. Once the stream is ready, it will send the link via the webhook. You can also enable it to pin this stream in chat if that helps you.

![](<../.gitbook/assets/image (26)>)
