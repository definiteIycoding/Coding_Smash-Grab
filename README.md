# Coding Smash & Grab

A standalone, feature-packed script for **Qbox** and **QBCore** that lets players smash **store windows** and **car windows** for loot.

## ✨ Features
- Smash store windows & car windows
- Per-store loot pools (convenience, liquor, electronics, jewelry)
- Global and per-vehicle cooldowns + per-player anti-spam
- Police alerts with night-time bonus
- Optional min cops requirement
- Vehicle class blacklist (disable smashing emergency/military by default)
- Optional evidence drop hook
- Discord logging with styled embeds (💎 🚗 📦 👮)
- Author branding + anti-rename protection
- Framework toggle: `qbcore` / `qbox`
- No external dependencies

---

## 📦 Install
1. Drop **`coding_smashandgrab`** into `resources`.
2. Add to `server.cfg`:
   ```
   ensure coding_smashandgrab
   ```
3. Edit **`shared/config.lua`**:
   - Set `Config.Framework` to `'qbcore'` or `'qbox'`
   - Put your Discord webhook in `Config.DiscordWebhook`
   - Adjust loot, cooldowns, min cops, blacklist, evidence, etc.

---

## 🧰 Tips
- Add your own stores by copying entries in `Config.Locations`. You can set `loot = "Loot_Convenience"` (or any table key) to override the pool.
- If your inventory uses different item names, edit the loot tables.
- Evidence hook calls `Config.Evidence.Event` with the smash coordinates; integrate with your police script as needed.

---

## 👨‍💻 Author
Created and copyrighted by **DefinitelyCoding**
