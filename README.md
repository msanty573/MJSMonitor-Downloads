# OmniMonitor downloads

Installers for **OmniMonitor** by [MJS Applications](https://mjsapps.net) — watch your servers,
services and websites: red, yellow or green at a glance, with alerts when something goes down. This repository holds downloads only; the
source code is not here.

**Easiest:** <https://mjsapps.net/omnimonitor/> recommends the right file for your computer.

**All files:** <https://github.com/msanty573/OmniMonitor-Downloads/releases/tag/latest> (the
release notes list which version each file is).

| Computer | File |
|---|---|
| Mac with Apple silicon (M1 or newer) | [OmniMonitor-macOS-arm64.dmg](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-macOS-arm64.dmg) |
| Mac with an Intel processor | [OmniMonitor-macOS-x86_64.dmg](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-macOS-x86_64.dmg) |
| Windows (Intel or AMD) — installer | [OmniMonitor-Setup-x64.exe](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-Setup-x64.exe) |
| Windows (Intel or AMD) — portable zip | [OmniMonitor-windows-x64-portable.zip](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-windows-x64-portable.zip) |
| Windows on ARM — installer | [OmniMonitor-Setup-arm64.exe](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-Setup-arm64.exe) |
| Windows on ARM — portable zip | [OmniMonitor-windows-arm64-portable.zip](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-windows-arm64-portable.zip) |
| Linux (Intel or AMD) — tar.gz | [OmniMonitor-linux-x86_64.tar.gz](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-linux-x86_64.tar.gz) |
| Linux (Intel or AMD) — RPM (RHEL, AlmaLinux, Rocky, Fedora) | [omnimonitor.el10.x86_64.rpm](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/omnimonitor.el10.x86_64.rpm) |
| Linux (Intel or AMD) — .deb (Ubuntu 26.04+) | [omnimonitor.ubuntu.amd64.deb](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/omnimonitor.ubuntu.amd64.deb) |
| Linux on ARM — tar.gz | [OmniMonitor-linux-aarch64.tar.gz](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/OmniMonitor-linux-aarch64.tar.gz) |
| Linux on ARM — RPM | [omnimonitor.el10.aarch64.rpm](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/omnimonitor.el10.aarch64.rpm) |
| Linux on ARM — .deb (Ubuntu 26.04+) | [omnimonitor.ubuntu.arm64.deb](https://github.com/msanty573/OmniMonitor-Downloads/releases/download/latest/omnimonitor.ubuntu.arm64.deb) |

**System requirements:** macOS 12 Monterey or newer · 64-bit Windows 10 or 11 (Windows 11
on ARM PCs) · 64-bit Linux. No administrator rights needed. Only scan and monitor networks
you own or have permission to monitor.

## First launch

OmniMonitor isn't signed with a paid Apple or Microsoft developer certificate yet, so the
first launch shows a warning:

- **Mac:** open the .dmg and drag OmniMonitor to Applications. The first time you open it,
  macOS says it can't verify the app — click **Done**, then go to **System Settings →
  Privacy & Security**, scroll down and click **Open Anyway**. (On macOS 12–14 you can
  also Control-click OmniMonitor, choose **Open**, then **Open** again.)
- **Windows:** if SmartScreen says "Windows protected your PC", click **More info →
  Run anyway**.
- **Linux:** install the .deb (`sudo apt install ./omnimonitor.ubuntu.*.deb`, which also sets
  up updates through apt) or the RPM (`sudo dnf install ./omnimonitor.el10.*.rpm`), or extract
  the tar.gz and run `./install.sh`. To get RPM updates through dnf, add the repository once:

  ```
  sudo rpm --import https://msanty573.github.io/OmniMonitor-Downloads/RPM-GPG-KEY-omnimonitor
  sudo curl -o /etc/yum.repos.d/omnimonitor.repo https://msanty573.github.io/OmniMonitor-Downloads/omnimonitor.repo
  ```

## Updates

**Help → Check for Updates…** finds and installs new versions; the .deb (and the RPM, once
its repository is added) also updates with your system's other updates.

## Security

Found a security problem? Please report it privately — see [SECURITY.md](SECURITY.md).
