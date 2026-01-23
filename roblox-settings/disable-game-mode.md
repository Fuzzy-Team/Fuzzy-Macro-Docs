# Disable game mode

{% hint style="warning" %}
For macOS 14.0+ (Sonoma) only
{% endhint %}

{% stepper %}
{% step %}
### Disable Game Mode in Roblox (quick)

* Launch Roblox and make it fullscreen.
* Click the controller icon in the Apple menu and disable Game Mode.

_Sometimes it turns on by itself, so check regularly to make sure it's off. If you are unable to turn it off, try restarting your Mac._

![](<../.gitbook/assets/image (12)>)
{% endstep %}

{% step %}
### If Game Mode Won't Turn Off (pause/auto-reenable issues)

Follow these steps to kill the gamepolicyd process in Activity Monitor:

* Open Activity Monitor (Applications > Finder).

![](<../.gitbook/assets/image (13)>)

*   Press the magnifying-glass icon and search:

    Copy:

    ```
    gamepolicyd
    ```

![](<../.gitbook/assets/image (14)>)

* Double-click the process (the only one shown) and ensure the process window appears as below:

![](<../.gitbook/assets/image (15)>)

* Press the Quit button and choose Force Quit.

![](<../.gitbook/assets/image (16)>)

Alternatively:

* Back on the search results, select gamepolicyd (click ONCE) and press the "x" in a hexagon in the upper-left to quit.

![](<../.gitbook/assets/image (17)>)

Note: gamepolicyd will start to back up after being force-quit (this is normal).

* After force-quitting, you should be able to turn off Game Mode. Go to the upper-right and press the game controller icon.

![](<../.gitbook/assets/image (18)>)
{% endstep %}
{% endstepper %}
