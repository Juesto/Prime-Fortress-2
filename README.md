**This repository is for our mod code related to Prime Fortress 2 modification, based on Nicknine's tf_port.
Our goal is to provide what we think how Team Fortress 2 should be.**

Team Fortress 2
=====

This is the old Team Fortress 2 source code from February 2008 ported to Source Engine 2013. This ensures the game has all the latest engine features and security fixes. No new features will be added to the code. No bugs will be fixed with the exception of crashes and bugs that were not in the original 2008 build of the game.

Assets that need to be used with compiled binaries and running instructions can be foun in the official Facepunch thread: https://web.archive.org/https://forum.facepunch.com/games/squi/Team-Fortress-2-1-0-1-8-Source-2013-Port/

## Dependencies

### Windows
* [Visual Studio 2013 with Update 5](https://visualstudio.microsoft.com/vs/older-downloads/)

### macOS
* [Xcode 5.0.2](https://developer.apple.com/downloads/more)

### Linux
* GCC 4.8
* [Steam Client Runtime](http://media.steampowered.com/client/runtime/steam-runtime-sdk_latest.tar.xz)

## Building

Compiling process is the same as for Source SDK 2013. Instructions for building Source SDK 2013 can be found here:
https://developer.valvesoftware.com/wiki/Source_SDK_2013


## Installing:

### Client:

1. Go to the Tools section in your Steam Library and install Source SDK Base 2013 Multiplayer. 

2. Download the client package and extract its contents to <Steam>\steamapps\sourcemods.

3. Restart Steam. "Prime Fortress 2" should appear in your Steam Library.

NOTE: If you're on Linux or Mac, Steam client currently has a bug where it doesn't attach -steam parameter when running Source mods like it's supposed to. You'll need to manually add -steam parameter to the mod in your Steam Library.

### Server:

1. These instructions assume you know how to host a dedicated server for TF2 and/or other Source games. If you don't, refer to these articles:

   * https://developer.valvesoftware.com/wiki/SteamCMD
   
   * https://wiki.teamfortress.com/wiki/Windows_dedicated_server 
   
   * https://wiki.teamfortress.com/wiki/Linux_dedicated_server 

2. Use SteamCMD to download app 244310 (Source SDK Base 2013 Dedicated Server).

3. Download the server package and extract its contents to where you installed Source SDK Base 2013 Dedicated Server.

4. If you're on Linux, go to <server_install_folder>/bin and make copies of the files as follows:

   * soundemittersystem_srv.so -> soundemittersystem.so

   * scenefilecache_srv.so -> scenefilecache.so
