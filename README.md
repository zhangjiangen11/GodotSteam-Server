# GodotSteam Server for Godot Engine 4.x | Community Edition
An ecosystem of tools for [Godot Engine](https://godotengine.org) and [Valve's Steam](https://store.steampowered.com). For the Windows, Linux, and Mac platforms.

Additional Flavors
---
Pre-Compiles | Plug-ins | Server | Examples
--- | --- | --- | ---
[Godot 2.x](https://github.com/GodotSteam/GodotSteam/tree/godot2) | [GDNative](https://github.com/GodotSteam/GodotSteam/tree/gdnative) | [Server 3.x](https://github.com/GodotSteam/GodotSteam-Server/tree/godot3) | [Skillet](https://github.com/GodotSteam/Skillet)
[Godot 3.x](https://github.com/GodotSteam/GodotSteam/tree/godot3) | [GDExtension](https://github.com/GodotSteam/GodotSteam/tree/gdextension) | [Server 4.x](https://github.com/GodotSteam/GodotSteam-Server/tree/godot4) | ---
[Godot 4.x](https://github.com/GodotSteam/GodotSteam/tree/godot4) | --- | [GDNative](https://github.com/GodotSteam/GodotSteam-Server/tree/gdnative) | ---
[MultiplayerPeer](https://github.com/GodotSteam/MultiplayerPeer)| --- | [GDExtension](https://github.com/GodotSteam/GodotSteam-Server/tree/gdextension) | ---

Documentation
---
[Documentation is available here](https://godotsteam.com/). You can also check out the Search Help section inside Godot Engine after compiling it with GodotSteam Server.

Feel free to chat with us about GodotSteam or ask for assistance on the [Discord server](https://discord.gg/SJRSq6K).

Donate
---
Pull-requests are the best way to help the project out but you can also donate through [Github Sponsors](https://github.com/sponsors/Gramps)!

Current Build
---
You can [download pre-compiled versions of this repo here](https://github.com/GodotSteam/GodotSteam-Server/releases).

**Version 4.5 Changes**
- Added: missing Utils class: functions, enums, constants
- Changed: minor clean-ups
- Fixed: wrong accessor for Networking Sockets, thanks to ***Michael Janesway***
- Fixed: missing callback fro `validate_auth_ticket_response`, thanks to ***Michael Janesway***
- Fixed: all wronge accessors for all other class functions

[You can read more change-logs here](https://godotsteam.com/changelog/server4/).

Compatibility
---
While rare, sometimes Steamworks SDK updates will break compatilibity with older GodotSteam versions. Any compatability breaks are noted below. API files (dll, so, dylib) _should_ still work for older version.

Steamworks SDK Version | GodotSteam Version
---|---
1.59 or newer | 4.2 or newer
1.58a or older | 4.1 or older

Versions of GodotSteam that have compatibility breaks introduced.

GodotSteam Version | Broken Compatibility
---|---
4.3| Networking identity system removed, replaced with Steam IDs
4.4 | sendMessages returns an Array

Known Issues
---
- Steam overlay will not work when running your game from the editor if you are using Forward+ as the renderer.  It does work with Compatibility though.  Your exported project will work perfectly fine in the Steam client, however.
- When self-compiling, **do not** use MinGW as it will cause crashes.

Quick How-To
---
For complete instructions on how to build the Godot 4.x version of GodotSteam Server from scratch, [please refer to our documentation's 'How-To Modules' section.](https://godotsteam.com/howto/server/) It will have the most up-to-date information.

Alternatively, you can just [download the pre-compiled versions in our Releases section](https://github.com/GodotSteam/GodotSteam-Server/releases) and skip compiling it yourself!

License
---
MIT license
