# NetLock

**Per-app internet firewall.** Choose which apps may use the internet: each app gets its own switch, and blocked
apps can't reach the network. No account, no ads, no analytics. NetLock collects no data.

This repository only holds the **downloads**. Get the latest version from
**[Releases](https://github.com/iamanwaralam/netlock-releases/releases/latest)**.

| Platform | Status |
|---|---|
| **Linux** | **Available**: `.deb`, `.rpm` and Arch package |
| Android | Coming to Google Play |
| Windows | Coming soon |
| macOS | Planned |

## Linux

**Install** the package for your distribution from the [latest release](https://github.com/iamanwaralam/netlock-releases/releases/latest):

```sh
sudo apt install ./netlock_1.0.0_amd64.deb             # Ubuntu 24.04+, Debian 13+, Kali, Mint 22+, Pop!_OS 24.04+
sudo dnf install ./netlock-1.0.0-1.x86_64.rpm          # Fedora, RHEL / Rocky / Alma 9+
sudo pacman -U ./netlock-1.0.0-1-x86_64.pkg.tar.zst     # Arch, EndeavourOS, Manjaro
```

**Use:**

1. Start **NetLock** from your app menu.
2. Tap the Internet switch next to an app, then turn the firewall **on**.
3. Enter your password once. A small engine (the systemd service `netlock-engine`) applies the rules from then on.
4. Restart the blocked app from the menu or dock. It now has no internet; your other apps keep working.

Blocking keeps working when NetLock is closed and after a reboot. Only you (and root) can change the rules.

**Requirements:** x86_64, systemd, cgroup v2, and the GNOME or KDE Plasma desktop. `nftables` and `pkexec` are
installed with the package.

**Limits:**

- On XFCE, MATE, Cinnamon and LXQt, NetLock installs but can't block. These desktops don't start each app in its
  own systemd scope.
- Apps started from a terminal aren't blocked. Start them from the menu or dock.
- Restart an app after blocking it; connections it already opened can stay up.
- No ARM build yet. Ubuntu 22.04 and Debian 12 can't install the `.deb`.

**Uninstall:** `sudo apt remove netlock`, `sudo dnf remove netlock` or `sudo pacman -R netlock`. That also removes
the engine and its firewall rules. Your list of blocked apps stays in `~/.local/share/NetLock`.

## Privacy

NetLock works only on your computer. It makes no network requests of its own, has no accounts, analytics or ads,
and doesn't inspect, log or send your traffic. Your rules stay on your computer. Privacy policy:
https://techsavvyhelp.com/netlock-privacy-policy/

## Feedback

Found a problem? [Open an issue](https://github.com/iamanwaralam/netlock-releases/issues). Please include your
distribution, your desktop (GNOME or KDE) and what happened.

© 2026 TechSavvyHelp. NetLock is free to use.
