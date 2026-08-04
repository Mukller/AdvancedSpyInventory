<div align="center">

**English** • [Русский](README.md)

</div>

# AdvancedSpyInventory

<p align="center">
  <a href="https://github.com/Mukller">
    <img src="https://img.shields.io/badge/Anton%20Petnitsky-Developer-0d1117?style=for-the-badge&logo=github&logoColor=white&labelColor=0d1117&color=58a6ff" alt="Anton Petnitsky" />
  </a>
</p>


<div align="center">

**🔍 An advanced plugin for viewing players' inventories on a PaperMC server**

[![Java](https://img.shields.io/badge/Java-11%2B-blue?style=flat-square&logo=java)](https://www.java.com/)
[![PaperMC](https://img.shields.io/badge/PaperMC-Latest-green?style=flat-square&logo=minecraft)](https://papermc.io)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)](LICENSE)

</div>

## 📌 Description

AdvancedSpyInventory is a PaperMC plugin that lets server admins and moderators conveniently view the contents of any player's inventory, ender chest, and other storages in real time. Perfect for verifying fair play and fighting cheating.

## ✨ Features

- ✅ **View inventory** of players in real time
- ✅ **View ender chest** (if supported)
- ✅ **Protection from modifications** while viewing
- ✅ **Convenient UI** with navigation support
- ✅ **Logging** of admin actions
- ✅ **Full localization** into Russian
- ✅ **Configurable** for your server

## 🚀 Quick start

### Requirements

- **Java**: 11 or higher
- **PaperMC**: latest version recommended
- **Admin rights** on the server

### Installation

1. Download the latest plugin version (`.jar` file)
2. Place the file into your server's `plugins/` folder
3. Reload the server with `/reload` or restart it
4. The plugin is ready to go!

```bash
# If you need to reload the configuration
/reload
```

## 📖 Usage

### Main command

```
/spy <player name>
```

**Example:**
```
/spy PlayerName
```

### Who can use it?

By default one of the following is required:
- Server operator (`/op`)
- A role with the `advancedspyinventory.spy` or `advancedspyinventory.admin` permission

### Commands

| Command | Description | Permission |
|---------|---------|-----------|
| `/spy <name>` | Open a player's inventory | `advancedspyinventory.spy` |
| `/spy reload` | Reload the plugin config | `advancedspyinventory.admin` |
| `/spy help` | Command help | `advancedspyinventory.spy` |

## ⚙️ Configuration

On first launch the plugin creates `config.yml` in `plugins/AdvancedSpyInventory/`.

### Example config.yml

```yaml
# Main settings
settings:
  # Show a notification when viewing an inventory
  notify-player: true
  
  # Log actions to the console
  logging-enabled: true
  
  # Plugin message prefix
  prefix: "&8[&3SpyInventory&8]"

# Messages (customization)
messages:
  player-offline: "&cPlayer not found or offline"
  no-permission: "&cYou don't have access to this command"
  success: "&aInventory loaded"
```

Edit the file to suit your needs and use `/spy reload` to apply changes.

## 🔐 Permissions

```
advancedspyinventory.spy          # Basic permission to view inventories
advancedspyinventory.admin        # Full access + admin commands
advancedspyinventory.notify       # Receive view notifications
advancedspyinventory.reload       # Reload the configuration
```

### Example with a permissions plugin (LuckPerms)

```
/lp user <username> permission set advancedspyinventory.spy true
/lp user <username> permission set advancedspyinventory.notify true
```

## 🐛 Common issues

### The plugin doesn't work after installation

1. Make sure Java is version 11 or higher
2. Check the server console for errors: `/say test`
3. Try a full server restart (not just `/reload`)

### The /spy command doesn't work

- Check that you have the required permissions
- Make sure the target player is online
- Try entering the name without spaces or special characters

### Error opening the inventory

This can be caused by:
- A conflict with another plugin
- An invalid config.yml (check the YAML syntax)
- An outdated PaperMC version

**Solution:** delete config.yml and reload the plugin — it will create a fresh default config.

## 📊 Versioning

The project uses [Semantic Versioning](https://semver.org/):
- **MAJOR** — incompatible API changes
- **MINOR** — new features, backward compatible
- **PATCH** — bug fixes

Current version: **2.4.13**

## 🤝 Contributing

We welcome any improvements! If you want to help:

1. **Fork** the repository
2. **Create a branch** for your feature (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** the branch (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Recommendations

- Follow the existing code style
- Add comments to complex logic
- Update the documentation when needed
- Make sure the plugin compiles without errors

## 📝 License

This project is distributed under the **MIT** license. See the [LICENSE](LICENSE) file for details.

**Key points:**
- ✅ You can use it commercially
- ✅ You can modify it
- ✅ You can distribute it
- ❌ Attribution and the license notice are required

## 👤 Author

**Mukller**  
GitHub: [@Mukller](https://github.com/Mukller)

## 📮 Support

If you have questions or found a bug:

1. Check [Issues](https://github.com/Mukller/AdvancedSpyInventory/issues) — there may already be a solution
2. Create a new [Issue](https://github.com/Mukller/AdvancedSpyInventory/issues/new) with a detailed description
3. Include the plugin and PaperMC version

**When creating an Issue, include:**
```
Plugin version: 2.4.13
PaperMC version: X.X.X
Java version: 11/17/21
Problem description: ...
```

## 🎮 Compatibility

| Version | Status |
|--------|--------|
| 1.20+ | ✅ Full support |
| 1.19 | ✅ Supported |
| 1.18 | ⚠️ Possible issues |
| < 1.18 | ❌ Not supported |

## 📚 Extra resources

- [PaperMC Docs](https://docs.papermc.io/)
- [Bukkit API](https://hub.spigotmc.org/javadocs/bukkit/)
- [SpigotMC (plugin downloads)](https://www.spigotmc.org/)

---

<div align="center">

Made with ❤️ by Mukller

⭐ If the project helped, give it a star!

</div>
