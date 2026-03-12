# MHAI - Homunculus AI Configuration Manager

**The ultimate visual configuration tool for Ragnarok Online Zero Homunculus AI.**

MHAI lets you fully customize your homunculus behavior through an intuitive GUI — no manual Lua editing required. Configure combat strategies, cooperative modes, skill usage, friend/enemy lists, and more with just a few clicks.

---

## ✨ Core Highlights

### Smart GUI Management Interface
- **One-Click Operation** — All settings configured through visual buttons, no manual `.lua` editing needed
- **Real-Time Status Display** — Button colors dynamically reflect current settings (Green = Enabled, Red = Disabled, Orange = Special State)
- **Quick Presets** — Built-in "Active Combat", "Passive Defense", and "Sentry Mode" presets for instant switching
- **Smart Tooltip System** — Every feature includes detailed descriptions, beginner-friendly
- **Dark Mode** — Easy on the eyes during long gaming sessions
- **Multi-Language** — English and Traditional Chinese interface support

### Auto-Update System
- **Version Management** — Automatically detects the latest version and displays update details
- **One-Click Update** — Supports independent or synchronized updates for both the program and Lua files

---

## ⚔️ Combat System

### 🔁 Four Cooperative Modes (Core Feature)

The intelligent cooperative system supports four combat modes, switchable via **ALT+T**:

#### 🟢 Passive Cooperative Mode
- **How it works:** Homunculus stays idle by default, only joins combat when the owner starts attacking
- **Attack logic:** Assists by attacking the same target the owner is attacking (including players)
- **Best for:** Safe grinding, avoiding accidental aggro, situations requiring precise control

#### 🔵 Active Attack Mode
- **How it works:** Fully autonomous — searches and attacks enemies within line of sight
- **Attack range:** Supports monsters and players (adjustable via "Attack Settings")
- **Best for:** AFK grinding, maximizing farming efficiency
- **Feature:** Can be combined with "Continuous Combat" mode for seamless chain attacks

#### 🔴 Target Lock Mode (PVP)
- **How it works:** 100% synchronized with the owner's current locked target
- **Special mechanic:** Ignores ALL filter settings (attack settings, black/whitelists)
- **Attack priority:** Whatever the owner attacks, the homunculus attacks
- **Best for:** PVP combat, situations requiring absolute obedience
- **Switching behavior:** Instantly follows when the owner switches targets; returns to idle after kill

#### 🟣 Bot Lock Mode (Recommended for Botting)
- **How it works:** Syncs with owner's target when locked; auto-searches and attacks when no target is locked
- **Smart logic:** Dual active + passive logic, perfect for AFK combat
- **Counter-attack support:** Enable counter-attack mode to prioritize protecting the owner when attacked
- **Best for:** Bot grinding, semi-automatic combat
- **Feature:** Combines the best of Active and Target Lock modes — ideal for botting

---

### 🛡️ Counter-Attack System
- **Owner Protection** — When the owner is attacked, the homunculus prioritizes switching targets to protect the owner
- **PVP Tip** — Recommended to disable during PVP to avoid splitting firepower

---

### ⚙️ Attack Intensity (3 Levels)

#### Standard Mode (Safe & Stable)
- Returns to the owner's side after each kill
- Maintains safe following distance
- Best for situations requiring control

#### Continuous Combat (Efficiency Priority)
- Immediately searches for the next target after a kill
- Reduces return time, increases farming efficiency
- Best for AFK grinding

#### Aggressive Mode (Maximum Efficiency)
- Does not return to owner + relaxed distance limits
- Maximizes attack range and frequency
- Best for clearing large areas in safe zones

---

### 🧍 Sentry Mode
- **Fixed Guard** — Move your homunculus to a designated position, then enable to guard that area
- **Auto-Return** — Automatically returns to the guard point after killing a target or losing aggro
- **Best for:** Guarding specific locations, instance checkpoints, fixed-position farming

---

### 💃 Dance Attack Mode
- **Attack Speed Boost** — Noticeably increases normal attack frequency and fluidity
- **Auto-Adjustment** — Automatically optimizes attack rhythm based on ASPD
- **Side Effect** — May reduce SP recovery rate
- **Note** — May not suit all attack speeds; testing recommended

---

### 🧠 Smart Pathfinding
- Homunculus attempts to navigate around obstacles to reach targets
- Detects if a monster is behind a wall and abandons the target early
- Avoids getting stuck on trees, small pits, and other map obstacles
- Built-in fail-safe mechanism

---

## 🎯 Target Settings

### Basic Target Filters

Flexibly control your homunculus's attack target range:

| Setting | Description | Recommended |
|---------|-------------|-------------|
| Attack Monsters | Whether to attack normal monsters | Enable while grinding |
| Attack Players | Whether to include players as targets | Enable for PVP |
| Attack Friends | Whether to attack whitelisted characters | Usually disabled |
| Attack Homunculi | Whether to attack other players' homunculi | Enable for PVP |
| Attack Plants | Grass/mushroom/Mandragora attack settings | 3-tier adjustment |

### 🌿 Plant Attack (3-Tier Setting)
- 🚫 **Don't Attack Plants** — Completely ignores all plant-type targets
- ✅ **Attack Plants** — Attacks all grass, mushrooms, and Mandragoras
- 🟡 **Attack All Except Mandragoras** — Avoids botting issues with plants and Mandragoras (Recommended)

---

### 🧙 Smart Attack Priority (PVP)
- **Priority order:** Wizard > Dancer > Blacksmith > Normal logic
- **Auto-sorting:** Intelligently analyzes enemy threat levels, prioritizes high-threat targets
- **Limitation:** Only supported in fully active attack mode
- **Mutually exclusive:** Cannot be enabled simultaneously with counter-attack mode

---

### 🎯 Instance Priority
- **Priority targeting** of instance monsters — prioritizes breaking flowers, eggs, and other instance objectives
- **Efficiency boost** — Quickly fulfills instance quest requirements
- **Smart detection** — Automatically identifies special instance targets

---

### 💎 Gorgeous Metal Lock
- **Absolute priority** — Ignores all attack modes, permanently locks onto Gorgeous Metal
- **No switching** — Will not change targets until the Gorgeous Metal is destroyed

---

## ✨ Skill System

### Skill Mode (3-Tier Switch)

#### Use Skills (Smart Casting)
- Can cast different skill levels based on owner/homunculus HP thresholds
- Each skill can be individually toggled on/off with custom delay settings

#### Skills on Players Only (PVP)
- Does not cast skills on monsters (conserves mana)
- Only uses skills against player targets
- Best for PVP combat scenarios

#### No Skills (Pure Physical)
- Completely disables skill casting
- Pure normal attacks only
- Saves SP consumption

---

## 🤝 Whitelist System

### Core Features
- **Target Exclusion** — Whitelisted characters will not be attacked
- **Area Selection** — Supports batch selection of multiple targets
- **Deduplication** — Same character won't be registered twice
- **Quick Add All** — One-click to add all visible characters to the whitelist
- **Persistent Storage** — Whitelist persists through map changes, teleportation, re-summoning

### Use Cases
- Avoid friendly fire on party members during group grinding
- Mark friendly players / guild members
- Set safe NPCs and players in botting areas

---

## ☠️ Blacklist System

### Core Features
- **Lock-On Attack** — Prioritizes attacking blacklisted targets
- **Persistent Records** — Blacklist persists through map changes, teleportation, re-summoning
- **Backup & Restore** — Supports blacklist data backup and restoration
- **Priority Control** — Configurable attack priority for blacklisted targets

### Blacklist Priority
- **Enable Priority Attack** — Blacklisted targets take priority over normal targets
- **Disable Priority Attack** — Blacklist serves as record only, doesn't affect attack order

### Use Cases
- Mark specific hostile players during PVP
- Mark special monsters that need to be killed first in instances

---

## ⌨️ Hotkey System

### ALT + T (Quick Mode Switch)
- **Double-tap trigger** — Quickly press ALT+T twice to activate
- **Designated switch** — Configurable which mode ALT+T switches to
- **Instant effect** — No need to re-summon the homunculus (resets after teleportation)
- **Combat-ready** — Can switch modes during combat at any time

---

## 🧠 Smart Recognition System

### NPC Auto-Detection
- **Auto-filter** — Identifies and avoids attacking guide NPCs, channel NPCs, shop NPCs
- **Safety guarantee** — Prevents accidental interaction with important NPCs
- **Zero configuration** — System auto-detects, no manual setup needed
- **Pet recognition** — Prevents homunculus from attacking pets

---

## 🧪 Supported Homunculus Types

| Type | Specialty | Key Skills |
|------|-----------|------------|
| **Vanilmirth** | Magic | Caprice (8013), Chaotic Blessing (8014) |
| **Filir** | Attack | Moonlight (8009) + Dual BUFFs: Flitting (8010), Emergency Avoid (8011) |
| **Amistr** | Defense | Castling / Defense BUFF (8006) |
| **Lif** | Support | Auto-Heal + Movement BUFF (8002) |

---

## ⚠️ Important Notes

- **Settings take effect after:** Re-summoning / Teleporting / Changing maps / Homunculus going out of sight and respawning at your feet
- Settings changes do **not** require restarting the game client

---

## Download & Installation

### Download
1. Go to the [**Releases**](https://github.com/Mehits3/MHAI-release/releases) page
2. Download the latest `MHAIv{version}.exe`

### Installation
1. Place the `.exe` file in your Ragnarok Online Zero installation directory
   - Recommended: same folder as your game client, or any convenient location
2. Run the `.exe` — the application will automatically detect your AI directory at:
   ```
   {Game Root}\AI\USER_AI\RNAI\
   ```
3. If the AI directory is not found automatically, you will be prompted to select it manually

### First-Time Setup
1. Launch MHAI
2. Activate your license (purchase required)
3. Configure your homunculus settings through the tabbed interface
4. Settings are saved automatically to your Lua configuration files

## System Requirements

- **OS**: Windows 10 / 11
- **Game**: Ragnarok Online Zero (with Homunculus AI support)
- **Network**: Internet connection required for updates and license activation
- **Disk**: ~20 MB free space

## License & Pricing

MHAI is commercial software. A valid license is required to use the application.

**Available Plans:**
- **30-Day License** — Monthly subscription
- **365-Day License** — Annual subscription
- **Lifetime License** — One-time purchase, permanent access

Visit the application's built-in license activation window to purchase and activate your license.

## FAQ

**Q: Where are my settings saved?**
A: Settings are saved directly to Lua files in your `AI\USER_AI\RNAI\custom\` directory.

**Q: Will updates overwrite my settings?**
A: No. The update system preserves your personal configuration while updating the AI logic.

**Q: Can I use MHAI with multiple game windows?**
A: Yes. MHAI uses a unified configuration system (`homunculus_config.lua`) with deep copy mechanism, so each game window loads independent parameters.

**Q: The application can't find my AI directory.**
A: Click the directory selection button and manually navigate to your `AI\USER_AI\RNAI\` folder.

## Support

If you encounter issues or have questions:
- Open an [Issue](https://github.com/Mehits3/MHAI-release/issues) on this repository
- Include your MHAI version number and a description of the problem

---

*MHAI is not affiliated with or endorsed by Gravity Co., Ltd.*
