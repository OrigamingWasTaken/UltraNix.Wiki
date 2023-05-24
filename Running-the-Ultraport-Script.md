These instructions will assume you have ULTRAKILL downloaded to the default download locations on MacOS/Linux.

- For MacOS, this is `/Users/$USER/Library/Application Support/Steam/steamapps/common/ULTRAKILL`.
- For Linux, this is `/home/$USER/.steam/steam/steamapps/common/ULTRAKILL`.

I will from here-on be referring to either of these directories as simply the "ULTRAKILL folder", for the sake of convenience.

## Linux

If you're on Linux, start by downloading [ULTRAPORT.tar.gz](https://github.com/coatlessali/UltraNix/blob/main/ULTRAPORT.tar.gz) and [ultraport.sh](https://github.com/coatlessali/UltraNix/blob/main/ultraport.sh).

Now, move the following files into your ULTRAKILL folder:

- ULTRAPORT.tar.gz
- ultraport.sh
- libsteam_api.so (Optional)
- discord_game_sdk.so (Optional)

Open your favorite terminal emulator, and `cd` to your ULTRAKILL folder.

`$ cd /home/$USER/.steam/steam/steamapps/common/ULTRAKILL/`

Ensure the script is executable,

`$ chmod +x ./ultraport.sh`

and then run the script.

`$ ./ultraport.sh`

Once it's done, the terminal should give you a command to copy paste into your Steam launch options, to be able to launch the game from Steam.

`/home/$USER/.steam/steam/steamapps/common/ULTRAKILL/ULTRAKILL.x86_64; echo %command%`

Alternatively, you can run it directly from the terminal:

`$ ./ULTRAKILL.x86_64`

Note: If it crashes one or two times starting up, that's okay. Unity 2019 sometimes aborts on startup.

## MacOS

Start by downloading [Darwin.tar.gz](https://github.com/coatlessali/UltraNix/blob/main/Darwin.tar.gz), and [ultraport.sh](https://github.com/coatlessali/UltraNix/blob/main/ultraport.sh).

Now move the following files into your ULTRAKILL folder:

- Darwin.tar.gz
- ultraport.sh
- libsteam_api.dylib (Optional)
- discord_game_sdk.dylib (Optional)

Now open the Terminal app, and `cd` to your ULTRAKILL folder:

`$ cd /Users/$USER/Application\ Support/Steam/steamapps/common/ULTRAKILL/`

Ensure the script is executable,

`$ chmod +x ./ultraport.sh`

and run it.

`$ ./ultraport.sh`

After it finishes, open your ULTRAKILL folder in Finder. Right click a new app that will have appeared, named `ULTRAKILL` (though the `.app` part will be hidden), and click "Open". MacOS will prompt you to let you know the app is unverified, but it is safe to run. **From now on, this is how you will have to open the game.**