<div align="center">
    <img src="https://github.com/nickdesi/proxmenux/blob/main/images/main.png"
         alt="ProxMenux Logo"
         style="max-width: 100%; height: auto;" >
</div>

<br />

**ProxMenux** is a management tool for **Proxmox VE** that simplifies system administration through an interactive menu, allowing you to execute commands and scripts with ease.

---

## ✨ Features

- 🖥️ **Interactive Menu System** - Easy navigation with `dialog` based interface
- 🌐 **Multi-language Support** - English, Spanish, French (with translation caching for performance)
- 🔧 **Hardware Configuration** - GPU passthrough, Coral TPU setup
- 💾 **Storage Management** - Disk passthrough, import disk images
- 🌍 **Network Tools** - Network repair and configuration utilities
- 📊 **ProxMenux Monitor** - Web dashboard on port 8008
- 🔄 **Auto-updates** - Built-in update mechanism

---

## 📌 Installation

Run this command in your Proxmox server terminal:

```bash
bash -c "$(wget -qLO - https://raw.githubusercontent.com/nickdesi/proxmenux/main/install_proxmenux.sh)"
```

> ⚠️ Always review scripts before executing them from the internet.

---

## 📌 Usage

Once installed, launch **ProxMenux** by running:

```bash
menu
```

---

## 📌 System Requirements

**Compatible with:**

- Proxmox VE 8.x and 9.x

**Dependencies (auto-installed):**

- `bash`, `curl`, `wget`, `jq`, `dialog`
- `python3-venv` (for translation support)

---

## 🌐 Supported Languages

| Language | File |
|----------|------|
| 🇬🇧 English | `en.lang` |
| 🇪🇸 Spanish | `es.lang` |
| 🇫🇷 French | `fr.lang` |

---

## 🏗️ Architecture

```
ProxMenux/
├── install_proxmenux.sh    # Main installer
├── menu                    # Entry point script
├── scripts/
│   ├── utils.sh           # Core utilities (translation, UI helpers)
│   ├── menus/             # Menu scripts
│   └── ...                # Feature scripts
├── lang/                   # Language files
└── web/                    # Web dashboard (Next.js)
```

---

## 🤝 Contributing

Contributions are welcome! Feel free to open issues or submit pull requests.

---

## 📄 License

This project is licensed under [CC BY-NC 4.0](LICENSE).
