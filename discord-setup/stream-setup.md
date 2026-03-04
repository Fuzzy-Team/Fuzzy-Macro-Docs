# Stream setup

The stream allows the macro to stream your screen in real-time through a link. This lets you watch your macro from other devices, such as your phone, while you are away.

## macOS Installation

{% stepper %}
{% step %}
### Download Homebrew

Run this command in Terminal:

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

## Windows Installation

{% stepper %}
{% step %}
### Download Winget

Run this command in PowerShell (as Administrator):

<pre class="language-ps1"><code class="lang-ps1">Invoke-WebRequest -Uri https://aka.ms/getwinget -OutFile winget.msixbundle
<strong>Add-AppxPackage winget.msixbundle
</strong>del winget.msixbundle
</code></pre>
{% endstep %}

{% step %}
### Install cloudflared

Open a new command prompt window and run the command below:

```bash
winget install --id Cloudflare.cloudflared
```
{% endstep %}
{% endstepper %}

### Enable stream setting

In your macro GUI, under Config → Stream, check the "Enable stream" option.

![](<../.gitbook/assets/image (25)>)

### Getting the stream link

When you start the macro, it will start the stream. Once the stream is ready, it will send the link via the webhook. You can also enable it to pin this stream in chat if that helps you.

![](<../.gitbook/assets/image (26)>)
