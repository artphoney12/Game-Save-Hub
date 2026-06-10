# GameSave Hub

GameSave Hub is a desktop application for managing offline game save data in internet cafes, gaming centers, and both diskless and non-diskless PC environments.

It is designed for shared gaming PCs where many players use different client machines, and where local files may reset after restart. The server stores save data centrally, while the client helps players load and save progress without manual file handling.

## Purpose

GameSave Hub makes game save handling easier, cleaner, and more consistent across multiple PCs.

Each player can use their own account, choose a game, select a save slot, and keep progress available even when moving to another PC.

## Applications

### GameSave Hub Server

The server manages users, game lists, save locations, settings/config folders, save quotas, license activation, payment access, updates, and client access.

Main server features:

- User account management
- Game save location management
- Additional settings/config folder management per game
- Import and export game list from `svClient.ini`
- Real-time game title search
- Per-user save storage
- Up to 10 save slots per user per game
- Slot add, delete, and rename
- Global or per-user save quota (MB / GB)
- Global or per-user upload/download speed limit
- Activity logs for server and client save/load summaries
- Admin password protection
- Internet cafe name branding in app title
- License tab with activation status and usage rules
- One-license-one-HWID activation
- Built-in payment page access for QRIS and PayPal
- Offline/payment connection fallback message in the embedded payment view
- Self-update from official update source
- Server self-update also extracts the latest Client package automatically
- Single-instance protection

### GameSave Hub Client

The client connects to the server, allows user login, displays offline game list, and handles save/load operations.

Main client features:

- Auto-connect to server
- User login and account creation
- Game list loaded from server
- Search box for offline game titles
- Local save folder and settings folder preparation after connection
- Manual Save Now and Load Now
- Auto Save + Load mode
- Save slot selection (Slot 1 to Slot 10)
- Slot add, delete, and rename
- Support for main save folder plus additional settings/config folders
- Open save folder and open settings folder actions
- Blocking progress window with percentage and transfer speed
- Strong success and failure notifications
- Skips locked nonessential files such as `.log`, `.tmp`, and `.lock` after retry attempts
- Shows warning/error when important save files remain locked and cannot be copied
- Activity logs for save/load results and skipped locked files
- English / Indonesia language setting
- Single-instance protection

Save files are synchronized as real files (not zip archives).

## Screenshots

### GameSave Hub Server

![](https://i.ibb.co.com/XZ153GGM/Game-Save-Hub-Server-VWYNWVRWK8.png)
![](https://i.ibb.co.com/sdDjCKc2/Game-Save-Hub-Server-WSFPn-Zb2qh.png)
![](https://i.ibb.co.com/qwX31G5/Game-Save-Hub-Server-i8wt-Kv-RASF.png)

### GameSave Hub Client

![](https://i.ibb.co.com/GwPvyqd/Game-Save-Hub-r-Cy2-Puwnh-Y.png)
![](https://i.ibb.co.com/W4SMHyBz/Game-Save-Hub-l-KEENC7-A5-A.png)

### License / Activation

![](https://i.ibb.co.com/8nhNXKzv/license.png)
