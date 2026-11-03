<p align="center">
  <img src="images/icon.png" width="112" alt="Netcurb icon">
</p>

<h1 align="center">Netcurb</h1>

<p align="center">
  <b>Per-app internet firewall.</b> One switch per app: blocked apps can't reach the internet.<br>
  No account · no ads · no analytics · no data collected
</p>

<p align="center">
  <a href="https://github.com/iamanwaralam/netcurb-releases/releases/latest"><img alt="Latest release" src="https://img.shields.io/github/v/release/iamanwaralam/netcurb-releases?label=latest&color=2952CC"></a>
  <a href="https://github.com/iamanwaralam/netcurb-releases/releases"><img alt="Downloads" src="https://img.shields.io/github/downloads/iamanwaralam/netcurb-releases/total?color=2952CC"></a>
  <img alt="Linux" src="https://img.shields.io/badge/Linux-deb%20%7C%20rpm%20%7C%20Arch-2952CC">
</p>

<p align="center">
  <img src="images/hero.png" alt="Netcurb for Linux: app list with three apps blocked, app details, and dark mode">
</p>

## Download

| Distribution | Package |
|---|---|
| Ubuntu 24.04+, Debian 13+, Kali, Linux Mint 22+, Pop!_OS 24.04+ | [**netcurb_1.1.0_amd64.deb**](https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/netcurb_1.1.0_amd64.deb) |
| Fedora, RHEL / Rocky / Alma 9+ | [**netcurb-1.1.0-1.x86_64.rpm**](https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/netcurb-1.1.0-1.x86_64.rpm) |
| Arch, Manjaro, EndeavourOS | [**netcurb-1.1.0-1-x86_64.pkg.tar.zst**](https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/netcurb-1.1.0-1-x86_64.pkg.tar.zst) |

All versions and checksums: [Releases](https://github.com/iamanwaralam/netcurb-releases/releases).
**Android** is coming to Google Play, **Windows** soon, and **macOS** later.

## Features

- 🧱 **One switch per app.** Block or allow internet access for each app you have installed.
- 🖥️ **Your real apps, with icons.** Every app in your menu, including Snap and Flatpak. System tools are listed separately.
- 🔒 **Stays on.** Blocking keeps working when Netcurb is closed and after a reboot.
- 👤 **Only you change the rules.** Other users on the same computer can't unblock your apps.
- 🌙 **Light and dark theme**, plus search and filters (user apps, blocked, system).
- 🧹 **Clean uninstall.** Removing Netcurb also removes its firewall rules and background service.
- 🕵️ **Private.** Netcurb makes no network requests of its own and never inspects your traffic.

## Screenshots

| App list | App details | Settings | Dark mode |
|:-:|:-:|:-:|:-:|
| <img src="images/app-list.png" width="200" alt="App list"> | <img src="images/app-detail.png" width="200" alt="App details"> | <img src="images/settings.png" width="200" alt="Settings"> | <img src="images/app-list-dark.png" width="200" alt="Dark mode"> |

## Install

Open a terminal (<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>T</kbd> on most desktops) and follow the steps for your
distribution. Each step is one command: copy it, paste it into the terminal, press <kbd>Enter</kbd>.

<details open>
<summary><b>Ubuntu, Debian, Kali, Linux Mint, Pop!_OS</b> (.deb)</summary>

1. Go to your Downloads folder:
   ```sh
   cd ~/Downloads
   ```
2. Download Netcurb:
   ```sh
   wget https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/netcurb_1.1.0_amd64.deb
   ```
3. *(Optional)* Check the download. It should print `netcurb_1.1.0_amd64.deb: OK`:
   ```sh
   wget -q https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/SHA256SUMS
   sha256sum -c SHA256SUMS --ignore-missing
   ```
4. Install it (enter your password when asked, then press <kbd>Y</kbd> if apt asks to continue):
   ```sh
   sudo apt install ./netcurb_1.1.0_amd64.deb
   ```
   Keep the `./` in front of the file name, so apt installs this file instead of searching online.
5. Open **Netcurb** from your app menu.

</details>

<details>
<summary><b>Fedora, RHEL, Rocky Linux, AlmaLinux</b> (.rpm)</summary>

1. Go to your Downloads folder:
   ```sh
   cd ~/Downloads
   ```
2. Download Netcurb:
   ```sh
   curl -LO https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/netcurb-1.1.0-1.x86_64.rpm
   ```
3. *(Optional)* Check the download. It should print `netcurb-1.1.0-1.x86_64.rpm: OK`:
   ```sh
   curl -LO https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/SHA256SUMS
   sha256sum -c SHA256SUMS --ignore-missing
   ```
4. Install it (enter your password when asked, then press <kbd>Y</kbd> to confirm):
   ```sh
   sudo dnf install ./netcurb-1.1.0-1.x86_64.rpm
   ```
5. Open **Netcurb** from your app menu.

</details>

<details>
<summary><b>Arch Linux, Manjaro, EndeavourOS</b> (.pkg.tar.zst)</summary>

1. Go to your Downloads folder:
   ```sh
   cd ~/Downloads
   ```
2. Download Netcurb:
   ```sh
   curl -LO https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/netcurb-1.1.0-1-x86_64.pkg.tar.zst
   ```
3. *(Optional)* Check the download. It should print `netcurb-1.1.0-1-x86_64.pkg.tar.zst: OK`:
   ```sh
   curl -LO https://github.com/iamanwaralam/netcurb-releases/releases/download/linux-v1.1.0/SHA256SUMS
   sha256sum -c SHA256SUMS --ignore-missing
   ```
4. Install it (enter your password when asked, then press <kbd>Y</kbd> to confirm):
   ```sh
   sudo pacman -U ./netcurb-1.1.0-1-x86_64.pkg.tar.zst
   ```
5. Open **Netcurb** from your app menu.

</details>

**Upgrading from NetLock?** Install Netcurb the same way. It replaces NetLock automatically (on Arch, answer
<kbd>Y</kbd> when pacman asks to remove `netlock`). Your blocked apps carry over; open Netcurb and turn the firewall on
once more.

**Updating to a newer Netcurb:** download the new package from [Releases](https://github.com/iamanwaralam/netcurb-releases/releases)
and install it with the same command as above.

## How to use

1. Open **Netcurb** from your app menu.
2. Tap the switch next to an app so it turns red, then turn the firewall **on**.
3. Enter your password **once**. A small background service applies your rules from then on.
4. Close the app you blocked and open it again **from the menu or dock**. It now has no internet; everything else
   works as before.

To allow an app again, tap its switch, or turn the firewall off.

## Requirements

- x86_64 PC with **systemd** and **cgroup v2** (standard on current distributions)
- **GNOME** or **KDE Plasma** desktop, on X11 or Wayland
- `nftables` and `pkexec` (installed automatically with the package)

## Good to know

- **Restart an app after blocking it.** Connections it already opened can stay up until then.
- **Start blocked apps from the menu or dock.** Apps started from a terminal aren't blocked.
- **XFCE, MATE, Cinnamon and LXQt** aren't supported yet. Netcurb installs there, but it can't block apps.
- **Not available yet:** an ARM build, and packages for Ubuntu 22.04 or Debian 12.

## Uninstall

Run the command for your distribution in a terminal:

| Distribution | Command |
|---|---|
| Ubuntu, Debian, Kali, Mint, Pop!_OS | `sudo apt remove netcurb` |
| Fedora, RHEL, Rocky, Alma | `sudo dnf remove netcurb` |
| Arch, Manjaro, EndeavourOS | `sudo pacman -R netcurb` |

This also removes Netcurb's background service and firewall rules. Your list of blocked apps is kept in
`~/.local/share/Netcurb`. To remove it too:

```sh
rm -rf ~/.local/share/Netcurb
```

## Privacy

Netcurb works entirely on your computer. It has no accounts, analytics or ads, makes no network requests of its own,
and doesn't inspect, log or send your traffic. Read the
[privacy policy](https://techsavvyhelp.com/netcurb-privacy-policy/).

## Feedback

Found a bug or have an idea? [Open an issue](https://github.com/iamanwaralam/netcurb-releases/issues). Please include
your distribution, your desktop (GNOME or KDE) and what happened.

---

<sub>© 2026 TechSavvyHelp. Netcurb is free to use. Screenshots show example apps.</sub>
