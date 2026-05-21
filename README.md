# GameSave Hub

GameSave Hub is a desktop application for managing offline game save data in internet cafes, gaming centers, and diskless PC environments.

It is designed for shared gaming PCs where many players may use different client machines, and where local files can be reset after restart. The server stores user save data centrally, while the client helps players load and save their progress without manual file handling.

## Purpose

GameSave Hub makes game save handling easier, cleaner, and more consistent across multiple cafe PCs.

Each player can use their own account, choose a game, select a save slot, and keep their progress available even when moving to another PC.

## Applications

### GameSave Hub Server

The server manages users, game lists, save locations, user storage, save quotas, license activation, and client access.

Main server features:

- User account management.
- Game save location management.
- Real-time game title search.
- Per-user game save storage.
- Up to 10 save slots per user and game.
- Slot add, delete, and rename management.
- Global or per-user save quota limit in MB / GB.
- Admin password protection.
- Internet cafe name branding in the app title.
- License tab with activation status and license rules.
- One-license-one-HWID activation.
- Self-update support from the official update source.
- Single-instance protection.

The server stores local data beside the server executable:

- `game_save_hub.db`
- `users`

The `updates` folder is created only when the self-update process runs.

### GameSave Hub Client

The client connects to the server, lets users log in, lists offline games, and handles save/load actions.

Main client features:

- Auto-connect to server.
- User login and account creation.
- Game list loaded from server.
- Search box for offline game titles.
- Local save folder preparation after connection.
- Manual `Save Now` and `Load Now`.
- Auto `Save + Load` mode.
- Save slot selection from `Slot 1` to `Slot 10`.
- Slot add, delete, and rename.
- Blocking progress window with percentage and transfer speed.
- Strong success and failure notifications.
- English / Indonesia language setting.
- Single-instance protection.

Save files are synchronized as real files, not zip archives.
