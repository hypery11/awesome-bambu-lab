# Awesome Bambu Lab [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

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

## Contents

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

## Home Assistant & automation

- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — Home Assistant integration.
- **[ha-bambu-lab-p1-spaghetti-detection](https://github.com/nberktumer/ha-bambu-lab-p1-spaghetti-detection)** — Spaghetti detection integration.
- **[Bambu-HomeAssistant-Flows](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows)** — HA dashboards and Node-RED flows.
- **[printwatch-card](https://github.com/drkpxl/printwatch-card)** — HA dashboard card for printer monitoring.
- **[SpoolmanSync](https://github.com/gibz104/SpoolmanSync)** — Automatic Spoolman tracking via HA.
- **[HA-Panda-PWR](https://github.com/62fixolab/HA-Panda-PWR)** — Home Assistant integration for the BIGTREETECH Panda PWR smart plug.

## Firmware & hardware mods

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — Custom firmware for X1 / X1C.
- **[Bambu-Lab-Klipper-Conversion](https://github.com/ChazLayyd/Bambu-Lab-Klipper-Conversion)** — Run Klipper by replacing the internal electronics.
- **[BMCU-C-PJARCZAK](https://github.com/jarczakpawel/BMCU-C-PJARCZAK)** — BMCU 370C firmware for A1 / A1 mini / P1S.
- **[Bambu-Bus](https://github.com/Bambu-Research-Group/Bambu-Bus)** — Tools and docs on the Bambu Bus.
- **[x1-expander](https://github.com/jwise/x1-expander)** — Expander board for the X1 Carbon.
- **[OpenBL](https://github.com/opensourcemanufacturing/OpenBL)** — Exploration of printer hardware and firmware.
- **[bambu-cuts](https://github.com/unrelatedlabs/bambu-cuts)** — Cutter and plotter for the A1 mini.
- **[BambuScribe](https://github.com/Animesh-Varma/BambuScribe)** — Turn a Bambu Lab printer into a pen plotter with safe custom G-code (no slicer hacks).
- **[Bambu-Poop-Conveyor-ESP32](https://github.com/t0nyz0/Bambu-Poop-Conveyor-ESP32)** — ESP32 waste conveyor with MQTT automation.
- **[PandaStatusOS](https://github.com/jeremykenedy/PandaStatusOS)** — Clean-room open firmware for the BIGTREETECH Panda Status P2 LED bar.

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
- **[layer-rescue](https://github.com/EmirhanSyl/layer-rescue)** — Bambu Studio post-processing script to resume a failed print from any layer.

## Print farms & queues

- **[bambuddy](https://github.com/maziggy/bambuddy)** — Self-hosted command center.
- **[bambu-farm](https://github.com/TFyre/bambu-farm)** — Web interface for multiple printers.
- **[fdm-monster](https://github.com/fdm-monster/fdm-monster)** — Printer farm management platform.
- **[print-farm-manager](https://github.com/joeltelling/print-farm-manager)** — Multi-brand self-hosted farm manager.

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

## Camera & timelapse

- **[BambuP1Streamer](https://github.com/slynn1324/BambuP1Streamer)** — MJPEG stream for P1 printers.
- **[bambu-go2rtc](https://github.com/synman/bambu-go2rtc)** — go2rtc MJPEG streamer.
- **[BambuSource2Raw](https://github.com/hisptoot/BambuSource2Raw)** — Raw webcam stream from X1 / P1P.
- **[BambuCAM](https://github.com/BangerTech/BambuCAM)** — Web app for monitoring multiple printer cameras.

## Dashboards, displays & apps

- **[BambuHelper](https://github.com/Keralots/BambuHelper)** — ESP32 desk monitor over MQTT.
- **[PrintSphere](https://github.com/cptkirki/PrintSphere)** — Round ESP32-S3 status companion.
- **[CYD-Klipper](https://github.com/suchmememanyskill/CYD-Klipper)** — Wireless status display (Klipper / Bambu / OctoPrint).
- **[BambUI](https://github.com/fidoriel/BambUI)** — Open UI for LAN mode.
- **[openbu](https://github.com/cygnusx-1-org/openbu)** — Android app for Developer Mode.
- **[panda-be-free](https://github.com/MiguelSchulz/panda-be-free)** — Open-source iOS printer dashboard.
- **[BambuBoard](https://github.com/t0nyz0/BambuBoard)** — Near real-time web dashboard.
- **[Bambulabs-Exporter](https://github.com/Aetrius/Bambulabs-Exporter)** — Prometheus exporter.

## Bridges & AI agents

- **[OctoPrint-OctoEverywhere](https://github.com/QuinnDamerell/OctoPrint-OctoEverywhere)** — Remote access that also supports Bambu printers.
- **[bambu-printer-mcp](https://github.com/DMontgomery40/bambu-printer-mcp)** — MCP server for Bambu printers.
- **[bambu-mcp](https://github.com/griches/bambu-mcp)** — MCP server for multi-printer control.
- **[bambu](https://github.com/voska/bambu)** — Agent-friendly LAN CLI to slice, preflight, send and monitor prints.
- **[Kiln](https://github.com/codeofaxel/Kiln)** — MCP server for AI agents to design, slice and print on Bambu Lab and other printers.

## Closed-source / commercial (for reference)

- **[Bambu Handy](https://bambulab.com/en/download)** — Official mobile app.
- **[MakerWorld](https://makerworld.com)** — Official model repository.

## Related lists

- [neardws/awesome-bambu](https://github.com/neardws/awesome-bambu) — Earlier small list.
- [Awesome](https://github.com/sindresorhus/awesome)

## Contributing

Open a PR or issue. One line per entry, open-source and on-topic, link to the repo, no star counts. Closed-source/commercial only in the reference section.

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright to this work.
