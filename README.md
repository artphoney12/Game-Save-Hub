# GameSave Hub

GameSave Hub is a desktop application for managing offline game save data in internet cafes, gaming centers, and diskless or non-diskless PC environments.

It helps operators keep player save data organized, centralized, and easier to restore across different Client PCs.

The Server stores save data centrally, while the Client allows players to save and load their progress without manually copying folders.

## Purpose

GameSave Hub is designed for shared gaming PCs where many players use different machines, and where local save data may reset after restart.

With GameSave Hub, each player can use a personal account, select a game, choose a save slot, and continue their progress from another Client PC.

## Applications

### GameSave Hub Server

The Server is used by the operator or administrator to manage users, games, save locations, settings folders, quotas, licenses, updates, payments, and Client access.

#### Main Server Features

- User account management
- Game save location management
- Multiple settings/config folder locations per game
- Import and export game lists using `svClient.ini`
- Real-time game title search
- Separate save storage for each user
- Up to 10 save slots per user and game
- Add, delete, and rename save slots
- Global or per-user save storage quotas in MB or GB
- Global or per-user upload and download speed limits
- Server and Client save/load activity summaries
- Admin password protection
- Custom internet cafe name in the application title
- License activation status and usage information
- One-license-one-HWID activation
- Built-in QRIS and PayPal payment access
- Self-update from the official update source
- Automatic extraction of the latest Client package during Server updates
- English and Indonesian language support

### GameSave Hub Client

The Client is used on player PCs to connect to the Server, log in, select games, and perform save/load operations.

#### Main Client Features

- Automatic Server connection
- Client and Server version compatibility check before the session is enabled
- Clear warning when the Client version does not match the Server version
- User login and account creation
- Game list loaded from the Server
- Fast offline game search
- Automatic preparation of save and settings folders
- Manual **Save Now** and **Load Now**
- **Auto Save** every 45 seconds
- Load operations remain manual through **Load Now**
- Save slot selection from Slot 1 to Slot 10
- Add, delete, and rename save slots
- Support for one main save folder and multiple settings/config folders
- Open save folder and settings folder actions
- Transfer progress with percentage and transfer speed
- Clear success and failure notifications
- Retry and permissive reading for locked files
- Automatic skipping of locked nonessential files such as `.log`, `.tmp`, and `.lock`
- Warning or error when important save files remain locked
- Client and Server activity logs for save/load results
- English and Indonesian language support

## Save and Load via Google Drive

GameSave Hub v2.0.1 includes optional Google Drive save/load directly from the Client.

This feature is useful for customers who want an additional cloud backup option, or for players who want their selected save slot to be stored outside the local PC and Server storage.

Google Drive support uses `rclone`, which is already bundled with GameSave Hub. Users do not need to download or install rclone separately.

### Google Drive Features

- Login and logout from Google Drive through the Client
- Google authentication through a dedicated Microsoft Edge app window
- Manual **Save to Google Drive**
- Manual **Load from Google Drive**
- Optional automatic Google Drive upload after a successful Auto Save
- Auto Save runs every 45 seconds, saves to the Server first, and then uploads to Google Drive when cloud auto-save is enabled
- Save and settings folders are stored separately using their Client path structure
- Google Drive authorization is stored locally on the Client PC
- Linked Google Drive account email is displayed in the Client
- Google Drive storage usage, maximum capacity, available capacity, and usage percentage are displayed in the Client
- Built-in Google Drive file manager for viewing and deleting app-managed cloud files

## Operator Benefits

- Centralized save data management for multiple Client PCs
- Easier player progress restoration across different PCs
- Reduced manual folder copying for operators and customers
- Support for diskless and non-diskless environments
- Clear activity logs for save/load monitoring
- Flexible save quota and transfer speed control
- Optional Google Drive cloud backup for selected user, game, and slot data

## Customer Benefits

- Players can log in with their own account
- Save progress can be loaded on another Client PC
- Multiple save slots help separate different progress points
- Manual Load prevents accidental overwrite from automatic loading
- Google Drive support provides an optional cloud save/load option
