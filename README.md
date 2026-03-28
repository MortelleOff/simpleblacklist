# 🛡️ Simple Blacklist (Anti-Cheat & Mod Control)

**Simple Blacklist** is a powerful, lightweight Fabric utility designed for server administrators who want absolute control over the mods players bring into their server. Protect your community from hacked clients and unauthorized advantages with ease.

## ✨ Features

* **🚫 Active Blacklist**: Instantly block and kick players attempting to join with forbidden mods (e.g., Wurst, Meteor, Aristois).
* **🔔 Discord Webhook Alerts**: Receive real-time notifications directly in your Discord server whenever a player is caught using a blacklisted mod.
* **✅ Smart Whitelist (Known Mods)**: The server recognizes your approved modpack. Any unrecognized mod is flagged as "Suspect" for admins to review, without automatically banning the player.
* **🖱️ Interactive In-Game Moderation**: Run a simple command to view a player's mod list. Suspect mods appear in red and are **clickable**—click them in the chat to instantly add them to the server's whitelist!
* **🔄 Live Configuration**: Reload your settings, change kick messages, and update your whitelists/blacklists on the fly. No server restarts required!
* **🌐 Language Configuration**: English and French are fully supported and configurable !
* **📥 Client Auto-Updater**: The client automatically checks for updates via GitHub. If a new version is found, it downloads it and prompts the player to restart their game.

## 🛠️ Admin Commands (Requires OP / Permission Level 2)

All commands are centralized under `/simplebl`:
* `/simplebl checkmods <player>` : View a player's active mod list (Sorted by Suspects and Approved).
* `/simplebl allowmod <modid>` : Permanently add a suspect mod to the server's known whitelist.
* `/simplebl verif <player>` : Force a manual re-check of a player's mods.
* `/simplebl reload` : Reload the `simpleblacklist.json` configuration file instantly.

## ⚙️ Installation & Setup

**⚠️ IMPORTANT:** This mod is a synchronization tool. It MUST be installed on **BOTH** the Server and the Client.

1. Drop the `.jar` into your server's `mods` folder.
2. Include the `.jar` in your players' `mods` folder (or your official Modpack).
3. Start the server once to generate the config file.
4. Open `config/simpleblacklist.json` on your server to set up your **Discord Webhook URL**, customize your kick messages, and add your known mods.

*(Note: Players connecting without the mod installed will be automatically kicked after a customizable timeout of 40 seconds).*
