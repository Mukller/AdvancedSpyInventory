<div align="center">

[![License: MIT](https://img.shields.io/badge/License-MIT-purple?style=flat-square)](LICENSE.md)
[![maintained](https://img.shields.io/badge/maintained%3F-yes-green?style=flat-square)](https://github.com/Mukller/AdvancedSpyInventory)
[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen?style=flat-square)](CONTRIBUTING.md)

### 🌐 Язык / Language

**Нажми, чтобы развернуть нужный язык · Click to expand your language**

</div>

<details open>
<summary><b>🇬🇧 English</b></summary>

<br>

# AdvancedSpyInventory

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

</details>

<details>
<summary><b>🇷🇺 Русский</b></summary>

<br>

# AdvancedSpyInventory

<div align="center">

**🔍 Продвинутый плагин для просмотра инвентаря игроков на сервере PaperMC**

[![Java](https://img.shields.io/badge/Java-11%2B-blue?style=flat-square&logo=java)](https://www.java.com/)
[![PaperMC](https://img.shields.io/badge/PaperMC-Latest-green?style=flat-square&logo=minecraft)](https://papermc.io)
[![License](https://img.shields.io/badge/License-MIT-purple?style=flat-square)](LICENSE)


</div>

## 📌 Описание

AdvancedSpyInventory — это плагин для PaperMC, позволяющий администраторам и модераторам сервера удобно просматривать содержимое инвентаря, эндерчеста и других хранилищ любого игрока в реальном времени. Идеален для проверки честности игроков и борьбы с читерством.

## ✨ Возможности

- ✅ **Просмотр инвентаря** игроков в реальном времени
- ✅ **Просмотр эндерчеста** (если поддерживается)
- ✅ **Защита от модификаций** во время просмотра
- ✅ **Удобный интерфейс** с поддержкой навигации
- ✅ **Логирование** действий администраторов
- ✅ **Полная локализация** на русский язык
- ✅ **Конфигурируемость** под твой сервер

## 🚀 Быстрый старт

### Требования

- **Java**: 11 или выше
- **PaperMC**: Latest версия рекомендуется
- **Права администратора** на сервере

### Установка

1. Скачай последнюю версию плагина (`.jar` файл)
2. Положи файл в папку `plugins/` твоего сервера
3. Перезагрузи сервер командой `/reload` или перезапусти его
4. Плагин готов к работе!

```bash
# Если нужна перезагрузка конфигурации
/reload
```

## 📖 Использование

### Основная команда

```
/spy <ник игрока>
```

**Пример:**
```
/spy PlayerName
```

### Кто может использовать?

По умолчанию необходимо одно из следующих прав:
- Оператор сервера (`/op`)
- Роль с разрешением `advancedspyinventory.spy` или `advancedspyinventory.admin`

### Команды

| Команда | Описание | Разрешение |
|---------|---------|-----------|
| `/spy <ник>` | Открыть инвентарь игрока | `advancedspyinventory.spy` |
| `/spy reload` | Перезагрузить конфиг плагина | `advancedspyinventory.admin` |
| `/spy help` | Справка по командам | `advancedspyinventory.spy` |

## ⚙️ Конфигурация

После первого запуска плагина в папке `plugins/AdvancedSpyInventory/` будет создан файл `config.yml`.

### Пример config.yml

```yaml
# Основные настройки
settings:
  # Показывать уведомления при просмотре инвентаря
  notify-player: true
  
  # Логировать действия в консоль
  logging-enabled: true
  
  # Префикс сообщений плагина
  prefix: "&8[&3SpyInventory&8]"

# Сообщения (кастомизация)
messages:
  player-offline: "&cИгрок не найден или оффлайн"
  no-permission: "&cУ вас нет доступа к этой команде"
  success: "&aИнвентарь загружен"
```

Отредактируй файл под свои нужды и используй `/spy reload` для применения изменений.

## 🔐 Разрешения (Permissions)

```
advancedspyinventory.spy          # Базовое разрешение на просмотр инвентаря
advancedspyinventory.admin        # Полный доступ + команды администратора
advancedspyinventory.notify       # Получать уведомления о просмотре
advancedspyinventory.reload       # Перезагружать конфигурацию
```

### Пример с Permission плагином (LuckPerms)

```
/lp user <username> permission set advancedspyinventory.spy true
/lp user <username> permission set advancedspyinventory.notify true
```

## 🐛 Частые проблемы

### Плагин не работает после установки

1. Убедись, что версия Java не ниже 11
2. Проверь консоль сервера на ошибки: `/say test`
3. Попробуй перезагрузить сервер полностью (не просто `/reload`)

### Команда /spy не работает

- Проверь, что у тебя есть нужные разрешения
- Убедись, что целевой игрок онлайн
- Попробуй введести ник без пробелов и спецсимволов

### Ошибка при открытии инвентаря

Это может быть вызвано:
- Конфликтом с другим плагином
- Некорректным config.yml (проверь синтаксис YAML)
- Устаревшей версией PaperMC

**Решение:** Удали config.yml, перезагрузи плагин, он создаст новый конфиг по умолчанию.

## 📊 Версионирование

Проект использует [Semantic Versioning](https://semver.org/):
- **MAJOR** — несовместимые изменения API
- **MINOR** — новые функции, совместимые с предыдущими версиями
- **PATCH** — исправления ошибок

Текущая версия: **2.4.13**

## 🤝 Вклад в проект

Мы приветствуем любые улучшения! Если хочешь помочь:

1. **Форк** репозитория
2. **Создай ветку** для твоей функции (`git checkout -b feature/AmazingFeature`)
3. **Закоммитай** изменения (`git commit -m 'Add some AmazingFeature'`)
4. **Запуши** ветку (`git push origin feature/AmazingFeature`)
5. **Открой Pull Request**

### Рекомендации

- Следуй существующему стилю кода
- Добавляй комментарии к сложным логикам
- Обновляй документацию при необходимости
- Убедись, что плагин скомпилировался без ошибок

## 📝 Лицензия

Проект распространяется под лицензией **MIT**. Подробнее см. файл [LICENSE](LICENSE).

**Ключевые моменты:**
- ✅ Можешь использовать в коммерческих целях
- ✅ Можешь модифицировать
- ✅ Можешь распространять
- ❌ Обязателен указание авторства и лицензии

## 👤 Автор

**Mukller**  
GitHub: [@Mukller](https://github.com/Mukller)

## 📮 Поддержка

Если у тебя возникли вопросы или ты нашел баг:

1. Проверь [Issues](https://github.com/Mukller/AdvancedSpyInventory/issues) — может быть уже есть решение
2. Создай новую [Issue](https://github.com/Mukller/AdvancedSpyInventory/issues/new) с подробным описанием
3. Укажи версию плагина и PaperMC

**При создании Issue укажи:**
```
Версия плагина: 2.4.13
Версия PaperMC: X.X.X
Java версия: 11/17/21
Описание проблемы: ...
```

## 🎮 Совместимость

| Версия | Статус |
|--------|--------|
| 1.20+ | ✅ Полная поддержка |
| 1.19 | ✅ Поддерживается |
| 1.18 | ⚠️ Возможны проблемы |
| < 1.18 | ❌ Не поддерживается |

## 📚 Дополнительные ресурсы

- [PaperMC Документация](https://docs.papermc.io/)
- [Bukkit API](https://hub.spigotmc.org/javadocs/bukkit/)
- [SpigotMC (скачивание плагинов)](https://www.spigotmc.org/)

---

<div align="center">

Made with ❤️ by Mukller

⭐ Если проект помог, поставь звезду!

</div>

</details>
