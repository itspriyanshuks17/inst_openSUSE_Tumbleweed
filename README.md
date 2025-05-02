# 🐧 openSUSE Tumbleweed on WSL

A simple guide to install, use, and uninstall **openSUSE Tumbleweed** on **Windows Subsystem for Linux (WSL)**.

---

## 📝 Prerequisites

- **Windows 10 (Build 19041+)** or **Windows 11**
- **WSL enabled** (WSL 2 is recommended)

To verify your WSL setup, run:
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

Run the following command:

```powershell
wsl --install openSUSE-Tumbleweed
```

### Step 2: Set Up

* The system will download and install openSUSE Tumbleweed.
* When prompted, create your UNIX username and password.

---

## 🚀 Launch openSUSE Tumbleweed

To start the distribution at any time:

```powershell
wsl -d openSUSE-Tumbleweed
```

---

## 🔧 Post-Installation Setup

After launching, update the system and install commonly used tools:

```bash
sudo zypper refresh
sudo zypper update
sudo zypper install git curl vim
```

---

## 🔍 Finding and Installing Packages

openSUSE uses **zypper** as its package manager. Here's how you can manage packages:

### Searching for Packages

To search for a package, use:

```bash
sudo zypper search <package_name>
```

Example:

```bash
sudo zypper search python3
```

### Installing Packages

To install a package, use:

```bash
sudo zypper install <package_name>
```

Example:

```bash
sudo zypper install htop
```

### Viewing Package Information

For detailed information about a package, run:

```bash
sudo zypper info <package_name>
```

---

## ❌ Uninstall openSUSE Tumbleweed

To completely remove openSUSE Tumbleweed from WSL, run:

```powershell
wsl --unregister openSUSE-Tumbleweed
```

> ⚠️ **Warning:** This action is irreversible and will delete all data contained in the distro.

---

## 📚 Resources

* [openSUSE on WSL](https://en.opensuse.org/WSL)
* [Microsoft WSL Documentation](https://learn.microsoft.com/en-us/windows/wsl/)

