# AdvancedSpyInventory

<div align="center">

**🔍 Advanced inventory viewing plugin for PaperMC**

[![Java](https://img.shields.io/badge/Java-11%2B-blue?style=flat-square&logo=java)](https://www.java.com/)
[![PaperMC](https://img.shields.io/badge/PaperMC-Latest-green?style=flat-square&logo=minecraft)](https://papermc.io)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)](LICENSE)

[English](README_EN.md) • [Русский](README.md)

</div>

## 📌 Description

AdvancedSpyInventory is a PaperMC plugin that allows server administrators and moderators to conveniently view the inventory, ender chest, and other storage containers of any player in real-time. Perfect for checking player honesty and fighting cheating.

## ✨ Features

- ✅ **View player inventory** in real-time
- ✅ **View ender chest** (if supported)
- ✅ **Protection from modifications** during viewing
- ✅ **Convenient interface** with navigation support
- ✅ **Action logging** for administrators
- ✅ **Full Russian localization** with English support
- ✅ **Configurable** for your server

## 🚀 Quick Start

### Requirements

- **Java**: 11 or higher
- **PaperMC**: Latest version recommended
- **Server operator** rights

### Installation

1. Download the latest version of the plugin (`.jar` file)
2. Place the file in the `plugins/` folder of your server
3. Reload the server with `/reload` or restart it completely
4. Plugin is ready to use!

```bash
# If you need to reload config
/reload
```

## 📖 Usage

### Main Command

```
/spy <player_name>
```

**Example:**
```
/spy PlayerName
```

### Who Can Use?

By default, you need one of the following:
- Server operator (`/op`)
- Role with `advancedspyinventory.spy` or `advancedspyinventory.admin` permission

### Commands

| Command | Description | Permission |
|---------|-------------|-----------|
| `/spy <name>` | Open player's inventory | `advancedspyinventory.spy` |
| `/spy reload` | Reload plugin config | `advancedspyinventory.admin` |
| `/spy help` | Command help | `advancedspyinventory.spy` |

## ⚙️ Configuration

After the first plugin run, a `config.yml` file will be created in the `plugins/AdvancedSpyInventory/` folder.

### Example config.yml

```yaml
# Main settings
settings:
  # Show notifications when viewing inventory
  notify-player: true
  
  # Log actions to console
  logging-enabled: true
  
  # Plugin message prefix
  prefix: "&8[&3SpyInventory&8]"

# Messages (customization)
messages:
  player-offline: "&cPlayer not found or offline"
  no-permission: "&cYou don't have access to this command"
  success: "&aInventory loaded"
```

Edit the file according to your needs and use `/spy reload` to apply changes.

## 🔐 Permissions

```
advancedspyinventory.spy          # Basic permission to view inventory
advancedspyinventory.admin        # Full access + admin commands
advancedspyinventory.notify       # Receive view notifications
advancedspyinventory.reload       # Reload configuration
```

### Example with Permission Plugin (LuckPerms)

```
/lp user <username> permission set advancedspyinventory.spy true
/lp user <username> permission set advancedspyinventory.notify true
```

## 🐛 Troubleshooting

### Plugin doesn't work after installation

1. Make sure Java version is 11 or higher
2. Check server console for errors: `/say test`
3. Try full server restart (not just `/reload`)

### /spy command doesn't work

- Check that you have the necessary permissions
- Make sure the target player is online
- Try entering the nickname without spaces and special characters

### Error when opening inventory

This could be caused by:
- Conflict with another plugin
- Incorrect config.yml (check YAML syntax)
- Outdated PaperMC version

**Solution:** Delete config.yml, reload the plugin, it will create a new default config.

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
4. **Push** your branch (`git push origin feature/AmazingFeature`)
5. **Open a Pull Request**

### Recommendations

- Follow existing code style
- Add comments to complex logic
- Update documentation if needed
- Make sure the plugin compiles without errors

## 📝 License

The project is distributed under the **MIT** license. See [LICENSE](LICENSE) file for details.

**Key points:**
- ✅ Can be used for commercial purposes
- ✅ Can be modified
- ✅ Can be distributed
- ❌ Attribution and license must be included

## 👤 Author

**Mukller**  
GitHub: [@Mukller](https://github.com/Mukller)

## 📮 Support

If you have questions or found a bug:

1. Check [Issues](https://github.com/Mukller/AdvancedSpyInventory/issues) — there might be a solution already
2. Create a new [Issue](https://github.com/Mukller/AdvancedSpyInventory/issues/new) with a detailed description
3. Specify the plugin and PaperMC version

**When creating an Issue, please provide:**
```
Plugin version: 2.4.13
PaperMC version: X.X.X
Java version: 11/17/21
Problem description: ...
```

## 🎮 Compatibility

| Version | Status |
|---------|--------|
| 1.20+ | ✅ Full support |
| 1.19 | ✅ Supported |
| 1.18 | ⚠️ Possible issues |
| < 1.18 | ❌ Not supported |

## 📚 Additional Resources

- [PaperMC Documentation](https://docs.papermc.io/)
- [Bukkit API](https://hub.spigotmc.org/javadocs/bukkit/)
- [SpigotMC (plugin downloads)](https://www.spigotmc.org/)

---

<div align="center">

Made with ❤️ by Mukller

⭐ If the project helped, star it!

</div>
