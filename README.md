# quickshell-git (Prebuilt Arch Package)

Prebuilt Arch Linux package for Quickshell, built automatically from upstream Git and published via GitHub Releases.

No AUR.  
No pacman repo.  
No manual builds.

---

## 📦 Package

| Package | Description |
|----------|------------|
| quickshell-git | Flexible toolkit for building desktop shells with QtQuick |

Builds include:

- x86_64_v3 optimized builds (preferred)
- Built from latest upstream Git
- Automatically released via GitHub Actions

---

# 🚀 Install / Update

```bash
curl -fLO https://raw.githubusercontent.com/Ravi-Kishor/quickshell-git/main/update-quickshell
chmod +x update-quickshell
sudo mv update-quickshell /usr/local/bin/update-quickshell
update-quickshell
```

---

## 🧠 What the updater does

- Checks installed version via pacman
- Fetches latest GitHub release
- Prefers x86_64_v3 build
- Falls back to generic x86_64
- Downloads and installs automatically

Interactive mode:
- Update only if newer
- Force reinstall

---

## 🏗 Build Info

- Built inside Arch container
- Stripped binaries
- x86_64_v3 builds include AVX/FMA support
- Provides: `quickshell`
- Conflicts with: `quickshell`

---

## ⚠ Requirements

Arch Linux only.

Requires:

- pacman
- curl
- jq
- sudo
