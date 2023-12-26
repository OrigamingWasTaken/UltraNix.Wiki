#### Is this a recompilation of ULTRAKILL?
No. This is a script that downloads a dummy UnityPlayer, and moves the game files into their proper place to be run on UNIX-likes. It's basically a glorified mod installer.

#### Is this speedrun legal?
No. This counts as a modification to the game files, which makes it illegal for speedruns.

![Screenshot_20231226-114607_Discord (6)](https://github.com/coatlessali/UltraNix/assets/61166135/732f043c-259f-40f7-a261-6e04b2dd1186)


#### Is this supported?
Not officially. Please don't report any bugs occurring with these ports to any official sources, unless you can reproduce them on the Windows build. I will provide as much support as I can, but don't be surprised if the devs add a Windows-only library, or remove OpenGLCore, and the game stops working permanently. Feel free to open issues in the GitHub repository, or hit me (coatlessali) up in the ULTRAKILL or Newblood Discord servers.

![244906341-86499157-27e0-4c30-bf52-5eb80ff0b064](https://github.com/coatlessali/UltraNix/assets/61166135/4431dfc9-f115-4e56-8fdf-1a34eb1ea24b)

#### What if the ULTRAKILL team members take issue with this project?
At their request, **I will take down this repository/all associated plugins, no questions asked.** Though judging by the fact that they went as far as to convert the MP4 files in the game to WEBMs for (presumably) better WINE compatibility, if I had to guess, I'd say they probably don't mind.

#### What are the system requirements for Linux?
Here are the specs for the worst computer (an Elitebook 8460p) that I have managed to get the game running decently on, under Debian 12 on XFCE:
* CPU: Intel Core i5-2520M
* GPU: AMD Radeon HD 6470M / 1GB GDDR3
* RAM: 2 GiB DDR3 (WITH NOTHING ELSE OPEN)

This should net you a minimum of 50 FPS at 960p, even on some of the laggier levels like 4-2/5-3. Technically all you really need is an x86_64 processor, a distro using glibc, and OpenGL 3.2 support.

#### What are the minimum system requirements for MacOS?
Great question. Not sure.

#### Where do I get ULTRAKILL?
You can purchase it via Steam in a web browser, and download it using the methods documented [here](https://github.com/coatlessali/UltraNix/wiki/Downloading-ULTRAKILL-and-Plugins).

#### That's too hard, so I downloaded ULTRAKILL from GameUnlocked9000.gov, can you help me set it up?
**No.** Go buy it.

#### Why can't you ship the plugins for Steam/Discord?
They are copyrighted material that I cannot freely distribute. I know it's inconvenient, but I'd rather not get letters from either company's legal team.

#### What the heck does "upstream" mean?
In this case, I am using "upstream" to refer to the developers of ULTRAKILL, as well as the private project files for the game that they have. For example, an issue that can "only be fixed upstream" is an issue that is up to the developers of the game to address, as it would either be impossible/impractical to fix with a mod. This repo and any mods associated with it, would be considered "downstream".

#### Does this yield better performance?
It depends. I initially thought that the CPU overhead of running OpenGL would be far greater than the overhead of running WINE/Proton, but it seems for Unity in specific, I was wrong.

If your CPU is the bottleneck, this will improve performance. If your GPU is the bottleneck, this will either do nothing, or possibly even hurt your performance.

#### I can use Proton instead, should I?
It depends. If you don't mind the work necessary to get this working and can live with the caveats, it can be worth your time, especially if you're in a situation where it could improve performance (see above).

#### Are mods supported?
Not 100%. You need to use the version of BepInEx for your Operating System, and not every mod works due to compatibility issues.

#### I'm having a problem, any help?
Check the [known issues page.](https://github.com/coatlessali/UltraNix/wiki/Known-Issues), or the issue tracker.