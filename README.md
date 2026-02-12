# quickkshell-git (Prebuilt Arch Packages)

Prebuilt Arch Linux packages built automatically via GitHub Actions.

Includes:

- quickshell-git
- dms-shell-git
- x86_64
- x86_64_v3 optimized builds

---

## 📦 Packages

| Package | Description |
|----------|------------|
| quickshell-git | QtQuick-based desktop shell toolkit |
| dms-shell-git  | DankMaterialShell (Core + Shell) |

Both packages:

- Built from latest upstream Git
- Automatically released
- Provide x86_64_v3 optimized binaries (preferred)
- Fallback to generic x86_64 if needed

---

# 🚀 Install / Update

---

## Update quickshell-git

```bash
curl -fLO https://raw.githubusercontent.com/Ravi-Kishor/quickkshell-git/main/update-quickshell
chmod +x update-quickshell
sudo mv update-quickshell /usr/local/bin/update-quickshell
update-quickshell
```

---

## Update dms-shell-git

```bash
curl -fLO https://raw.githubusercontent.com/Ravi-Kishor/quickkshell-git/main/update-dms
chmod +x update-dms
sudo mv update-dms /usr/local/bin/update-dms
update-dms
```

---

## 🧠 What the updater does

- Checks installed version via pacman
- Fetches latest GitHub release
- Prefers x86_64_v3
- Falls back to generic x86_64
- Downloads and installs automatically

Interactive mode:
- Update only if newer
- Force reinstall

---

## 🏗 Build Info

- Built inside Arch container
- Stripped binaries
- Optimized for performance
- x86_64_v3 builds include AVX/FMA support

---

## ⚠ Requirements

Arch Linux only.

Requires:

- pacman
- curl
- jq
- sudo
