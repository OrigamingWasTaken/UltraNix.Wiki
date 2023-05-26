## Downloading ULTRAKILL (Steam)

Downloading ULTRAKILL via Steam may prove a little daunting at first. When you try to download it, you will more than likely be met with a grayed out download button, and a notification that says "AVAILABLE ON WINDOWS". Do not fret, however, as it is perfectly possible to download ULTRAKILL on these platforms.

### Gotchas: Copying from Windows

While copying the game over from Windows may work, I would **highly suggest** downloading the game again on your platform. This is because NTFS (the Windows File System) does not handle file permissions the same way as most UNIX file systems do. Downloading the files on your platform ensures that there won't be any permission issues, and ensures you have a fresh/clean copy of the game.

### Linux

You can download ULTRAKILL on Linux by enabling Steam Play for unsupported titles. This can be done in "Steam" -> "Settings" -> "Compatibility" on the latest Steam client. Enable Support for all other titles using Proton Experimental, and then close the window.

![20230524_16h20m59s_grim](https://github.com/coatlessali/UltraNix/assets/61166135/d0359184-d51c-4004-8eec-14ea6456abfc)
![20230524_16h21m07s_grim](https://github.com/coatlessali/UltraNix/assets/61166135/47e5548a-755c-45d4-b86d-d071934a6ec1)

When prompted, restart Steam, and the game should be available to download. The default download location on Linux is `/home/user/.steam/steam/steamapps/common/`.

### MacOS

As Steam Play isn't available on MacOS, we have to trick the Steam client into downloading it using a file known as an **appmanifest.acf** Start by downloading the [.acf](https://github.com/coatlessali/UltraNix/blob/main/appmanifest_1229490.acf) file included in the GitHub repo. Now, you should move it to `/Users/$USER/Library/Application Support/Steam/steamapps/`, and restart Steam if it's already open.

After relaunching Steam, the game should automatically start downloading. By default, it will download to `/Users/$USER/Application Support/Steam/steamapps/common/`.

## Downloading the Steamworks SDK and Discord Game SDK (Optional)

In order for Steamworks integration (for in-game Leaderboards, Steam Rich Presence) and Discord integration (Discord Rich Presence) to work, you need to download the MacOS/Linux binaries for the specific versions of those plugins that are used by ULTRAKILL.

### Steamworks SDK

Start by signing into your Steam account on the [Steamworks Website](https://partner.steamgames.com/). After this, you can go to [this page](https://partner.steamgames.com/downloads/list) to download the Steamworks SDK. Make sure to download version **1.48a**, as this is the version ULTRAKILL uses.

After opening up the `.zip` file, navigate to `sdk/redistributable_bin/`. From here:

- If on Linux, go to `linux64`, and extract the `libsteam_api.so` file somewhere safe.
- If on MacOS, go to `osx`, and extract the `libsteam_api.dylib` file somewhere safe.

### Discord Game SDK

Go to the [Discord Game SDK](https://discord.com/developers/docs/game-sdk/sdk-starter-guide) page and download the Discord Game SDK **v2.5.6**.

After opening up the `.zip` file, navigate to `/lib/x86_64/`, and from there:

- If on Linux, extract the `discord_game_sdk.so` file somewhere safe.
- If on MacOS, extract the `discord_game_sdk.dylib` file somewhere safe.

### After Downloading

Now that you have everything you need, move onto Running the Script.