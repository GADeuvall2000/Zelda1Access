Zelda 1 Access
by G-Rad

Zelda 1 Access adds accessibility features to the NES game The Legend of Zelda so it can be played with a screen reader.

This release will allow you to play through both quests to completion. 


Features:
- Spoken menus and dialog
- Spoken inventory sub-screen with treasure cycling
- Pathfinding and navigation across overworld, dungeons, caves, and basements
- Spatial enemy radar and item beacons
- Footstep and wall-bump audio cues
- Player-placed waypoints
- Accessibility menu for toggling features and adjusting volumes
- Emulated Second controller Save Screen shortcut

This requires BizHawk.  If you don't have it, download it here:
https://github.com/Lethal-Lawnmower/BizHawk/releases/tag/v1.0.0-accessibility

Installation:
1. Place `nvdaControllerClient64.dll` and `Tolk.dll` in the root of your BizHawk folder.
2. Copy the `Zelda1 Access` folder into BizHawk's `Lua` folder.
3. Run `SoundBridge.bat` from the newly located Zelda1Access Folder.
4. Start BizHawk and load The Legend of Zelda.
5. Once Zelda is running, open the Lua Console and load `Zelda1Access.lua`.
6.  If you loaded it successfully, you will hear the Secret revealed chime.
7. Play.

Notes:
- `nvdaControllerClient64.dll` and `Tolk.dll` must be in the root BizHawk directory.
- Do not remove files from the `Zelda1 Access` folder or the script will not work.
- You must load the game first before loading the script or the script will not work.
- The sound bridge handles both screen-reader speech and synthesized game audio (footsteps, bumps, radar pings, item beacons).

In-Game Controls:
- D-Pad, Defaults to Arrow keys: Move Link
- `A` button, Defaults to `X` on Keyboard: Use Sword
- `B` button, Defaults to `Z` on Keyboard: Use Secondary item
- `Select Button, Defaults to `Spacebar` on Keyboard: Pause Game
- `Start Button, Defaults to `Enter` on keyboard: Open inventory

Accessibility Shortcuts:
- `Delete`: Open Accessibility Menu
- `L` or `Insert`: Announce current location (screen, dungeon, cave, or basement)
- `G`: Announce current Rupees
- `B`: Announce current Bombs
- `K`: Announce current Keys
- `H`: Announce current Health in Hearts
- `; (semi)`: Announce current B item
- `' (Apostrophe)`: Announce current A item (sword)
- `D`: Repeat last spoken dialog
- `M`: Probe current tile coordinate

Pathfinding:
- `Page Up` / `Page Down`: Cycle through entities on the screen
- `Home`: Repeat selected entity
- `End`: Announce directions to selected entity

Waypoints:
- `Shift + /`: Add a waypoint at Link's current tile (prompts for label)
- `Shift + M`: Relabel the selected waypoint
- `, (comma)` / `/`: Cycle previous / next waypoint on the current screen
- `.`: Navigate to the selected waypoint
- `Shift + , (comma)`: Remove the selected waypoint
- `Shift + .`: Clear all waypoints

Inventory Subscreen:
- `Page Up` / `Page Down`: Cycle through owned treasures (Raft, Book, Ring, Stepladder, Master Key, Power Bracelet, plus current dungeon's Map and Compass)
- `Home`: Announce current Triforce pieces
- `End`: Announce Current Shield
- `L` or `Insert`: Announce current Quest
- `Shift` + `End`: Go to Save Screen


Accessibility Menu:
- `Up` / `Down`: Move between menu items
- `Left` / `Right`: Adjust selected setting
- `Delete` or `Escape`: Close menu

Settings include overworld and dungeon coordinate format, footsteps, wall bumps, item beacons, item drop linger, enemy radar, enemy auto-lock, freeze enemies, and targeted suppression for some enemies.
