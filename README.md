# MHAI - Homunculus AI Configuration Manager

**A visual configuration tool for Ragnarok Online Zero Homunculus AI.**

MHAI lets you customize your homunculus behavior through an intuitive GUI — no manual Lua editing required. Configure combat strategies, skill usage, friend/enemy lists, and more with just a few clicks.

---

## Features

- **Visual Configuration** — Toggle AI settings with simple on/off buttons instead of editing Lua files manually
- **Combat AI Control** — Fine-tune attack priorities, skill usage, and combat scenarios (counter-attack, protect owner, active attack)
- **Skill Management** — Configure skill delays, SP thresholds, and priority levels for each homunculus type
- **Friend & Enemy Lists** — Manage your homunculus's friend and enemy lists with real-time file monitoring
- **Auto Updates** — Built-in update system automatically downloads the latest version
- **Multi-Language** — English and Traditional Chinese (繁體中文) interface support
- **Dark Mode** — Easy on the eyes during long gaming sessions

## Supported Homunculus Types

| Type | Specialty | Key Skills |
|------|-----------|------------|
| **Lif** | Movement BUFF | 輕捷移動 (8002) |
| **Amistr** | Defense BUFF | 防禦力 (8006) |
| **Filir** | Attack | 月光 (8009), 橫越速度 (8010), 緊急迴避 (8011) |
| **Vanilmirth** | Magic | 善變 (8013), 混亂祈福 (8014) |

## Screenshots

> *Coming soon — screenshots of the main interface and configuration panels.*

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
