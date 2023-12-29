## All Platforms
* All limitations of GLCore are present, such as disabled silhouettes. [GLCoreScissors can fix this with caveats, but has been broken since at least Patch 14b.](https://github.com/coatlessali/GLCoreScissors)
* There is a **crippling mouse bug** that causes any click/release input to repeat the last axis movement (including mouse movement and scroll wheel) by one unit. This means if you scroll to change weapons and don't move the mouse before clicking, you will change weapons again upon trying to fire.
* If your OpenGL drivers are faulty, you may run into issues with the camera switching in 4-S making the level unplayable.

## Linux
* Scrolling in menus is very slow/inverted.
* Game may randomly abort during startup.
* Usage of gamescope and alt-tabbing may cause input problems.
* `-force-wayland` doesn't work without using `LD_PRELOAD` to load your system's SDL2 library. This option also doesn't work with the `./run_bepinex.sh` script, so replace it with the env var `SDL_VIDEODRIVER=wayland`.

## MacOS
* Using mouse tweaking software can cause scrolling issues, especially if smooth scrolling is turned on. I'm hesitant to say this is an issue with the game, but I'd rather put it here to be safe.
* The game will crash if certain folders aren't present in `ULTRAKILL.app`, such as `Preferences`, `CyberGrind`, and `Saves`. I believe it is permissions related.
* For some unexplained reason, the MacOS port might have permissions denied and not be able to run. No idea why, I don't use a Mac.