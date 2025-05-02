# 🐧 openSUSE Tumbleweed on WSL

A simple guide to install and uninstall **openSUSE Tumbleweed** on **Windows Subsystem for Linux (WSL)**.


## 📝 Prerequisites

- ✅ Windows 10 (Build 19041+) or **Windows 11**
- ✅ **WSL enabled** (WSL 2 recommended)

To check your WSL version:
```powershell
wsl --status
````

If WSL is not installed:

```powershell
wsl --install
```

---

## 📥 Installing openSUSE Tumbleweed

### Step 1: Open PowerShell as Administrator

```powershell
wsl --install openSUSE-Tumbleweed
```

### Step 2: Set Up

* The system will download and install openSUSE Tumbleweed.
* When prompted, create your UNIX username and password.

---

## 🚀 Launch openSUSE Tumbleweed

To start the distro at any time:

```powershell
wsl -d openSUSE-Tumbleweed
```

---

## 🔧 Post-Installation Setup

Update the system and install common tools:

```bash
sudo zypper refresh
sudo zypper update
sudo zypper install git curl vim
```

---

## ❌ Uninstall openSUSE Tumbleweed

To **completely remove** openSUSE Tumbleweed from WSL:

```powershell
wsl --unregister openSUSE-Tumbleweed
```

> ⚠️ This action is **irreversible** and will delete all data inside the distro.

---

## 📚 Resources

* [openSUSE on WSL](https://en.opensuse.org/WSL)
* [Microsoft WSL Documentation](https://learn.microsoft.com/en-us/windows/wsl/)

```
