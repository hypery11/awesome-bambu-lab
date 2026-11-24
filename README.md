# Awesome Bambu Lab [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

![Awesome Bambu Lab](assets/banner.png)

[![Entries](https://img.shields.io/badge/entries-244-blue)](#contents) [![Last updated](https://img.shields.io/badge/last_updated-2026--11--24-brightgreen)](https://github.com/hypery11/awesome-bambu-lab/commits/main/) [![License: CC0-1.0](https://img.shields.io/badge/license-CC0--1.0-lightgrey)](LICENSE) [![Link check](https://github.com/hypery11/awesome-bambu-lab/actions/workflows/links.yml/badge.svg)](https://github.com/hypery11/awesome-bambu-lab/actions/workflows/links.yml)

English | [繁體中文](README.zh-TW.md)

> A curated map of the open-source ecosystem around Bambu Lab 3D printers: LAN control, Home Assistant, firmware, slicers, farms, filament and cameras.

**Status:** Curated 2026-10. Contributions welcome.

**Disclaimer:** Unofficial, not affiliated with Bambu Lab. Custom firmware and hardware mods **may void your warranty** and can damage hardware; some firmware projects have licensing questions, check each project's license yourself. Use at your own risk.

---

## Start here

The projects people actually share. Everything below is the map around them, not a product catalog.

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — Community custom firmware for the X1 / X1 Carbon.
- **[bambuddy](https://github.com/maziggy/bambuddy)** — Self-hosted, cloud-free command center for Bambu printers.
- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — Home Assistant integration for Bambu Lab printers.
- **[OpenBambuAPI](https://github.com/Doridian/OpenBambuAPI)** — Community documentation of the Bambu printer APIs.
- **[RFID-Tag-Guide](https://github.com/Bambu-Research-Group/RFID-Tag-Guide)** — How to read Bambu filament NFC/RFID tags.

---

## New this week

Added between 2026-11-18 and 2026-11-24 (derived from git history).

- **[Bambu Controller](https://github.com/mrquentin/bambu-controller)** — Small self-hosted web app to monitor and control Bambu Lab printers in LAN-only mode with local accounts: SSDP discovery, live camera (JPEG or RTSPS via ffmpeg), temperatures, fans, lights, speed levels, jog and pause/resume/stop, AMS load/unload, HMS alerts, an FTPS storage browser to start prints from a `.3mf`, and a G-code console; protocol notes recovered from the LanBu Android app. _(LAN mode, APIs & libraries)_
- **[bambu-lan-plugin-aarch64](https://github.com/cyrinux/bambu-lan-plugin-aarch64)** — Unofficial open-source native aarch64 reimplementation of the LAN part of Bambu's closed, x86-64-only networking plugins (`libbambu_networking.so`, `libBambuSource.so`), so Bambu Studio and OrcaSlicer on arm64 Linux get discovery, the Device tab, LAN printing and the live camera; printers must be in LAN-only mode with Developer Mode, and only the A1 is tested so far. _(LAN mode, APIs & libraries)_
- **[Orcbro](https://github.com/blankkit/orcbro)** — Self-hosted container that bridges Bambu Lab printers in LAN mode to Bambro, an iOS app, over a simple HTTPS/JSON API: status and control over MQTT, slicing STL, OBJ, STEP and 3MF with the OrcaSlicer CLI and official Bambu profiles, and printing, with no Bambu cloud account. _(LAN mode, APIs & libraries)_
- **[null-bambu-cli](https://github.com/GOROman/null-bambu-cli)** — Python CLI (`nbc`) for Bambu Lab printers that are *not* in LAN Only Mode: SSDP discovery with certificate-fingerprint pinning, status and AMS/spool filament over local MQTT, and listing, uploading or deleting sliced files on internal or external storage over the local network. _(LAN mode, APIs & libraries)_
- **[Bambu Lab Cards (CzechTropi)](https://github.com/CzechTropi/bambulab-card)** — Three minimalist HACS dashboard cards built on ha-bambulab: a printer card (camera, progress, temperatures, errors), an AMS card styled like Bambu Studio and an external-spool card, all configurable in the visual editor, with a mock data source for trying them without a printer. _(Home Assistant & automation)_
- **[Bambu Filament Manager (Trunks1982)](https://github.com/Trunks1982/ha-bambu-filament-manager)** — HACS spool inventory for Bambu printers in Home Assistant, running on ha-bambulab: an AMS card styled like Bambu Studio, NFC stickers with one-tap slot loading, live usage tracking, AMS drying and humidity warnings, per-print costs and notifications; sending to the AMS needs LAN mode with Developer Mode. _(Home Assistant & automation)_
- **[BamButton-IDF](https://github.com/FLsmaier/BamButton-IDF)** — Pure ESP-IDF port of Bambutton for an ESP32-C3 Super Mini: a physical button that polls Bambuddy, flashes its LED while the printer waits for the plate to be cleared, and sends the plate-clear through the Bambuddy API when pressed; setup via the board's own access point. _(Firmware & hardware mods)_
- **[MakerWorld Settings Importer for OrcaSlicer](https://github.com/FleeceFlames/Orca_makerworld_importer)** — OrcaSlicer 2.5+ Python plugin that converts a MakerWorld `.3mf` (usually sliced for Bambu printers) to your currently active printer, overlaying only the creator's compatible process settings on your own printer, plate and filament presets, and writing a change log. _(Slicers, profiles & G-code)_
- **[bambu-slice-mcp](https://github.com/ZHT0711/bambu-slice-mcp)** — MCP server that runs Bambu Studio / OrcaSlicer's own slicing engine headlessly through the CLI and sweeps a setting (layer height, support threshold, infill…) to report measured print time and filament use per variant; also flattens the preset inheritance chains the CLI ignores. _(Slicers, profiles & G-code)_
- **[NoCali](https://github.com/HanSur94/nocali)** — Small local web page for the X1 Carbon / X1 that removes the vibration (resonance) calibration from a sliced file, opens the cleaned file in Bambu Connect to print, and shows the printer live (progress, temperatures, fans, AMS filaments, HMS errors in plain text, camera); the printer stays in normal cloud mode. _(Slicers, profiles & G-code)_

<details>
<summary>21 more added this week</summary>

- **[BatchSlicer](https://github.com/drak42/batch_slicer)** — Linux command-line tool (`pipx install batchslicer`) that slices one model or whole folders with Bambu Studio's, OrcaSlicer's or Creality Print's own CLI and the printer, filament and process presets you already have: kit parts arranged on plates, multiple copies, multi-colour 3MF filament slots filled, preview pictures added to the G-code, and a watch folder; direct sending targets Klipper and OctoPrint, not Bambu printers. _(Slicers, profiles & G-code)_
- **[EmberCheck](https://github.com/drewrobinso/embercheck)** — Local, Helio-style post-processor for Bambu Studio G-code: a per-layer thermal check with an HTML heat-map report, then slowing too-hot layers and speeding up inner walls and infill on cool ones, overhang and bridge fan fixes, missing-retraction detection and travel reordering; Windows installer, with a preview Python build for macOS and other systems. _(Slicers, profiles & G-code)_
- **[Panda Connect](https://github.com/Skaronator/panda-connect)** — Local Bambu Lab printer driver for the self-hosted Prusa Connect server, so a mixed fleet can be managed in one place: it talks to the printer directly over MQTT/TLS in LAN-only mode with no Bambu account or cloud; H3C controls are hardware-verified, other models start as read-only monitoring. _(Print farms & queues)_
- **[printfarm-planner](https://github.com/projectbin07-stack/printfarm-planner)** — Plans a production run across a mixed printer fleet (Bambu Lab P1S, A1, A1 Mini or your own models), taking operator hours, AMS, material and nozzle constraints into account, and outputs a schedule, utilisation figures and a browser Gantt chart. _(Print farms & queues)_
- **[InvenTree Bambuddy](https://github.com/nemccarthy/inventree-bambuddy)** — InvenTree plugin that prints parts through Bambuddy: link a part to its sliced file, press Print to raise a build order and stage the plates in the Bambuddy queue, then book the good parts into stock; can optionally queue prints itself when stock falls below the minimum. _(Print farms & queues)_
- **[bambu-autoeject](https://github.com/bullsrobo-boop/bambu-autoeject)** — Joins several sliced plates into one job for a Bambu Lab A1 that, after each print, cools the bed, pushes the parts off the front with the nozzle and starts the next, with no extra hardware or firmware changes; alpha, not yet tested on a real printer. _(Print farms & queues)_
- **[kanbambu](https://github.com/akilea/kanbambu)** — Self-hosted kanban (FastAPI + SQLite, Docker) for print projects: drop a .gcode.3mf to read print time, grams per colour and a preview, and track copies, plates, successes and failures with retry history; no connection to the Bambu cloud or the printer. README in French. _(Print farms & queues)_
- **[simplyusage](https://github.com/wendsell/simplyusage)** — When a Bambu print sent from Bambu Studio or Orca ends, reads the real per-colour usage from the print file and deducts it from the SimplyPrint spool in each AMS slot used, filling the gap SimplyPrint leaves for prints it did not start itself. _(Filament, AMS & RFID)_
- **[Spool Inventory](https://github.com/sfandetti/panda-command-3d-desktop)** — Local app that connects to Bambu Lab printers over your network to show what is loaded in every AMS slot and how much is left on each roll, and keeps a shelf inventory: scan Bambu rolls with a Flipper Zero and sync over USB, let rolls be added as they pass through the AMS, or add other brands by hand. _(Filament, AMS & RFID)_
- **[Bambu NFC](https://github.com/faraztp/bambu-nfc)** — macOS Python tool for the MIFARE Classic 1K RFID tags on Bambu Lab spools using a PN532 reader: diagnoses the tag, shows filament data, dumps it, and rewrites it as a standard NDEF tag (URL, text, Wi-Fi credentials or raw bytes), deriving the keys from the UID. _(Filament, AMS & RFID)_
- **[PixxelSpool](https://github.com/pixxelhoff/PixxelSpool)** — Self-hosted filament storage for Bambu Lab users on a Raspberry Pi, Mac or Windows PC: put a spool on the NFC reader (or into the AMS) to see what it is, where it belongs and how much is left; syncs with the AMS, checks print jobs and 3MF files and finds colours from a photo, with no account or cloud. In beta. _(Filament, AMS & RFID)_
- **[Bambu Filament Guard](https://github.com/parthalon025/bambu-filament-guard)** — Windows companion to Bambu Studio that, each time you slice a plate, works out how many grams of each filament the print needs (purge and prime tower included), asks the printer how much each spool has left after the running print, and warns before you print if a spool will not last. _(Filament, AMS & RFID)_
- **[bambu-bus-reference](https://github.com/heavydms/bambu-bus-reference)** — Unofficial, source-tagged reference for the RS-485 bus between a Bambu printer and its AMS units, measured on an X2D with AMS 2 Pro: framing, message types, sequences and the pins 5/6 buffer signal, with figures from logic-analyzer captures plus the ESP32-S3 bridge/parser firmware and tools used to make them. _(Filament, AMS & RFID)_
- **[PrintBot camera](https://github.com/paulnorthup/ha-printbot-camera)** — Home Assistant camera for the Bambu Lab H2S that plays the printer's 1080p/30 fps live view over WebRTC through Home Assistant's built-in go2rtc, keeping a single connection to the printer so the dashboard's HLS and WebRTC players no longer knock each other over. _(Camera & timelapse)_
- **[Pygmy](https://github.com/danderik88/pygmy)** — Self-hosted Docker app that puts LAN-only Bambu Lab and Klipper printers on your phone without the cloud: live camera, controls, notifications, spaghetti detection, one-tap printing and an MCP endpoint for agents; early preview. _(Dashboards, displays & apps)_
- **[BambuBar for Omarchy](https://github.com/tripex/omarchy-bambubar)** — Omarchy bar widget and panel showing a Bambu Lab printer's progress, time left, temperatures (both nozzles on H2D/X2D) and every AMS with spools in their real colours and humidity, plus a notification when a print ends; started as the Omarchy version of the macOS BambuBar. _(Dashboards, displays & apps)_
- **[Bambu for UltraBar Studio](https://github.com/qlerup/ultrabar-bambu)** — Bambu LAN printer widgets for the CoreBAR display, configured in UltraBar Studio on your PC, which pins each printer's TLS certificate and streams live readings and controls to the bar. _(Dashboards, displays & apps)_
- **[Bambu Monitor for Flexbar](https://github.com/UpKiry/flexbar-bambu-monitor)** — Read-only FlexDesigner plugin that shows a Bambu Lab printer's cloud status (state, job, progress, time left, layers, temperatures, AMS slots) on a Flexbar, with sign-in through a local browser page instead of LAN IP and access code; supports China and global accounts. README in Simplified Chinese. _(Dashboards, displays & apps)_
- **[BambuPresence](https://github.com/ryanpcorg/BambuPresence)** — Lightweight pure-Go desktop app that connects to a Bambu Lab printer over LAN MQTT and shows live print status as Discord Rich Presence: model image, ETA or elapsed timer, layers, temperatures, active AMS spool, HMS error decoding, plus Windows toast notifications. _(Dashboards, displays & apps)_
- **[Printvault](https://github.com/emphyri0/printvault)** — Self-hosted print archive (photos, model files, filament, print time, settings, notes, maintenance tasks) that auto-logs every Bambu print over a read-only local MQTT connection, so cloud mode keeps working; imports from MakerWorld links or sliced 3MF/G-code, and adds camera snapshots, temperature charts and HMS error codes. Only the P2S is tested on hardware, and it has no login, so keep it on a trusted network. _(Dashboards, displays & apps)_
- **[PRINT//TRACE](https://github.com/Zosuya/print-trace)** — Read-only live 3D HUD that downloads the file being printed over FTPS and redraws the G-code toolpath layer by layer in sync with the printer's MQTT reports, embeddable in the Device tab of OrcaSlicer or Bambu Studio; tested on an A1, needs an SD card in the printer. README in Traditional Chinese and English. _(Dashboards, displays & apps)_

</details>

---

## Contents

- [At a glance](#at-a-glance)
- [Official open source (bambulab)](#official-open-source-bambulab)
- [LAN mode, APIs & libraries](#lan-mode-apis--libraries)
- [Home Assistant & automation](#home-assistant--automation)
- [Firmware & hardware mods](#firmware--hardware-mods)
- [Slicers, profiles & G-code](#slicers-profiles--g-code)
- [Print farms & queues](#print-farms--queues)
- [Filament, AMS & RFID](#filament-ams--rfid)
- [Camera & timelapse](#camera--timelapse)
- [Dashboards, displays & apps](#dashboards-displays--apps)
- [Bridges & AI agents](#bridges--ai-agents)
- [Closed-source / commercial (for reference)](#closed-source--commercial-for-reference)
- [Related lists](#related-lists)
- [Contributing](#contributing)
- [License](#license)

---

## At a glance

### LAN or cloud?

Whether a tool talks to the printer on your local network or through Bambu Cloud, as stated in each project's README or docs on 2026-10-21. Bambu firmware updates can change what third-party tools may do, so check the project before relying on it.

| Project | Local network (LAN) | Bambu Cloud |
|---|---|---|
| [ha-bambulab](https://github.com/greghesp/ha-bambulab) | Yes: LAN Mode setup with printer IP and access code | Yes: the [setup docs](https://github.com/greghesp/ha-bambulab/blob/main/docs/setup.mdx) recommend cloud credentials for the most features |
| [bambuddy](https://github.com/maziggy/bambuddy) | Yes: Developer Mode, works offline | Optional: profile management through your Bambu Cloud login |
| [bambu-gateway](https://github.com/leolobato/bambu-gateway) | Yes: default mode, needs Developer Mode | Optional: experimental cloud mode |
| [PrintGlance](https://github.com/talic/PrintGlance) | Yes: read-only, over Wi-Fi with the access code | Not needed, no account |
| [bambu-connect](https://github.com/mattcar15/bambu-connect) | Yes: printer IP and access code | Not mentioned |
| [bambu-proxy](https://github.com/disconn3ct/bambu-proxy) | Yes: local MQTT relay so many clients share one printer | Not mentioned |
| [bambu-farm](https://github.com/ellenhp/bambu-farm) | Yes: built for LAN mode | Replaces it with a self-hosted service; README says not ready for general use |

## Official open source (bambulab)

- **[BambuStudio](https://github.com/bambulab/BambuStudio)** — Official slicer (open source).

## LAN mode, APIs & libraries

- **[OpenBambuAPI](https://github.com/Doridian/OpenBambuAPI)** — API documentation.
- **[bambulabs_api](https://github.com/BambuTools/bambulabs_api)** — Unofficial Python API.
- **[bambulabs_api](https://github.com/torbenconto/bambulabs_api)** — Unofficial Go bindings.
- **[bambulab](https://github.com/markhaehnel/bambulab)** — Rust API client crate.
- **[pybambu](https://github.com/greghesp/pybambu)** — Python library used by the HA integration.
- **[bambu-printer-manager](https://github.com/synman/bambu-printer-manager)** — Pure-Python printer manager library.
- **[bambu-connect](https://github.com/mattcar15/bambu-connect)** — Stats, controls and camera access.
- **[Bambu-Lab-Cloud-API](https://github.com/coelacant1/Bambu-Lab-Cloud-API)** — Analysis of the Bambu cloud API.
- **[open-bamboo-networking](https://github.com/ClusterM/open-bamboo-networking)** — Open replacement for Bambu Studio's proprietary network plugin.
- **[bambu-farm](https://github.com/ellenhp/bambu-farm)** — Self-hostable Bambu Cloud alternative.
- **[open-bambu-networking-plugin](https://github.com/persano/open-bambu-networking-plugin)** — Open-source OrcaSlicer networking plugin: cloud printing, remote liveview, AMS sync.
- **[bambu-proxy](https://github.com/disconn3ct/bambu-proxy)** — MQTT proxy that multiplexes many clients onto one Bambu printer connection.
- **[bambulab-virtual-printer](https://github.com/tbc0309/bambulab-virtual-printer)** — Local Bambu printer and AMS MQTT simulator with a web dashboard, for testing clients without a real printer.
- **[bambu-lan-cli](https://github.com/zxy8060/bambu-lan-cli)** — Experimental Python CLI for file checks, Bambu Studio CLI slicing, LAN status and signed print sending with AMS or external spool; you supply your own authorized signing identity.
- **[Bambu-A1-Skip-Object](https://github.com/TDX33029/Bambu-A1-Skip-Object)** — Desktop tool that reimplements Bambu Handy's skip-object-during-print command for the A1, reverse-engineered from the Android app, over cloud or LAN MQTT; end-to-end skipping not yet re-tested, README in Chinese.
- **[bambu.local](https://github.com/drkostas/bambu.local)** — Dependency-free Python library that talks to a printer over your own network with no cloud account: full state report and commands over MQTT, plus file upload, listing and deletion over FTPS.
- **[bambu-harness](https://github.com/Halfypoo/bambu-harness)** — Zero-dependency Node.js CLI that drives an A1 mini over LAN Only and Developer Mode: slice with OrcaSlicer, then upload and print over FTPS and MQTT, with JSON output for scripts.
- **[bambu-ctl & bambu-exporter](https://github.com/polarn/bambu)** — Go tools for the Bambu cloud: a CLI that also feeds a Waybar module, and a Prometheus exporter for Kubernetes; both use the cloud MQTT broker with your account token, so the printer stays in Cloud mode. Tested with a P2S.
- **[@printhive/bambu-models](https://github.com/PrintHive/bambu-models)** — Dependency-free TypeScript table of Bambu Lab printer models and hardware, looked up by SSDP model code, serial number or MQTT printer_type, with a source and reference for every fact.
- **[BambuLAN](https://github.com/gonzalop/bambulan)** — Go library, CLI and real-time web dashboard for cloud-free LAN management of Bambu Lab printers (status, control, camera, FTPS files), with optional Home Assistant MQTT Discovery.
- **[beambam](https://github.com/tribixbite/beambam)** — Pure-Python LAN-first stack that bridges signed MQTT for newer Bambu firmware (X2D / H2D / P2S and Jan-2025+), with a daemon, web UI, Home Assistant discovery, MCP tools and Prometheus metrics; no live cloud dependency.
- **[bambu-moonraker-shim (Shambu)](https://github.com/justinh-rahb/bambu-moonraker-shim)** — Experimental LAN bridge that presents a Bambu Lab printer as a Moonraker API so Mainsail or Fluidd can talk to it over MQTT and FTPS, without installing Klipper; developed against a P1S.
- **[bambu-lan-bridge](https://github.com/ddr56/bambu-lan-bridge)** — LAN-only Docker proxy that presents each printer as a virtual LAN-mode device and signs privileged commands with a Bambu Studio app certificate you supply, so a cloud-bound printer accepts clients like Bambu Studio, OrcaSlicer, Bambuddy or Home Assistant without Developer Mode; no Bambu account.
- **[bambu-swift](https://github.com/troglodisme/bambu-swift)** — Dependency-free Swift package that reads a printer's live status over local MQTT (job, progress, layers, temperatures, fans, filament, errors), with a small example Mac app; status only, sends no commands.
- **[Thicket](https://github.com/elitk1919/Thicket)** — Single-file Python CLI that discovers Bambu Lab printers (X1C, P1P, A1) on the local network, shows status, follows a print until it finishes, and uploads a sliced file to start, pause, resume or stop it, with no cloud account; print control needs LAN Only mode with Developer Mode.
- **[bambu-lan-connector](https://github.com/FreitasCSpace/bambu-lan-connector)** — Open-source native aarch64 replacement for Bambu Studio's closed networking and camera plugins, so the Studio flatpak on ARM64 Linux can connect to printers, send prints and show the live camera in LAN mode.
- **[bambu-lan](https://github.com/canndurmaz/bambu-lan)** — Pure-Python server and CLI that keep a Bambu printer completely offline while you watch and control it from anywhere over Tailscale: web dashboard with live camera, print control, file upload with AMS mapping, temperatures, fans and AMS status; built for the X2D, with per-model profiles for 15 Bambu printers.
- **[Bambu Controller](https://github.com/mrquentin/bambu-controller)** — Small self-hosted web app to monitor and control Bambu Lab printers in LAN-only mode with local accounts: SSDP discovery, live camera (JPEG or RTSPS via ffmpeg), temperatures, fans, lights, speed levels, jog and pause/resume/stop, AMS load/unload, HMS alerts, an FTPS storage browser to start prints from a `.3mf`, and a G-code console; protocol notes recovered from the LanBu Android app.
- **[bambu-lan-plugin-aarch64](https://github.com/cyrinux/bambu-lan-plugin-aarch64)** — Unofficial open-source native aarch64 reimplementation of the LAN part of Bambu's closed, x86-64-only networking plugins (`libbambu_networking.so`, `libBambuSource.so`), so Bambu Studio and OrcaSlicer on arm64 Linux get discovery, the Device tab, LAN printing and the live camera; printers must be in LAN-only mode with Developer Mode, and only the A1 is tested so far.
- **[Orcbro](https://github.com/blankkit/orcbro)** — Self-hosted container that bridges Bambu Lab printers in LAN mode to Bambro, an iOS app, over a simple HTTPS/JSON API: status and control over MQTT, slicing STL, OBJ, STEP and 3MF with the OrcaSlicer CLI and official Bambu profiles, and printing, with no Bambu cloud account.
- **[null-bambu-cli](https://github.com/GOROman/null-bambu-cli)** — Python CLI (`nbc`) for Bambu Lab printers that are *not* in LAN Only Mode: SSDP discovery with certificate-fingerprint pinning, status and AMS/spool filament over local MQTT, and listing, uploading or deleting sliced files on internal or external storage over the local network.

## Home Assistant & automation

- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — Home Assistant integration.
- **[ha-bambu-lab-p1-spaghetti-detection](https://github.com/nberktumer/ha-bambu-lab-p1-spaghetti-detection)** — Spaghetti detection integration.
- **[Bambu-HomeAssistant-Flows](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows)** — HA dashboards and Node-RED flows.
- **[printwatch-card](https://github.com/drkpxl/printwatch-card)** — HA dashboard card for printer monitoring.
- **[SpoolmanSync](https://github.com/gibz104/SpoolmanSync)** — Automatic Spoolman tracking via HA.
- **[HA-Panda-PWR](https://github.com/62fixolab/HA-Panda-PWR)** — Home Assistant integration for the BIGTREETECH Panda PWR smart plug.
- **[homeassistant-app-bambuddy](https://github.com/Spegeli/homeassistant-app-bambuddy)** — BamBuddy packaged as a Home Assistant App (Supervisor).
- **[ha-bambulab-blueprints](https://github.com/pleasantone/ha-bambulab-blueprints)** — Home Assistant blueprints for filter wear tracking, auto power-down, chamber heater safety and print notifications.
- **[universal-3d-cards](https://github.com/Rein033/universal-3d-cards)** — Home Assistant dashboard card for Bambu Lab and other printers, with a drawn printer, live camera and AMS spools in their real colours.
- **[3d-printdash](https://github.com/Freaky-Jay-22/3d-printdash)** — Local Home Assistant app or Docker dashboard for Bambu Lab and Klipper printers with built-in filament manager, cameras and print history.
- **[bambuddy-dragonbreath](https://github.com/rmonk/bambuddy-dragonbreath)** — Sidecar that turns a Panda Breath chamber heater (DragonBreath firmware) on and off from Bambuddy print events, picking the temperature from the filaments the print uses.
- **[bambu-dashboard-card](https://github.com/kai-wei-kfuse/bambu-dashboard-card)** — Multi-printer Home Assistant dashboard card built on ha-bambulab, with camera, controls, AMS spools and a project browser; first public release v0.1.0, still early.
- **[3D Print Cost](https://github.com/ZoziLaMalice/ha-3d-print-cost)** — Home Assistant integration that works out the electricity and filament cost of every Bambu Lab print.
- **[bambu-printer-card](https://github.com/Ergorock/bambu-printer-card)** — Lovelace card for printers in the ha-bambulab integration: live camera, progress, HMS errors, temperatures, fans, AMS and print controls, with optional smart-plug power.
- **[SpoolSync](https://github.com/Telo87/ha-spoolsync)** — Home Assistant add-on that syncs spools both ways between Spoolman and the Bambu Lab cloud filament library and books usage from print jobs; relies on the undocumented cloud API.
- **[Bambu Printer Notifications](https://github.com/dabo53ck/bambu-printer-notifications-blueprint)** — Home Assistant blueprint for the ha-bambulab integration that sends a mobile notification with a camera snapshot when a print finishes or faults, taken before the build plate lowers.
- **[Bambu Lab Printer Card](https://github.com/bitosome/3d-printer-card)** — Home Assistant Lovelace card with live camera, AMS trays, temperatures, power and electricity cost per print, plus per-print cost history.
- **[Bambu Lab for Gladys Assistant](https://github.com/guim31/gladys-bambulab)** — Gladys Assistant integration for X1, P1, A1, H2 and P2S printers over local LAN MQTT, with SSDP discovery, pause/resume, HMS errors and a dashboard widget; no cloud, not yet tested on a physical printer.
- **[Bambu Lab A1 Card](https://github.com/hudsonbrendon/bambu-a1-card)** — Animated Home Assistant Lovelace card that draws the A1 and its AMS lite, for the bambulab_local or ha-bambulab integration; installs through HACS as a custom repository.
- **[mqtt_purifier](https://github.com/3dfarmers/mqtt_purifier)** — ESP32 firmware that watches a Bambu Lab printer over local MQTT and turns a Xiaomi air purifier on for ABS / ASA prints, then off after the job ends; no cloud or Home Assistant.
- **[BambuDeck-HA](https://github.com/demonkazuya/BambuDeck-HA)** — Touchscreen deck for the 2.8" CYD (ESP32-2432S028R) that shows and controls Bambu printers through Home Assistant and ha-bambulab instead of the printer's MQTT: telemetry, cover thumbnail, AMS slots and HMS error dialogs, with web OTA.
- **[Bambu Printer Card](https://github.com/ossilampe/bambu-printer-card)** — Home Assistant card for ha-bambulab that draws the printer and up to four AMS units as one picture with live values inside, spools in their real colours, and a details view with pause / resume / stop, light and camera; English and German.
- **[ioBroker.bambulab](https://github.com/DrozmotiX/ioBroker.bambulab)** — ioBroker adapter that connects Bambu Lab printers locally with the printer's IP, access code and serial number, with no cloud involved.
- **[Bambulab2Lox](https://github.com/ricten/Bambulab2Lox)** — LoxBerry plugin that reads Bambu Lab printers over their local MQTT broker and republishes state, progress, temperatures, AMS and errors to Loxone, with optional locked-by-default commands (light, pause, resume, speed, stop); no cloud, beta tested on an H2C, README in German.
- **[AMS Graphic Card](https://github.com/spikekai/ha-ams-graphic-card)** — Home Assistant Lovelace card for the `bambu_lab` integration that draws every AMS slot as a real spool (colour, remaining filament, multi-colour segments) and highlights the tool head that is feeding; supports AMS, AMS 2 PRO, AMS HT and AMS-3H, with the model detected from device metadata.
- **[BambuDiscordStatus](https://github.com/kmoeta/BambuDiscordStatus)** — Vencord userplugin that shows a Bambu Lab printer as Discord Rich Presence, pulled live from Home Assistant (ha-bambulab) over WebSocket: print name, progress, layer, filament and time left, plus finish and failure notifications; no separate script on the PC.
- **[Filament Stock](https://github.com/matata86/filament-stock)** — HACS integration that keeps a filament stock in grams for Bambu printers in Home Assistant, deducting what each AMS slot used per print via ha-bambulab, with items from your Bambu filament profiles, barcode scanning and a dashboard card.
- **[bambu-print-guard](https://github.com/noskillor/bambu-print-guard)** — Local, free AI failure detection for Bambu printers in LAN-only + Developer mode via Home Assistant (ha-bambulab): watches the camera with the open-source Obico model for spaghetti, detached parts and blobs, and sends a push notification with an annotated photo, the layer and Z height where the failure started, the last good layer, and Pause / Resume buttons; no cloud, subscription or GPU.
- **[Bambu Lab Cards (CzechTropi)](https://github.com/CzechTropi/bambulab-card)** — Three minimalist HACS dashboard cards built on ha-bambulab: a printer card (camera, progress, temperatures, errors), an AMS card styled like Bambu Studio and an external-spool card, all configurable in the visual editor, with a mock data source for trying them without a printer.
- **[Bambu Filament Manager (Trunks1982)](https://github.com/Trunks1982/ha-bambu-filament-manager)** — HACS spool inventory for Bambu printers in Home Assistant, running on ha-bambulab: an AMS card styled like Bambu Studio, NFC stickers with one-tap slot loading, live usage tracking, AMS drying and humidity warnings, per-print costs and notifications; sending to the AMS needs LAN mode with Developer Mode.

## Firmware & hardware mods

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — Custom firmware for X1 / X1C.
- **[Bambu-Lab-Klipper-Conversion](https://github.com/ChazLayyd/Bambu-Lab-Klipper-Conversion)** — Run Klipper by replacing the internal electronics.
- **[BMCU-C-PJARCZAK](https://github.com/jarczakpawel/BMCU-C-PJARCZAK)** — BMCU 370C firmware for A1 / A1 mini / P1S.
- **[Bambu-Bus](https://github.com/Bambu-Research-Group/Bambu-Bus)** — Tools and docs on the Bambu Bus.
- **[x1-expander](https://github.com/jwise/x1-expander)** — Expander board for the X1 Carbon.
- **[OpenBL](https://github.com/opensourcemanufacturing/OpenBL)** — Exploration of printer hardware and firmware.
- **[bambu-cuts](https://github.com/unrelatedlabs/bambu-cuts)** — Cutter and plotter for the A1 mini.
- **[BambuScribe](https://github.com/Animesh-Varma/BambuScribe)** — Turn a Bambu Lab printer into a pen plotter with safe custom G-code (no slicer hacks).
- **[P1S Pen Plotter](https://github.com/gtls64/p1s-pen-plotter)** — Turns a P1S into a pen plotter: arrange SVGs on the bed and export a .gcode.3mf to print from Bambu Studio, with pen-swap pauses per colour; work in progress, tested on one printer.
- **[BambuScribe Write](https://github.com/ICEIU-I/BambuScribe-Write)** — Desktop app that lays out text, formulas, tables and images as handwriting for an A1 with a pen, generates the G-code and uploads it over LAN; README in Chinese.
- **[Bambu-Poop-Conveyor-ESP32](https://github.com/t0nyz0/Bambu-Poop-Conveyor-ESP32)** — ESP32 waste conveyor with MQTT automation.
- **[PandaStatusOS](https://github.com/jeremykenedy/PandaStatusOS)** — Clean-room open firmware for the BIGTREETECH Panda Status P2 LED bar.
- **[ReBLLED](https://github.com/brossow/ReBLLED)** — Alternative firmware for the BLLED ESP32 LED controller that lights the chamber automatically and shows print status.
- **[A1 Mini Pen Plotter](https://github.com/Hansolox80/a1-mini-pen-plotter)** — Cross-platform desktop app that converts SVGs into optimized G-code for pen plotting on a Bambu Lab A1 Mini.
- **[BMCU A1 Lite](https://github.com/kolengri/bmcu-a1-lite)** — Experimental BMCU 370C firmware that implements the AMS Lite protocol for an A1 on firmware 01.08.01.00 with stock Bambu Studio; one two-color print reported on the developer's board so far.
- **[A1 hotend sensor board RE](https://github.com/rjacobs1969/bambulab_a1_filament_sensor)** — Reverse-engineering notes for the Bambu Lab A1 hotend sensor board: the 8-pin flat cable pinout, schematic, three Hall-effect sensors (filament presence, cutter position, tangling), measured voltages and an EBB42 adapter board.
- **[Panda State](https://github.com/ImSammyTTV/Panda-State)** — Open replacement firmware for BIQU's ESP32-C3 Panda light boards (Panda Status P2 for P2S/X2D and others) with extra effects, Home Assistant over MQTT and an open HTTP API.
- **[BamButton-IDF](https://github.com/FLsmaier/BamButton-IDF)** — Pure ESP-IDF port of Bambutton for an ESP32-C3 Super Mini: a physical button that polls Bambuddy, flashes its LED while the printer waits for the plate to be cleared, and sends the plate-clear through the Bambuddy API when pressed; setup via the board's own access point.

## Slicers, profiles & G-code

- **[OrcaSlicer](https://github.com/OrcaSlicer/OrcaSlicer)** — Open-source slicer with first-class Bambu support.
- **[OrcaSlicer-bambulab](https://github.com/FULU-Foundation/OrcaSlicer-bambulab)** — OrcaSlicer variant focused on Bambu printers.
- **[OrcaStudio](https://github.com/jarczakpawel/OrcaStudio)** — Bambu Studio fork with OrcaSlicer changes.
- **[bambulab-studio-orca-slicer-presets](https://github.com/DRIgnazGortngschirl/bambulab-studio-orca-slicer-presets)** — Community presets collection.
- **[Bambu_CustomGCode](https://github.com/eukatree/Bambu_CustomGCode)** — Custom G-code for Bambu Studio.
- **[Filament_Calibration_Wizard](https://github.com/Django1982/Filament_Calibration_Wizard)** — Filament calibration helper for Orca and Bambu Studio.
- **[Bricklayers](https://github.com/TengerTechnologies/Bricklayers)** — Brick-layer post-processing script.
- **[StudioBridge](https://github.com/Rdiger-36/StudioBridge)** — Adds printers from other accounts to Bambu Studio.
- **[docker-orcaslicer](https://github.com/linuxserver/docker-orcaslicer)** — OrcaSlicer in a browser-accessible container.
- **[docker-bambustudio](https://github.com/linuxserver/docker-bambustudio)** — Bambu Studio in a browser-accessible container.
- **[obs-bambustudio](https://github.com/ciroiriarte/obs-bambustudio)** — Unofficial native Bambu Studio packages for openSUSE and other Linux distributions, built from upstream source on the openSUSE Build Service and rebuilt automatically on new releases.
- **[layer-rescue](https://github.com/EmirhanSyl/layer-rescue)** — Bambu Studio post-processing script to resume a failed print from any layer.
- **[preset-porter](https://github.com/OMRITGM/preset-porter)** — Browser tool that fixes Bambu Studio filament presets that become "Unsupported" after switching printers.
- **[shambu](https://github.com/Shavvimal/shambu)** — CLI and Claude Code plugin to build, inspect and patch Bambu Studio .3mf projects and slice headless.
- **[PausePalette](https://github.com/DanaLeeTech/PausePalette)** — Plans colour order and inserts spool-swap pauses so you can print more colours than your AMS has slots.
- **[pandy-slicer](https://github.com/gccammelli/pandy-slicer)** — Bambu Studio's CLI slicer as a Home Assistant add-on or Docker container, so the Pandy app can print MakerWorld models in LAN-only mode.
- **[Bambuddy for OrcaSlicer](https://github.com/nobodyguy/orca-bambuddy)** — OrcaSlicer plugin that sends sliced plates to a Bambuddy server to print, queue or store, and shows your Bambuddy printers in the slicer.
- **[slicers.wasm](https://github.com/boolean3d/slicers.wasm)** — Unofficial WebAssembly builds of Bambu Studio, OrcaSlicer and PrusaSlicer that run in a browser tab and slice locally, plus a helper to reach printers on your network.
- **[BambuStudio Import for OrcaSlicer](https://github.com/Flexicano/orcaslicer-bambustudio-import)** — OrcaSlicer 2.5 plugin that imports your Bambu Studio filament, process and printer user profiles, showing which ones will work before you import.
- **[SlicerBridge](https://github.com/UnicornGraveyard/SlicerBridge)** — Converts a multicolor 3MF project from Bambu Studio, OrcaSlicer or a maker fork into a ready file for each of 34 printers, keeping painted colors and print settings.
- **[QuickLook 3MF Viewer](https://github.com/Natlab3d/QuickLook.Plugin.ThreeMFViewer)** — QuickLook plugin for Windows that previews 3MF and Bambu Studio projects in 3D with their saved filament colors, including painted regions.
- **[PrintLater](https://github.com/rgerr/printlater)** — Windows tool that starts a print at a chosen time by adding a cold-wait block to the top of a sliced .gcode.3mf, keeping Bambu Handy and cloud printing; no Developer Mode, LAN-only mode or firmware changes.
- **[bambu2prusa](https://github.com/charliejgallo/bambu2prusa)** — Converts Bambu Studio 3MF projects so PrusaSlicer can open them, one file per plate with negative parts and modifiers kept; lightly tested.
- **[3MF Colour Converter](https://github.com/haglundmorten-code/3mf-colour-converter)** — Browser tool that moves painted multi-colour projects between Bambu Studio / OrcaSlicer and PrusaSlicer without repainting, keeping parts and modifiers; files never leave the browser.
- **[OrcaSlicer Nonplanar](https://github.com/fich-l/orcaslicer-nonplanar)** — Test release of OrcaSlicer 2.4.2 with nonplanar top surfaces on gently sloped tops (up to 12°), checked against a hotend model; community tests list A1, A1 mini, P1S, P2S, X1C, X2D and H2D as working. Official build is macOS on Apple Silicon only.
- **[slicer-engine-wasm](https://github.com/gantry3d/slicer-engine-wasm)** — Build recipe and patches that compile Bambu Studio's slicing engine (without the GUI) to WebAssembly so it can slice a 3MF offline on a phone or under Node; releases ship engine.wasm with checksums. AGPL-3.0, not affiliated with Bambu Lab.
- **[bambu-auto-wipe](https://github.com/langkuo/bambu-auto-wipe)** — Bambu Studio post-processing script that adds nozzle wipes by accumulated extrusion length, only during infill moves, with presets for H2D, A1 / A1 mini, P1P / P1S and X1 / X1C.
- **[Preset Doctor](https://github.com/smehl86/preset-doctor)** — Offline Windows tool that finds custom filament, process and printer presets that vanished after a Bambu Studio or OrcaSlicer update because their parent preset was renamed, and repairs them.
- **[bambu-studio-wasm](https://github.com/3dfarmers/bambu-studio-wasm)** — Bambu Studio v02.09.01.70's command-line slicer and libslic3r compiled to WebAssembly, so a web page can slice a Bambu Studio project on the visitor's own computer; experimental, AGPL-3.0.
- **[Slicer Router](https://github.com/PrintHive/slicer-router)** — Rust library, CLI and Tauri app for macOS and Windows that opens each .3mf in the slicer that made it (Bambu Studio, OrcaSlicer, Snapmaker Orca or PrusaSlicer) by reading its metadata.
- **[U1 Converter](https://github.com/kitkat0981/u1-converter)** — In-browser converter for Bambu Studio filament presets and .3mf projects so they work in Snapmaker Orca for the Snapmaker U1; files are not uploaded, and it self-hosts with Docker.
- **[VertexSlicer](https://github.com/cybertech99/VertexSlicer)** — Rust mixed-layer-height slicer for the H2D (separate heights for walls and infill, plus per-zone settings) that reads your Bambu Studio profiles and writes a .gcode.3mf Bambu Studio can preview and send.
- **[X2D mixed nozzle sizes](https://github.com/sebo2000/x2d-mixed-nozzle)** — Unofficial, experimental script and small GUI that re-slices a Bambu Studio project with Bambu Studio's own CLI so an X2D can print one plate with a different nozzle size on each side (for example 0.2 mm on Main and 0.4 mm on Auxiliary).
- **[Bambu Filament Library for Fusion](https://github.com/mtenemy2/fusion-bambu-filament-library)** — Autodesk Fusion script that adds every Bambu Lab filament color as an appearance and each product line as a physical material from Bambu's technical data sheets, updating from Bambu's official color table.
- **[bambu-filament-profiles](https://github.com/skornehl/bambu-filament-profiles)** — Tool that builds Bambu Studio filament profiles sorted by brand (instead of everything under "Generic") from open filament databases fetched on your computer, and installs them into a local Bambu Studio (Linux, Flatpak, Windows, macOS), with a local companion app to search and install; targets the P1S with a 0.4 mm nozzle.
- **[MakerWorld Settings Importer for OrcaSlicer](https://github.com/FleeceFlames/Orca_makerworld_importer)** — OrcaSlicer 2.5+ Python plugin that converts a MakerWorld `.3mf` (usually sliced for Bambu printers) to your currently active printer, overlaying only the creator's compatible process settings on your own printer, plate and filament presets, and writing a change log.
- **[bambu-slice-mcp](https://github.com/ZHT0711/bambu-slice-mcp)** — MCP server that runs Bambu Studio / OrcaSlicer's own slicing engine headlessly through the CLI and sweeps a setting (layer height, support threshold, infill…) to report measured print time and filament use per variant; also flattens the preset inheritance chains the CLI ignores.
- **[NoCali](https://github.com/HanSur94/nocali)** — Small local web page for the X1 Carbon / X1 that removes the vibration (resonance) calibration from a sliced file, opens the cleaned file in Bambu Connect to print, and shows the printer live (progress, temperatures, fans, AMS filaments, HMS errors in plain text, camera); the printer stays in normal cloud mode.
- **[BatchSlicer](https://github.com/drak42/batch_slicer)** — Linux command-line tool (`pipx install batchslicer`) that slices one model or whole folders with Bambu Studio's, OrcaSlicer's or Creality Print's own CLI and the printer, filament and process presets you already have: kit parts arranged on plates, multiple copies, multi-colour 3MF filament slots filled, preview pictures added to the G-code, and a watch folder; direct sending targets Klipper and OctoPrint, not Bambu printers.
- **[EmberCheck](https://github.com/drewrobinso/embercheck)** — Local, Helio-style post-processor for Bambu Studio G-code: a per-layer thermal check with an HTML heat-map report, then slowing too-hot layers and speeding up inner walls and infill on cool ones, overhang and bridge fan fixes, missing-retraction detection and travel reordering; Windows installer, with a preview Python build for macOS and other systems.

## Print farms & queues

- **[bambuddy](https://github.com/maziggy/bambuddy)** — Self-hosted command center.
- **[bambu-farm](https://github.com/TFyre/bambu-farm)** — Web interface for multiple printers.
- **[fdm-monster](https://github.com/fdm-monster/fdm-monster)** — Printer farm management platform.
- **[print-farm-manager](https://github.com/joeltelling/print-farm-manager)** — Multi-brand self-hosted farm manager.
- **[bambu-gateway](https://github.com/leolobato/bambu-gateway)** — Self-hosted LAN web app and REST API to monitor and print on Bambu printers.
- **[fabrica](https://github.com/wsturner88/fabrica)** — Local multi-brand print farm dashboard with cameras, AMS spool control and MCP tools for AI agents.
- **[BambuStand](https://github.com/cliffom/bambustand)** — Terminal and local web dashboard for watching a Bambu Lab print farm through Bambu Cloud: printer status, progress, time left, temperatures, AMS filament and faults (formerly bambu-tui).
- **[Printer Farmlord](https://github.com/levleon13/printer-farmlord)** — Self-hosted LAN dashboard for a room of Bambu printers with cameras, AMS spools, automatic drying and print controls; runs on a spare Android phone, Mac or Linux.
- **[BamDude](https://github.com/kainpl/bamdude)** — Self-hosted print archive, management and automation system for Bambu Lab printers; a hard fork of Bambuddy with a Telegram bot, multi-chat auth and Ukrainian locale.
- **[Print Handy](https://github.com/catduckgnaf/print-handy)** — Local-first companion that takes a model link from Discord, Telegram or Matrix, slices it, matches spools, asks before printing and watches the camera for spaghetti on Bambu and other printers.
- **[ODIN](https://github.com/HughKantsime/runsodin)** — Self-hosted 3D print farm manager (MES / SCADA style) for Bambu Lab, Klipper, Prusa and Elegoo, with no cloud required.
- **[PrintFarm Assistant](https://github.com/Bronove/printfarm-assistant)** — Unofficial Windows desktop workbench for farms using Bambu Studio: batch import, settings changes, slicing, plate arrangement and output checks in one local workspace; base code is MIT, some optimisation components are closed source; README in Chinese.
- **[PF PrintFloor](https://github.com/pomeroyfamily/pf-printfloor)** — Self-hosted, status-only web dashboard for a mixed printer fleet (Bambu Lab, Snapmaker U1 / Klipper and Elegoo Centauri Carbon) on one page; it never starts, pauses or changes prints, only smart plugs and camera streams. Early release.
- **[Panda Connect](https://github.com/Skaronator/panda-connect)** — Local Bambu Lab printer driver for the self-hosted Prusa Connect server, so a mixed fleet can be managed in one place: it talks to the printer directly over MQTT/TLS in LAN-only mode with no Bambu account or cloud; H3C controls are hardware-verified, other models start as read-only monitoring.
- **[printfarm-planner](https://github.com/projectbin07-stack/printfarm-planner)** — Plans a production run across a mixed printer fleet (Bambu Lab P1S, A1, A1 Mini or your own models), taking operator hours, AMS, material and nozzle constraints into account, and outputs a schedule, utilisation figures and a browser Gantt chart.
- **[InvenTree Bambuddy](https://github.com/nemccarthy/inventree-bambuddy)** — InvenTree plugin that prints parts through Bambuddy: link a part to its sliced file, press Print to raise a build order and stage the plates in the Bambuddy queue, then book the good parts into stock; can optionally queue prints itself when stock falls below the minimum.
- **[bambu-autoeject](https://github.com/bullsrobo-boop/bambu-autoeject)** — Joins several sliced plates into one job for a Bambu Lab A1 that, after each print, cools the bed, pushes the parts off the front with the nozzle and starts the next, with no extra hardware or firmware changes; alpha, not yet tested on a real printer.
- **[kanbambu](https://github.com/akilea/kanbambu)** — Self-hosted kanban (FastAPI + SQLite, Docker) for print projects: drop a .gcode.3mf to read print time, grams per colour and a preview, and track copies, plates, successes and failures with retry history; no connection to the Bambu cloud or the printer. README in French.

## Filament, AMS & RFID

- **[RFID-Tag-Guide](https://github.com/Bambu-Research-Group/RFID-Tag-Guide)** — Reading the filament tags.
- **[Bambu-Lab-RFID-Library](https://github.com/queengooborg/Bambu-Lab-RFID-Library)** — Library of filament tag scans.
- **[OpenSpool](https://github.com/spuder/OpenSpool)** — Open RFID for filament spools.
- **[openspoolman](https://github.com/drndos/openspoolman)** — Spoolman with Bambu NFC tags.
- **[bambu-spoolman](https://github.com/mrkirby153/bambu-spoolman)** — Bambu integration for Spoolman.
- **[HaspelSync](https://github.com/Rdiger-36/HaspelSync)** — Track filament consumption.
- **[flipper-bambu](https://github.com/uzyn/flipper-bambu)** — Flipper Zero NFC parser for Bambu filament.
- **[bambu-spoolman-bridge](https://github.com/Yarasarda/bambu-spoolman-bridge)** — Tracks third-party filament usage in Spoolman without switching to LAN-only mode.
- **[TigerTag-Studio-Manager](https://github.com/TigerTag-Project/TigerTag-Studio-Manager)** — Desktop printer and filament manager for the TigerTag open NFC standard.
- **[TigerSpool-RFID](https://github.com/TigerTag-Project/TigerSpool-RFID)** — ESP32 + PN532 RFID spool scanner that assigns filament to printer slots.
- **[bambu-ams-spool-sync](https://github.com/demonkazuya/bambu-ams-spool-sync)** — Home Assistant integration that pushes Spoolman Sync spool assignments to Bambu AMS trays.
- **[bambu-spoolman-autoadd](https://github.com/Satal/bambu-spoolman-autoadd)** — Small service that creates Bambu RFID spools in Spoolman as soon as they are loaded into an AMS tray, via ha-bambulab in Home Assistant; works in cloud mode, no LAN mode needed.
- **[BridgeBox](https://github.com/J0eB0l/BridgeBox)** — Small board that connects a stock Bambu AMS (AMS 1, AMS 2 Pro, AMS HT, AMS Lite) to a Klipper printer through AFC-Klipper-Add-On, without opening the AMS or changing its firmware.
- **[Bambu Filament Companion](https://github.com/IATolk/Bambu-Filament-Companion)** — Unofficial Windows scheduled task that deducts each finished print's filament from spool weights in Bambu Studio's cloud Filament Manager; built for an A1 with AMS Lite.
- **[bambu-hando](https://github.com/john-crouch/bambu-hando)** — Loads filament profiles from SpoolmanDB or your own JSON and turns them into Bambu Studio custom filament presets (Linux, macOS) plus matching filaments and spools in SpoolEase.
- **[Bambu Lab to Spoolman Bridge](https://github.com/andreas-fe/bambu-spoolman-plus)** — Docker service that books filament use from A1, P1 and X1 printers into Spoolman over LAN, reading per-slot grams from the sliced file over FTPS and the active tray over MQTT; README in German.
- **[Bambu AMS RFID Filament Tracker](https://github.com/Aleitao2/bambu-ams-rfid)** — ESP32 firmware and Home Assistant automations for a P1S + AMS with third-party spools: reads NFC stickers through the AMS's own RFID board over SPI (plus a PN532), looks the tag up in Spoolman and assigns the spool to the tray in Bambuddy.
- **[FilMaNH](https://github.com/NikolausH76/FilMaNH)** — Local filament and spool manager for Bambu Lab printers on macOS, Windows and Android: follows the printers on your home network and books each print's usage and cost, without cloud or printer settings changes; README in German with an English version.
- **[3MF Katalog Manager](https://github.com/Bexxs75/3mf-katalog-manager)** — Local desktop app to catalog 3MF / STL / STEP / OBJ models and manage filament spools and AMS slots on Linux, Windows and macOS; English, German, Spanish and French.
- **[Bambu Filament Manager for Home Assistant](https://github.com/alex1255/bambu-filament-manager)** — Home Assistant integration that keeps a numbered spool inventory, assigns spools to AMS slots and deducts each finished print's per-slot usage reported by the Bambu Lab integration; first test release from a P1S setup, README in German.
- **[Spoolbook](https://github.com/Infraviored/spoolbook)** — Home Assistant integration that tracks every spool in a Bambu Lab AMS, including third-party spools, with an AMS overview, live per-print usage, weighing and QR labels.
- **[Bambu Filament Scanner](https://github.com/talla83/bambu-filament-scanner)** — Android app (8.0+) that reads the MIFARE Classic 1K NFC tags on original Bambu Lab spools and shows material, type, colour (with Bambu colour name), diameter, weight, length, temperatures, drying and production date, with a local scan history; read-only, needs a phone with MIFARE Classic support. README in German.
- **[simplyusage](https://github.com/wendsell/simplyusage)** — When a Bambu print sent from Bambu Studio or Orca ends, reads the real per-colour usage from the print file and deducts it from the SimplyPrint spool in each AMS slot used, filling the gap SimplyPrint leaves for prints it did not start itself.
- **[Spool Inventory](https://github.com/sfandetti/panda-command-3d-desktop)** — Local app that connects to Bambu Lab printers over your network to show what is loaded in every AMS slot and how much is left on each roll, and keeps a shelf inventory: scan Bambu rolls with a Flipper Zero and sync over USB, let rolls be added as they pass through the AMS, or add other brands by hand.
- **[Bambu NFC](https://github.com/faraztp/bambu-nfc)** — macOS Python tool for the MIFARE Classic 1K RFID tags on Bambu Lab spools using a PN532 reader: diagnoses the tag, shows filament data, dumps it, and rewrites it as a standard NDEF tag (URL, text, Wi-Fi credentials or raw bytes), deriving the keys from the UID.
- **[PixxelSpool](https://github.com/pixxelhoff/PixxelSpool)** — Self-hosted filament storage for Bambu Lab users on a Raspberry Pi, Mac or Windows PC: put a spool on the NFC reader (or into the AMS) to see what it is, where it belongs and how much is left; syncs with the AMS, checks print jobs and 3MF files and finds colours from a photo, with no account or cloud. In beta.
- **[Bambu Filament Guard](https://github.com/parthalon025/bambu-filament-guard)** — Windows companion to Bambu Studio that, each time you slice a plate, works out how many grams of each filament the print needs (purge and prime tower included), asks the printer how much each spool has left after the running print, and warns before you print if a spool will not last.
- **[bambu-bus-reference](https://github.com/heavydms/bambu-bus-reference)** — Unofficial, source-tagged reference for the RS-485 bus between a Bambu printer and its AMS units, measured on an X2D with AMS 2 Pro: framing, message types, sequences and the pins 5/6 buffer signal, with figures from logic-analyzer captures plus the ESP32-S3 bridge/parser firmware and tools used to make them.

## Camera & timelapse

- **[BambuP1Streamer](https://github.com/slynn1324/BambuP1Streamer)** — MJPEG stream for P1 printers.
- **[bambu-go2rtc](https://github.com/synman/bambu-go2rtc)** — go2rtc MJPEG streamer.
- **[BambuSource2Raw](https://github.com/hisptoot/BambuSource2Raw)** — Raw webcam stream from X1 / P1P.
- **[BambuCAM](https://github.com/BangerTech/BambuCAM)** — Web app for monitoring multiple printer cameras.
- **[print-guard](https://github.com/Servation/print-guard)** — Experimental Windows program that watches a P1S over LAN MQTT and its camera, scores frames with a spaghetti detector, and pauses or stops failing prints; has an alert-only dry-run mode.
- **[scrypted-bambu](https://github.com/tetra-fox/scrypted-bambu)** — Scrypted plugin that brings Bambu printer cameras (port 6000 JPEG on P1/A1, RTSP on X1/H2/P2) into HomeKit or an NVR, plus a chamber light switch.
- **[PrintView](https://github.com/wvfouram/printview)** — Raspberry Pi 5 service for a P1S in LAN-only + Developer Mode: live camera, controls, local spaghetti detection, per-layer timelapses and an Arduino bed relay, used from a phone web app, an Android app or a public link.
- **[Bambu X2D OBS overlay](https://github.com/chatcode-lab/bambu-overlay)** — Locally hosted, read-only OBS overlay for streaming X2D prints: progress, temperatures, plate preview, filament and AMS slots in six layouts, plus automatic camera-crop panning and an audio meter; built as a macOS app.
- **[PrintBot camera](https://github.com/paulnorthup/ha-printbot-camera)** — Home Assistant camera for the Bambu Lab H2S that plays the printer's 1080p/30 fps live view over WebRTC through Home Assistant's built-in go2rtc, keeping a single connection to the printer so the dashboard's HLS and WebRTC players no longer knock each other over.

## Dashboards, displays & apps

- **[BambuHelper](https://github.com/Keralots/BambuHelper)** — ESP32 desk monitor over MQTT.
- **[PrintSphere](https://github.com/cptkirki/PrintSphere)** — Round ESP32-S3 status companion.
- **[CYD-Klipper](https://github.com/suchmememanyskill/CYD-Klipper)** — Wireless status display (Klipper / Bambu / OctoPrint).
- **[BambUI](https://github.com/fidoriel/BambUI)** — Open UI for LAN mode.
- **[openbu](https://github.com/cygnusx-1-org/openbu)** — Android app for Developer Mode.
- **[panda-be-free](https://github.com/MiguelSchulz/panda-be-free)** — Open-source iOS printer dashboard.
- **[BambuBoard](https://github.com/t0nyz0/BambuBoard)** — Near real-time web dashboard.
- **[Bambulabs-Exporter](https://github.com/Aetrius/Bambulabs-Exporter)** — Prometheus exporter.
- **[xtouch](https://github.com/xperiments-in/xtouch)** — ESP32 touchscreen firmware for controlling and monitoring Bambu Lab printers.
- **[Bambu OLED Info](https://github.com/Asimmimx/bambu-oled-info)** — ESP32-C3 desk gadget with a small OLED and rotary knob that shows live printer status over local MQTT or your Bambu account; read-only.
- **[PrintGlance](https://github.com/talic/PrintGlance)** — Mac menu bar app for Bambu print progress and failure reasons over LAN.
- **[toothpeek](https://github.com/loicbisiere/toothpeek)** — Mac menu bar app with live camera, print progress and notifications for Bambu printers over LAN.
- **[print-heatmap](https://github.com/artemnovichkov/print-heatmap)** — GitHub-style heatmap of your Bambu printing history for a profile README or pinned gist.
- **[PrintCtrl](https://github.com/VoidedKN0X/PrintCtrl)** — Telemetry-free Android app for self-hosted Bambuddy and Spoolman servers, covering your Bambu printers and filament spools.
- **[Tiger Touch](https://github.com/TigerTag-Project/Tiger-Touch)** — Free open-source firmware that turns the BIGTREETECH Panda Touch / K-Touch into one touchscreen for Bambu Lab and other brands' printers, plus Klipper and OctoPrint.
- **[xTouch-CN](https://github.com/tbc0309/xTouch-CN)** — Independently maintained multilingual fork of xtouch for ESP32-2432S028R and Waveshare ESP32-S3/P4 boards, with web flashing, AMS management and camera on S3/P4.
- **[BambuDeck](https://github.com/Ripwords/BambuDeck)** — Self-hosted mobile PWA for Bambu printers in LAN mode: prints, cameras, toolpath layer preview, file browser, AMS filament and Home Assistant MQTT Discovery; runs in Docker.
- **[Layerwatch](https://github.com/d01/layerwatch)** — Android app to watch and control Bambu printers directly over your own network, with live camera and lock-screen alerts; no cloud account, ads or tracking.
- **[BambuBar](https://github.com/kopytjuk/bambubar)** — macOS menu bar app showing live print progress, time left, temperatures and AMS humidity over local MQTT.
- **[Bambu Bar](https://github.com/rolottr/bambu-bar)** — Native macOS menu bar app and desktop widgets for several Bambu printers over LAN, with a 3D printer model, AMS grams left, print controls and notifications; no account or cloud.
- **[Bambu Bar for Windows](https://github.com/bhex/bambu-bar-windows)** — Native Windows tray port of Bambu Bar for P2-series printers, with live status, AMS filament and pause, resume, stop and speed controls over the printer's MQTT; no cloud or account.
- **[bambu-monitor](https://github.com/koevetmc/bambu-monitor)** — Lightweight Linux system-tray monitor with desktop notifications and pause, resume, stop and light controls over local MQTT; no cloud or account.
- **[BambuDroid](https://github.com/kuaner/bambuDroid)** — Native Android LAN print dashboard for Bambu printers, built for non-touch screens and Bluetooth remotes; no cloud account.
- **[PrintWatch LAN](https://github.com/MJNProjekts/printwatch-lan)** — Telegram notifications, camera snapshots and remote control for Bambu P1/A1 printers in LAN-only mode, through your own Telegram bot; public beta.
- **[Mission Control for Bambu Lab](https://github.com/sthal/bambu-dash)** — Local mission-control style dashboard for one or several printers: native-quality camera with optional RTMP restreaming, progress, temperatures, AMS, print history and cost; no cloud, English and Russian UI.
- **[AMS-Screen](https://github.com/r3db/AMS-Screen)** — Dedicated AMS status screen over LAN for a Raspberry Pi (also runs on a PC or Mac), with a printable stand on MakerWorld; very early prototype.
- **[Gantry](https://github.com/parametryczny/Gantrybar)** — Menu-bar and tray monitor for macOS, Windows and Linux that follows a fleet of Bambu Lab, Klipper/Creality, Prusa and Snapmaker printers, with live status, AMS, camera and automations; local-first.
- **[Bambu Widget](https://github.com/davidkompan/bambuwidget)** — Windows desktop and Android home-screen widgets that show every printer on one or more Bambu Lab accounts through Bambu Cloud, with notifications.
- **[bambulab-exporter](https://github.com/D13410N3/bambulab-exporter)** — Read-only Prometheus exporter in Go that reads printer status over LAN MQTT; tested on an A1.
- **[P2S print station](https://github.com/airbornedan/p2s-print-station)** — LAN web page for a P2S to pick a file, place it, slice, preview, print and watch, without the Bambu Studio GUI or Handy; print control needs LAN and Developer mode.
- **[Bambu Dashboard](https://github.com/RealWarrior03/bambu-dashboard)** — Self-hosted Docker web dashboard for printers on your LAN: live status, HMS messages, MJPEG camera, light, temperature, fan and speed control, and AMS / AMS lite / AMS HT / AMS 2 Pro filament editing for several printers; README in German.
- **[iDotMatrix × Bambu Lab](https://github.com/tbc0309/idotmatrix-bambulab)** — ESP32-S3 controller that shows print status as animations on an iDotMatrix 32×32 Bluetooth pixel display, over LAN or the China / global Bambu cloud, with a web flasher and browser admin page; display only, no print control; README in Chinese with an English version.
- **[Bambu Monitor](https://github.com/Jolly-J/BambuMonitor)** — Android app that plays the printer's LAN RTSPS camera stream with hardware decoding, plus speed modes, light, pause/stop, temperatures, fans and AMS humidity and slots over LAN MQTT; README in Chinese.
- **[Pandy](https://github.com/gccammelli/pandy)** — Unofficial Android and iOS companion for Bambu printers in LAN-only mode: status, controls, AMS, MakerWorld browsing and slicing via pandy-slicer, with optional Home Assistant.
- **[bambu-decloud](https://github.com/vpavlin/bambu-decloud)** — Cloud-free setup for an A1: an Android app for monitoring, camera, AMS and slicing, a headless Bambu Studio behind a small HTTP API on a LAN box, and a FreeCAD macro that queues models for slicing.
- **[BambuDash](https://github.com/tunianbututou/BambuDash)** — Read-only multi-printer monitor for macOS, Windows and Android that signs in to Bambu Cloud and shows status, progress, layers, time left and temperatures, with history and a pinned mini window; sends no control commands; README in Chinese and English.
- **[bambu-printer-hub](https://github.com/NextBG/bambu-printer-hub)** — Small self-hosted remote dashboard: a LAN bridge makes only outbound connections to your server, which serves status, camera, pause / resume / stop and speed to phone or desktop, with HMS codes translated to Chinese.
- **[Bambu printer for Omarchy](https://github.com/jespermakes/omarchy-bambu)** — Omarchy bar plugin that talks to the printer over your own network: progress, temperatures, spools, chamber camera, notifications and pause, stop, light and speed, plus a bambu command; no cloud or account.
- **[BambuMonitor](https://github.com/ou0826/bambu-monitor)** — Windows desktop monitor that pops up alerts for finished, failed or paused prints, filament changes and HMS faults, over a direct LAN connection or through Bambu Cloud; README in Chinese, English version included.
- **[Bambu 3DPrint Dashboard for eWeLink CUBE](https://github.com/freezingzz/ewelink-cube-addon-bambu-3dprint-dashboard)** — Read-only eWeLink CUBE add-on that pulls printer status, AMS materials and job covers from Bambu Cloud and shows them on CUBE cards and CAST screens; currently focused on one H2C, English and Chinese UI.
- **[SDGoods Bambu Monitor](https://github.com/YeatsLiao/sdgoods-bambu-monitor)** — ESP-IDF firmware for the SDGoods ESP32-S3 round-screen device that shows a printer's progress, time left, temperatures and filament over the LAN, with 18 switchable skins; README in Chinese.
- **[printWatcher (BambuWatch)](https://github.com/yaturner/printWatcher)** — Android phone app plus Wear OS watch app that shows a Bambu Lab printer's progress on a tile, a watch-face complication and an ongoing-activity icon, and mirrors alerts for finished, paused or failed prints and HMS errors; the phone bridges local MQTT, with no cloud account or third-party server.
- **[MMM-BambuLab-BODK](https://github.com/BravoOscarDK/MMM-BambuLab-BODK)** — Configurable MagicMirror² module showing local Bambu Lab printer status over MQTT/TLS: job, progress, finish time, layers, temperatures, fans and AMS slots, with multiple printers; read-only, sends no control commands.
- **[webhook-p2s](https://github.com/Chris-Lzy/webhook-p2s)** — Lightweight Docker service that watches Bambu Lab printers over local MQTT and pushes start, finish, failure, pause and progress events to a DingTalk group bot, with camera snapshots and a web config page; no cloud sign-up.
- **[MyBambuddy](https://github.com/Michael3DPrint/mybambuddy)** — Unofficial Android app for monitoring and controlling a Bambu Lab printer through your own self-hosted Bambuddy server over plain HTTP; a personal project written for one X2D and tested against Bambuddy 1.3.0, meant for a home network or VPN.
- **[Bambu Deck](https://github.com/web-workers-com/bambu-deck)** — LAN-only Stream Deck plugin for up to four Bambu printers showing progress, AMS spools, temperatures and controls, taking over the whole deck when a print finishes or needs attention; UI in German for now.
- **[bambu-dash](https://github.com/zwmwei/bambu-dash)** — LAN-only live dashboard for Bambu printers as a web page, Android APK or NAS Docker container: progress, temperatures with 5-minute curves, AMS trays, fans, HMS alerts, camera (RTSPS to MJPEG), chamber light and pause / resume / stop (needs Developer Mode), with printer auto-discovery; developed and tested on a P2S. README in Simplified Chinese.
- **[Pygmy](https://github.com/danderik88/pygmy)** — Self-hosted Docker app that puts LAN-only Bambu Lab and Klipper printers on your phone without the cloud: live camera, controls, notifications, spaghetti detection, one-tap printing and an MCP endpoint for agents; early preview.
- **[BambuBar for Omarchy](https://github.com/tripex/omarchy-bambubar)** — Omarchy bar widget and panel showing a Bambu Lab printer's progress, time left, temperatures (both nozzles on H2D/X2D) and every AMS with spools in their real colours and humidity, plus a notification when a print ends; started as the Omarchy version of the macOS BambuBar.
- **[Bambu for UltraBar Studio](https://github.com/qlerup/ultrabar-bambu)** — Bambu LAN printer widgets for the CoreBAR display, configured in UltraBar Studio on your PC, which pins each printer's TLS certificate and streams live readings and controls to the bar.
- **[Bambu Monitor for Flexbar](https://github.com/UpKiry/flexbar-bambu-monitor)** — Read-only FlexDesigner plugin that shows a Bambu Lab printer's cloud status (state, job, progress, time left, layers, temperatures, AMS slots) on a Flexbar, with sign-in through a local browser page instead of LAN IP and access code; supports China and global accounts. README in Simplified Chinese.
- **[BambuPresence](https://github.com/ryanpcorg/BambuPresence)** — Lightweight pure-Go desktop app that connects to a Bambu Lab printer over LAN MQTT and shows live print status as Discord Rich Presence: model image, ETA or elapsed timer, layers, temperatures, active AMS spool, HMS error decoding, plus Windows toast notifications.
- **[Printvault](https://github.com/emphyri0/printvault)** — Self-hosted print archive (photos, model files, filament, print time, settings, notes, maintenance tasks) that auto-logs every Bambu print over a read-only local MQTT connection, so cloud mode keeps working; imports from MakerWorld links or sliced 3MF/G-code, and adds camera snapshots, temperature charts and HMS error codes. Only the P2S is tested on hardware, and it has no login, so keep it on a trusted network.
- **[PRINT//TRACE](https://github.com/Zosuya/print-trace)** — Read-only live 3D HUD that downloads the file being printed over FTPS and redraws the G-code toolpath layer by layer in sync with the printer's MQTT reports, embeddable in the Device tab of OrcaSlicer or Bambu Studio; tested on an A1, needs an SD card in the printer. README in Traditional Chinese and English.

## Bridges & AI agents

- **[OctoPrint-OctoEverywhere](https://github.com/QuinnDamerell/OctoPrint-OctoEverywhere)** — Remote access that also supports Bambu printers.
- **[OctoPrint-BambuPrinter](https://github.com/jneilliii/OctoPrint-BambuPrinter)** — OctoPrint plugin to connect Bambu Lab printers.
- **[bambu-printer-mcp](https://github.com/DMontgomery40/bambu-printer-mcp)** — MCP server for Bambu printers.
- **[bambu-mcp](https://github.com/griches/bambu-mcp)** — MCP server for multi-printer control.
- **[bambu](https://github.com/voska/bambu)** — Agent-friendly LAN CLI to slice, preflight, send and monitor prints.
- **[Kiln](https://github.com/codeofaxel/Kiln)** — MCP server for AI agents to design, slice and print on Bambu Lab and other printers.
- **[bamboozle](https://github.com/nxmxbbd/bamboozle)** — LAN-only Apple Home bridge that shows a Bambu printer's progress, status and camera in HomeKit, without Home Assistant or Homebridge.
- **[printshop-mcp](https://github.com/FireBall1725/printshop-mcp)** — MCP server for Bambuddy and Spoolman so an AI agent can check filament stock, send a sliced 3MF and watch the job.
- **[bambustudio-mcp](https://github.com/subhashdasyam/bambustudio-mcp)** — MCP server for the Bambu Studio slicer to inspect parts, configure saved 3MF projects and compare slices from Claude Code or Codex.
- **[bambu-sentinel-mcp](https://github.com/selcukgk29/bambu-sentinel-mcp)** — LAN-only MCP server for Bambu printers with live control, a filament-aware job queue across a fleet and print monitoring.
- **[Bambu Lab printer pane for Claude Code](https://github.com/artemnovichkov/claude-code-bambu-lab)** — Unofficial Claude Code plugin that shows a Bambu printer beside the chat: print settings, progress, temperatures, AMS spools, HMS errors and the plate thumbnail, with light, pause, resume, stop and skip-object buttons; status comes from Bambu's cloud, macOS only.
- **[Bambu Studio Advisor MCP](https://github.com/JohanRouyer/BambuStudio-Advisor-MCP)** — Local MCP server that lets Claude analyze an STL or 3MF, slice several variants with the Bambu Studio engine, compare time and weight, and hand back a ready .3mf project.
- **[Slicewise](https://github.com/gjlmotea/slicewise-mcp)** — MCP server for Bambu Studio presets and slicing: flattens preset inheritance so CLI slicing matches the GUI, audits which overrides took effect, and checks printability before slicing; does not control printers.

## Closed-source / commercial (for reference)

- **[Bambu Handy](https://bambulab.com/en/download)** — Official mobile app.
- **[MakerWorld](https://makerworld.com)** — Official model repository.

## Related lists

- [neardws/awesome-bambu](https://github.com/neardws/awesome-bambu) — Earlier small list.
- [Awesome](https://github.com/sindresorhus/awesome)

## Contributing

Open a PR or issue. One line per entry, open-source and on-topic, link to the repo, no star counts. Closed-source/commercial only in the reference section.

See [CONTRIBUTING.md](CONTRIBUTING.md) for the full rules, or [suggest a project](https://github.com/hypery11/awesome-bambu-lab/issues/new?template=suggest-project.yml) with the issue form.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright to this work.
