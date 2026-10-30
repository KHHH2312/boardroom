<div align="center">

<img src="docs/icon.png" width="84" alt="Boardroom">

# Boardroom

### An infinite blueprint room for plans that stay on your machine.

A local-first whiteboard with real tools, undo and PNG/JSON export.

[![Download for Windows](https://img.shields.io/badge/Download-Windows%20x64-0D2233?style=for-the-badge&logo=windows11&logoColor=white)](https://github.com/KHHH2312/boardroom/releases/latest)
[![Latest release](https://img.shields.io/github/v/release/KHHH2312/boardroom?style=flat-square&color=0D2233)](https://github.com/KHHH2312/boardroom/releases)
[![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11%20x64-EDE7DA?style=flat-square)](#requirements)
[![License](https://img.shields.io/badge/license-MIT-EDE7DA?style=flat-square)](LICENSE)

<img src="docs/boardroom-desk.png" alt="Boardroom" width="100%">

</div>

> **New — 1.15.0** — bring to front and send to back, image fit, alignment guides and SVG export.
> [Changelog →](CHANGELOG.md)

---

## Why Boardroom

**Plans are private.** A whiteboard that uploads every stroke is a meeting you did not consent to.

**A blueprint room is a place, not a form.** The tool rail and canvas carry the whole interaction.

**JSON export means the board survives the app.**

## Features

| | |
|---|---|
| **Infinite blueprint** | 32-unit snapping, pan, zoom-to-cursor and fit-to-plan. |
| **Real tools** | Select, rectangle, ellipse, arrow, line, freehand, text, sticky note, hand. |
| **Selection** | Move, corner-resize, align the group, lock a mark against edits (Ctrl+L), duplicate, delete and z-order. |
| **Find text** | Ctrl+F searches every text and sticky note on the plan; a hit selects the mark and centres the view. |
| **Style rail** | Chalk and fill palettes, stroke widths, opacity and type size. |
| **History** | Fifty undo steps, redo, and keyboard-first shortcuts. |
| **Boards library** | Search, templates (Retro, Kanban, Wireframe), duplicate and delete; autosaved JSON. |
| **Images** | Place, paste or drop PNG, JPEG and WebP images onto the plan. |
| **Export** | PNG for sharing (Shift-click exports the selection), JSON for keeping the scene editable. |
| **Local only** | Loopback server, strict CSP, no account and no telemetry. |
| **SVG export** | Export the plan or a selection as a true vector file with text, shapes and embedded images. |
| **Alignment guides** | Drag near another mark’s edge or centre with grid snap off to see a guide and land exactly on it. |
| **Image fit** | Switch a placed image between cover (crop to frame) and contain (whole image inside the frame). |
| **Stack order** | Bring a mark to the front or send it to the back in one click, alongside one-step forward and back. |

<div align="center">
<img src="docs/boardroom-draw.png" alt="Boardroom" width="49%">
<img src="docs/boardroom-library.png" alt="Boardroom" width="49%">
<img src="docs/boardroom-plan.png" alt="Boardroom" width="49%">
</div>

## Requirements

- Windows 10 or 11, x64
- No account, no runtime install

## Install

1. Download **Boardroom-1.15.0-win32-x64.zip** from [Releases](https://github.com/KHHH2312/boardroom/releases/latest).
2. Verify it against `SHA256SUMS.txt`:
   ```powershell
   Get-FileHash .\Boardroom-*-win32-x64.zip -Algorithm SHA256
   ```
3. `FILEMANIFEST.txt` lists the SHA-256 and size of every file in the archive — diff it against what you unpacked.
4. Unzip anywhere and run **Boardroom.exe**.

> Self-signed development certificate: SmartScreen will warn until an OV/EV certificate is used.
> The SHA-256 checksum is the trust anchor.

## Using it

1. Install and launch Boardroom.
2. Open the library and start a new plan.
3. Pick a tool (or shortcut V/R/O/A/L/P/T/N) and draw.
4. Undo/redo with Ctrl+Z / Ctrl+Shift+Z; export PNG or JSON from the top bar.

## Verified

- Model/server suite: 64 checks green.
- Browser golden path: 51 checks green — stack order, image fit, guides, SVG export, locked marks, plan-wide find and backup/restore.
- Packaged app passes the source-parity integrity gate and ships with SHA-256 sums and a per-file manifest.

## Security and privacy

- Local-first: the app runs on loopback, stores data on your machine and sends no telemetry.
- Strict renderer policy, sandboxed window, denied navigation/window-open by default.
- Releases are integrity-gated, signed and published with SHA-256 sums and a per-file manifest.
- Found a flaw? Open a private security advisory instead of a public issue.

## FAQ

**Does it need an account?** No.

**Where is my data?** In the app's local data folder, not on a server.

**Why is the source not in this repository?** This repository distributes the application and its
documentation. The source is private.

## License

MIT — see [LICENSE](LICENSE). Third-party components in [THIRD-PARTY.md](THIRD-PARTY.md).

---

## The rest of the desk

Five local-first tools, one philosophy: your files, your machine, no telemetry.

- **Pressroom** — [deck studio](https://github.com/KHHH2312/pressroom)
- **Folio** — [PDF bindery](https://github.com/KHHH2312/folio)
- **Relay** — [API client](https://github.com/KHHH2312/relay)
- **Slate** — [markdown notebook](https://github.com/KHHH2312/slate)
- **Boardroom** — [whiteboard](https://github.com/KHHH2312/boardroom)
