## All Platforms
* All limitations of GLCore are present, such as disabled silhouettes. [\*](https://github.com/coatlessali/GLCoreScissors)
* There is a **crippling mouse bug** that causes any click/release input to repeat the last axis movement (including mouse movement and scroll wheel) by one unit. This means if you scroll to change weapons and don't move the mouse before clicking, you will change weapons again upon trying to fire.

## Linux
* Scrolling in menus is very slow/inverted.
* Game may randomly abort during startup.
* Usage of gamescope and alt-tabbing may cause input problems.
* `-force-wayland` doesn't work.

For Wayland, you can `LD_PRELOAD=/usr/lib/libSDL2.so SDL_VIDEODRIVER=wayland` at the beginning of your Steam launch options. This will load a newer version of SDL2 that will allow you to run the game with Wayland without a hang.

## MacOS
* Using mouse tweaking software such as [Mos](https://mos.caldis.me/) can cause scrolling issues, especially if smooth scrolling is turned on.
* The game will crash if certain folders aren't present in `ULTRAKILL.app`, such as `Preferences`, `CyberGrind`, and `Saves`.