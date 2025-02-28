# Changelog Page  
**Language**: English (International)  

---

## VERSION: INDEV  
**Format version**: `@indev:(update-number)(day)(month)(year)`

---

### @indev:0124022025  

#### 🆕 New Features  

**Scripts**  
- Added `PayUI` (MenuUI)  
- Added `WeatherUI` (AdminUI)  
- Added `GamemodeUI` (AdminUI)  
- Added `TimesetUI` (AdminUI)  
- Added `DevMenu` (secret feature)  
- Added new command `cdclearchat` to see countdown duration for clearchat  
- Added `extension/scorehud.js` (tested)  

**JSON UI**  
- Added `scorehudUI` (`ui/hud_screen.json`), using title and subtitle  

#### 🛠️ Changes & Fixes  

**Scripts**  
- Rebuilt `extension/clear-system.js`, `extension/kill-death.js`  
- Sorted enable & disable toggle  
- Migrated all extensions based on `devResources` into `dev-resources` folder  
- Exported module `@minecraft/server` in `backend/menu/list/index.js`  
- Fixed spam bug in `Gamemode Changes`  
- Fixed some bugs  

#### ❌ Removed  

**Scripts**  
- Removed `chatWrapping` (`extension/chatWrap.js`)  

#### ⚠️ Known Issues  

**Scripts**  
- `cdclearchat` countdown is static  
- `clear-system` not working  

---

### @indev:0224022025  

#### 🛠️ Changes & Fixes  

**Scripts**  
- Fixed bug in `WeatherUI`  
- Fixed command `cdclearchat` & `extension/clear-system`  

**JSON UI**  
- Fixed layout of `scorehud` subtitle  
- Changed the default texture of `scorehud` to `cleanUI`  

---

### @indev:0125022024  

#### 🆕 New Features  

**Scripts**  
- Added `list/scorehud.js` (tested in development)  

#### 🛠️ Changes & Fixes  

**Scripts**  
- `PWarpUI` is now a stable feature (`pwarp:test` → `pwarp:stable`)  
- Fixed some bugs  

#### ❌ Removed  

**Scripts**  
- Removed `AnnouncementUI`  

#### ⚠️ Known Issues  

**Scripts**  
- `Scorehud Exp` is not counted  

---

### @indev:0127022025  

#### 🆕 New Features  

**Scripts**  
- Added `veinminer` (`extension/veinminer.js`)  

#### 🛠️ Changes & Fixes  

**JSON UI**  
- Customized `ui/pause_screen.json` into `OreUI` style (cleaner design)  

#### ❌ Removed  

**Scripts**  
- Removed some unused methods and code  

#### ⚠️ Known Issues  

**Scripts**  
- Error: failed to call `dimension` in `backend/menu/list/punishment.js`  

---

## @indev:0128022025  

#### 🆕 New Features  

**Scripts**  
- Formatted placeholder in `scorehud.js`  
- Added filter to hide `scorehud` for players with `noScoreHud` tag  
- Implemented `formatNum` method in `scorehud.js`  
- Added `_isEnabled` method in `punishment.js`  

#### 🛠️ Changes & Fixes  

**Scripts**  
- Used more `while` loops in `scorehud.js`  
- Increased `stayDuration` for subtitle to prevent disappearance due to lag in `scorehud.js`  
- Rewrote some logic in `punishment.js`  
- Updated `blockWhiteList` regex in `config.js` (removed netherite from group 1, added as new value)  
- Optimized `QuickDB` to use object-based caching (`quick-db.js`)  
- Implemented constructor looping in `QuickDB` to preload data (`quick-db.js`)  
- Added logic to remove `"delete"` values from constructor looping in `QuickDB` (temporary)  

**Manifest.json**  
- Updated module `@minecraft/server` to `1.18.0-beta`  

**JSON UI**  
- Modified elements in `pause_screen.json`  

#### ❌ Removed  

**Scripts**  
- Removed item checks in `backend/menu/list/punishment.js` (replaced with optional chaining)  
- Removed `#UIDX` method from `QuickDB` (`quick-db.js`)  

#### ⚠️ Known Issues  

- `clear chat` doesn't work  
- Possible errors in `QuickDB`  
- Slowdown when minimized, causing `watchdog` to kill the server  

---

## @indev:0228022025  

#### 🆕 New Features  

**Scripts**  
- Added command `help` to display a list of commands  
- Added `veinminer` property in `config.js` (default: `false`)  
- Added command `scorehud` to toggle scorehud visibility  

#### 🛠️ Changes & Fixes  

*(Details not provided, update accordingly)*  
