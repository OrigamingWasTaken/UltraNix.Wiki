# Mod Support for UNIX

## Installation
Refer to [BepInEx's Documentation](https://docs.bepinex.dev/articles/user_guide/installation/index.html?tabs=tabid-nix) for installing the version of BepInEx necessary for *your* platform.

## Compatibility
Mods currently have hit-or-miss compatibility. This isn't usually an issue with Linux/MacOS, moreso the Unity Player/Mono not correcting Windows specific filepaths (i.e. `\` as the file separator instead of `/`), or not having shaders compiled for OpenGL. (By Default, Unity uses exclusively D3D11/D3D12 for Windows.)

Here are some reasons your mod might not work correctly:
* File paths in the code are specific to Windows. (i.e. `\\` or `@"\"` instead of `Path.DirectorySeparatorChar()`, not using `Path.Combine()`.)
* Shaders aren't compiled for your platform. (OpenGL on MacOS/Linux)

### Note for MacOS:
Having `libsteam_api64.dylib` in `ULTRAKILL.app/Contents/Frameworks/MonoEmbedRuntime/osx/` will **cause BepInEx to hang at the loading screen.** You can remove this file to proceed, however leaderboard support will be lost. This also renders mods that require Steam integration effectively useless. `(Can anyone confirm this is still a problem?)`

## r2modman
Please do not use r2modman unless you know what you are doing. I have found it significantly more reliable to manually manage your mods.

**If you choose to use r2modman, I will not provide any support. You are free to do so, but you are on your own.**

## NOTE:
The compatibility list was removed due to a lack of maintenance. I don't have the time to test every mod in existence anymore, especially since there are so many now. It will be replaced with an issue tracker in the future.