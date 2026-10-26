# 🛠️ Windows Debloater

[![Release](https://img.shields.io/github/v/release/saintberat/WinDebloat?color=blue&label=Latest%20Release)](https://github.com/saintberat/WinDebloat/releases/latest)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A modern, lightweight, and user-friendly **Windows 10/11 Debloater** application.

Easily remove pre-installed bloatware, disable telemetry and background data collection, disable Cortana, and optionally uninstall OneDrive from your system.

Built using **PowerShell + Windows Forms (GUI)**.

---

## ✨ Features

- 🗑️ **Remove Windows Bloatware:** Safely uninstall unnecessary pre-installed consumer apps.
- 🔒 **Disable Telemetry:** Turn off background tracking and telemetry services (`DiagTrack`, `dmwappushservice`).
- 🎤 **Disable Cortana:** Disable Cortana completely via Group Policy registry configurations.
- ☁️ **Remove OneDrive:** Cleanly stop and uninstall OneDrive on demand.
- ♻️ **System Restore Integration:** Create a fresh System Restore Point directly from the app before making changes.
- 📋 **Real-Time Logs:** Live execution status and feedback log viewer in the GUI.
- 🖥️ **Intuitive UI:** Clean and responsive desktop interface.
- ⚡ **Privilege Validation:** Built-in Administrator privilege checks.

---

## 📦 Supported Systems

- **Windows 10** (64-bit)
- **Windows 11** (64-bit)
- *PowerShell 5.1 or newer recommended.*

---

## 🚀 Usage

1. **Download** the latest [**`Debloater.exe`**](https://github.com/saintberat/WinDebloat/releases/latest/download/Debloater.exe) from the [Releases](https://github.com/saintberat/WinDebloat/releases/latest) page.
2. **Run as Administrator:** Right-click and choose **Run as administrator** (system modifications require elevated privileges).
3. Select the optimization tasks you wish to perform and click execute.

---

## 🔍 Capabilities

### 🗑️ Bloatware Removal

Removes pre-installed UWP/AppX packages, including:

- 3D Builder
- Bing Finance, News, Sports & Weather
- Office Hub & OneNote
- Skype
- Windows Maps & Alarms
- Feedback Hub
- Xbox applications
- Groove Music, Movies & TV
- And other non-essential consumer packages

---

### 🔒 Telemetry & Diagnostics

Applies the following optimizations:

- Sets `AllowTelemetry` policy to disabled (`0`).
- Stops and disables the `DiagTrack` (Connected User Experiences and Telemetry) service.
- Stops and disables the `dmwappushservice` service.

---

### 🎤 Cortana

Disables Cortana by setting the `AllowCortana` registry key under `HKLM\SOFTWARE\Policies\Microsoft\Windows\Windows Search`.

---

### ☁️ OneDrive

- Terminates active `OneDrive.exe` processes.
- Executes the official OneDrive uninstaller silently and cleans up residue folders.

---

### ♻️ System Restore

Enables you to create an automatic System Restore Point with a single click before initiating any debloating process.

---

## ⚠️ Important Notes & Recommendations

This tool modifies system settings and removes applications:

- It is strongly recommended to **create a System Restore Point** before running optimizations.
- Back up critical work and personal files.
- Some changes will only take full effect after a **system reboot**.

---

## 🛠️ Tech Stack

- **PowerShell**
- **Windows Forms (.NET Framework)**
- **Windows Registry APIs**
- **AppX / Dism Package Management APIs**

---

## 📄 License

Distributed under the **MIT License**. Free for personal and educational use.

---

## 🤝 Contributing

Contributions, bug reports, and feature suggestions are welcome! Feel free to open an **Issue** or submit a **Pull Request**.

---

## ⭐ Support

If you found this tool useful, consider giving the repository a **Star** (⭐)!

<!-- sync-activity: 2026-10-26T17:06:12Z (8a478a22) -->
