# World Tivi — downloads

World Tivi is a simple, fast IPTV player. Add your own M3U playlist, Xtream Codes account or Stalker portal and
watch with the remote, the keyboard or the mouse. World Tivi does not provide any channels or content.

This repository only hosts the desktop downloads. Website: https://worldtivi.vercel.app/

## Desktop apps

Get the files from the [latest release](https://github.com/ptrinh/worldtivi-public/releases/latest):

| Platform | File |
|---|---|
| macOS 11+ (Apple silicon and Intel, one app) | `WorldTivi-<version>-mac-universal.dmg` |
| Windows 10/11 x64 | `WorldTivi-<version>-windows-setup.exe` |
| Windows on Arm (Arm64) | `WorldTivi-<version>-windows-arm64-setup.exe` |
| Linux x64: Debian, Ubuntu and derivatives | `worldtivi_<version>_amd64.deb` |
| Linux x64: any distribution | `WorldTivi-<version>-linux-x86_64.AppImage` |
| Linux Arm64: Debian, Ubuntu and derivatives | `worldtivi_<version>_arm64.deb` |
| Linux Arm64: any distribution | `WorldTivi-<version>-linux-aarch64.AppImage` |

- The macOS app is signed with Developer ID (SENPRINTS LLC) and notarized by Apple.
- The Windows installers are signed by SENPRINTS LLC.
- `SHA256SUMS` in each release lists the checksums of its files.

## Install with a package manager

**macOS (Homebrew)**

```sh
brew install --cask ptrinh/tap/worldtivi
```

**Windows (winget)**, once the package is accepted into the winget repository:

```powershell
winget install SENPRINTS.WorldTivi
```

**Windows (Chocolatey)**, once the package is approved on chocolatey.org:

```powershell
choco install worldtivi
```

**Debian, Ubuntu and derivatives (apt)**: add the World Tivi repository once, then updates come with `apt upgrade` (amd64 and arm64).

```sh
curl -fsSL https://dl.trinh.uk/apt/worldtivi.gpg | sudo tee /usr/share/keyrings/worldtivi.gpg >/dev/null
echo "deb [signed-by=/usr/share/keyrings/worldtivi.gpg] https://dl.trinh.uk/apt stable main" | sudo tee /etc/apt/sources.list.d/worldtivi.list
sudo apt update && sudo apt install world-tivi
```

The repository's signing key: `World Tivi apt repository <worldtivi@trinh.uk>`, fingerprint
`2465 50D3 DF82 5561 50CF  F86F 3111 2CAD 1026 E03D`.

## Other platforms

Android TV / Google TV, LG webOS, Samsung Tizen and Apple TV versions are listed on the website.

Versions up to 1.0.1 were macOS (two DMGs) and Windows only; from 1.0.2 the apps are much smaller and Linux is there too.

Only add playlists and streams you have the right to watch.

© SENPRINTS LLC · [Privacy policy](https://worldtivi.vercel.app/privacy/) · worldtivi@trinh.uk
