# Awesome Bambu Lab [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated map of the open-source ecosystem around Bambu Lab 3D printers: LAN control, Home Assistant, firmware, slicers, farms, filament and cameras.
>
> 精選 Bambu Lab 3D 印表機開源生態：區網控制、Home Assistant、韌體、切片、農場、線材與鏡頭。

**Status / 狀態:** Curated 2026-10. Contributions welcome. / 2026-10 整理，歡迎貢獻。

**Disclaimer / 免責聲明:** Unofficial, not affiliated with Bambu Lab. Custom firmware and hardware mods **may void your warranty** and can damage hardware; some firmware projects have licensing questions, check each project's license yourself. Use at your own risk. / 非官方，與 Bambu Lab 無關。自製韌體與硬體改裝**可能使保固失效**並損壞機器；部分韌體專案有授權疑義，請自行查閱。風險自負。

---

## Start here / 從這裡開始

The projects people actually share. Everything below is the map around them, not a product catalog.
別人會轉發的是這幾個。下面是圍繞它們的地圖，不是產品目錄。

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — Community custom firmware for the X1 / X1 Carbon. / X1／X1 Carbon 社群自製韌體。
- **[bambuddy](https://github.com/maziggy/bambuddy)** — Self-hosted, cloud-free command center for Bambu printers. / 自架、免雲端的 Bambu 印表機控制中心。
- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — Home Assistant integration for Bambu Lab printers. / Bambu Lab 的 Home Assistant 整合。
- **[OpenBambuAPI](https://github.com/Doridian/OpenBambuAPI)** — Community documentation of the Bambu printer APIs. / 社群整理的 Bambu API 文件。
- **[RFID-Tag-Guide](https://github.com/Bambu-Research-Group/RFID-Tag-Guide)** — How to read Bambu filament NFC/RFID tags. / 讀取 Bambu 線材 RFID 標籤的指南。

---

## Contents / 目錄

- [Official open source (bambulab) / 官方開源](#official-open-source-bambulab--官方開源)
- [LAN mode, APIs & libraries / 區網模式、API 與函式庫](#lan-mode-apis--libraries--區網模式api-與函式庫)
- [Home Assistant & automation / Home Assistant 與自動化](#home-assistant--automation--home-assistant-與自動化)
- [Firmware & hardware mods / 韌體與硬體改裝](#firmware--hardware-mods--韌體與硬體改裝)
- [Slicers, profiles & G-code / 切片、設定檔與 G-code](#slicers-profiles--g-code--切片設定檔與-g-code)
- [Print farms & queues / 列印農場與佇列](#print-farms--queues--列印農場與佇列)
- [Filament, AMS & RFID / 線材、AMS 與 RFID](#filament-ams--rfid--線材ams-與-rfid)
- [Camera & timelapse / 鏡頭與縮時](#camera--timelapse--鏡頭與縮時)
- [Dashboards, displays & apps / 儀表板、螢幕與 App](#dashboards-displays--apps--儀表板螢幕與-app)
- [Bridges & AI agents / 橋接與 AI 代理](#bridges--ai-agents--橋接與-ai-代理)
- [Closed-source / commercial (for reference) / 閉源／商業（對照用）](#closed-source--commercial-for-reference--閉源商業對照用)
- [Related lists / 相關列表](#related-lists--相關列表)
- [Contributing / 貢獻](#contributing--貢獻)
- [License / 授權](#license--授權)

---

## Official open source (bambulab) / 官方開源

- **[BambuStudio](https://github.com/bambulab/BambuStudio)** — Official slicer (open source). / 官方切片軟體（開源）。

## LAN mode, APIs & libraries / 區網模式、API 與函式庫

- **[OpenBambuAPI](https://github.com/Doridian/OpenBambuAPI)** — API documentation. / API 文件。
- **[bambulabs_api](https://github.com/BambuTools/bambulabs_api)** — Unofficial Python API. / 非官方 Python API。
- **[bambulabs_api](https://github.com/torbenconto/bambulabs_api)** — Unofficial Go bindings. / 非官方 Go 綁定。
- **[bambulab](https://github.com/markhaehnel/bambulab)** — Rust API client crate. / Rust API 客戶端。
- **[pybambu](https://github.com/greghesp/pybambu)** — Python library used by the HA integration. / HA 整合所用的 Python 函式庫。
- **[bambu-printer-manager](https://github.com/synman/bambu-printer-manager)** — Pure-Python printer manager library. / 純 Python 印表機管理函式庫。
- **[bambu-connect](https://github.com/mattcar15/bambu-connect)** — Stats, controls and camera access. / 讀取狀態、控制與鏡頭。
- **[Bambu-Lab-Cloud-API](https://github.com/coelacant1/Bambu-Lab-Cloud-API)** — Analysis of the Bambu cloud API. / Bambu 雲端 API 分析。
- **[open-bamboo-networking](https://github.com/ClusterM/open-bamboo-networking)** — Open replacement for Bambu Studio's proprietary network plugin. / 取代 Bambu Studio 專有網路外掛的開源實作。
- **[bambu-farm](https://github.com/ellenhp/bambu-farm)** — Self-hostable Bambu Cloud alternative. / 可自架的 Bambu Cloud 替代。
- **[open-bambu-networking-plugin](https://github.com/persano/open-bambu-networking-plugin)** — Open-source OrcaSlicer networking plugin: cloud printing, remote liveview, AMS sync. / OrcaSlicer 開源網路外掛：雲端列印、遠端鏡頭、AMS 同步。

## Home Assistant & automation / Home Assistant 與自動化

- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — Home Assistant integration. / HA 整合。
- **[ha-bambu-lab-p1-spaghetti-detection](https://github.com/nberktumer/ha-bambu-lab-p1-spaghetti-detection)** — Spaghetti detection integration. / 炒麵偵測整合。
- **[Bambu-HomeAssistant-Flows](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows)** — HA dashboards and Node-RED flows. / HA 儀表板與 Node-RED 流程。
- **[printwatch-card](https://github.com/drkpxl/printwatch-card)** — HA dashboard card for printer monitoring. / 監控印表機的 HA 卡片。
- **[SpoolmanSync](https://github.com/gibz104/SpoolmanSync)** — Automatic Spoolman tracking via HA. / 透過 HA 自動同步 Spoolman。
- **[HA-Panda-PWR](https://github.com/62fixolab/HA-Panda-PWR)** — Home Assistant integration for the BIGTREETECH Panda PWR smart plug. / BIGTREETECH Panda PWR 智慧插座的 Home Assistant 整合。

## Firmware & hardware mods / 韌體與硬體改裝

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — Custom firmware for X1 / X1C. / X1／X1C 自製韌體。
- **[Bambu-Lab-Klipper-Conversion](https://github.com/ChazLayyd/Bambu-Lab-Klipper-Conversion)** — Run Klipper by replacing the internal electronics. / 換掉主板改跑 Klipper。
- **[BMCU-C-PJARCZAK](https://github.com/jarczakpawel/BMCU-C-PJARCZAK)** — BMCU 370C firmware for A1 / A1 mini / P1S. / 給 A1／A1 mini／P1S 的 BMCU 韌體。
- **[Bambu-Bus](https://github.com/Bambu-Research-Group/Bambu-Bus)** — Tools and docs on the Bambu Bus. / Bambu Bus 工具與文件。
- **[x1-expander](https://github.com/jwise/x1-expander)** — Expander board for the X1 Carbon. / X1 Carbon 擴充板。
- **[OpenBL](https://github.com/opensourcemanufacturing/OpenBL)** — Exploration of printer hardware and firmware. / 印表機軟硬體探索。
- **[bambu-cuts](https://github.com/unrelatedlabs/bambu-cuts)** — Cutter and plotter for the A1 mini. / A1 mini 切割與繪圖。
- **[BambuScribe](https://github.com/Animesh-Varma/BambuScribe)** — Turn a Bambu Lab printer into a pen plotter with safe custom G-code (no slicer hacks). / 把 Bambu 印表機安全變成筆式繪圖機，產生自訂 G-code。
- **[Bambu-Poop-Conveyor-ESP32](https://github.com/t0nyz0/Bambu-Poop-Conveyor-ESP32)** — ESP32 waste conveyor with MQTT automation. / ESP32 廢料輸送帶。
- **[PandaStatusOS](https://github.com/jeremykenedy/PandaStatusOS)** — Clean-room open firmware for the BIGTREETECH Panda Status P2 LED bar. / BIGTREETECH Panda Status P2 燈條的 clean-room 開源韌體。

## Slicers, profiles & G-code / 切片、設定檔與 G-code

- **[OrcaSlicer](https://github.com/OrcaSlicer/OrcaSlicer)** — Open-source slicer with first-class Bambu support. / 對 Bambu 支援完整的開源切片。
- **[OrcaSlicer-bambulab](https://github.com/FULU-Foundation/OrcaSlicer-bambulab)** — OrcaSlicer variant focused on Bambu printers. / 聚焦 Bambu 的 OrcaSlicer 版本。
- **[OrcaStudio](https://github.com/jarczakpawel/OrcaStudio)** — Bambu Studio fork with OrcaSlicer changes. / 合入 OrcaSlicer 改動的 Bambu Studio 分支。
- **[bambulab-studio-orca-slicer-presets](https://github.com/DRIgnazGortngschirl/bambulab-studio-orca-slicer-presets)** — Community presets collection. / 社群設定檔集合。
- **[Bambu_CustomGCode](https://github.com/eukatree/Bambu_CustomGCode)** — Custom G-code for Bambu Studio. / 自訂 G-code。
- **[Filament_Calibration_Wizard](https://github.com/Django1982/Filament_Calibration_Wizard)** — Filament calibration helper for Orca and Bambu Studio. / 線材校正精靈。
- **[Bricklayers](https://github.com/TengerTechnologies/Bricklayers)** — Brick-layer post-processing script. / 磚式層疊後處理腳本。
- **[StudioBridge](https://github.com/Rdiger-36/StudioBridge)** — Adds printers from other accounts to Bambu Studio. / 把其他帳號的印表機加入 Bambu Studio。
- **[docker-orcaslicer](https://github.com/linuxserver/docker-orcaslicer)** — OrcaSlicer in a browser-accessible container. / 可用瀏覽器開的 OrcaSlicer 容器。
- **[docker-bambustudio](https://github.com/linuxserver/docker-bambustudio)** — Bambu Studio in a browser-accessible container. / 可用瀏覽器開的 Bambu Studio 容器。
- **[layer-rescue](https://github.com/EmirhanSyl/layer-rescue)** — Bambu Studio post-processing script to resume a failed print from any layer. / 從任意層續印失敗作品的 Bambu Studio 後處理腳本。

## Print farms & queues / 列印農場與佇列

- **[bambuddy](https://github.com/maziggy/bambuddy)** — Self-hosted command center. / 自架控制中心。
- **[bambu-farm](https://github.com/TFyre/bambu-farm)** — Web interface for multiple printers. / 多台印表機網頁介面。
- **[fdm-monster](https://github.com/fdm-monster/fdm-monster)** — Printer farm management platform. / 印表機農場管理平台。
- **[print-farm-manager](https://github.com/joeltelling/print-farm-manager)** — Multi-brand self-hosted farm manager. / 多品牌自架農場管理。

## Filament, AMS & RFID / 線材、AMS 與 RFID

- **[RFID-Tag-Guide](https://github.com/Bambu-Research-Group/RFID-Tag-Guide)** — Reading the filament tags. / 讀取線材標籤。
- **[Bambu-Lab-RFID-Library](https://github.com/queengooborg/Bambu-Lab-RFID-Library)** — Library of filament tag scans. / 線材標籤掃描資料庫。
- **[OpenSpool](https://github.com/spuder/OpenSpool)** — Open RFID for filament spools. / 開源線材 RFID。
- **[openspoolman](https://github.com/drndos/openspoolman)** — Spoolman with Bambu NFC tags. / 結合 Bambu NFC 的 Spoolman。
- **[bambu-spoolman](https://github.com/mrkirby153/bambu-spoolman)** — Bambu integration for Spoolman. / Spoolman 的 Bambu 整合。
- **[HaspelSync](https://github.com/Rdiger-36/HaspelSync)** — Track filament consumption. / 追蹤線材用量。
- **[flipper-bambu](https://github.com/uzyn/flipper-bambu)** — Flipper Zero NFC parser for Bambu filament. / Flipper Zero 線材 NFC 解析。
- **[bambu-spoolman-bridge](https://github.com/Yarasarda/bambu-spoolman-bridge)** — Tracks third-party filament usage in Spoolman without switching to LAN-only mode. / 不必切成純區網模式即可把第三方線材用量同步到 Spoolman。
- **[TigerTag-Studio-Manager](https://github.com/TigerTag-Project/TigerTag-Studio-Manager)** — Desktop printer and filament manager for the TigerTag open NFC standard. / TigerTag 開源 NFC 標準的桌面印表機與線材管理。
- **[TigerSpool-RFID](https://github.com/TigerTag-Project/TigerSpool-RFID)** — ESP32 + PN532 RFID spool scanner that assigns filament to printer slots. / ESP32＋PN532 線材 RFID 掃描器，掃完對應到印表機槽位。

## Camera & timelapse / 鏡頭與縮時

- **[BambuP1Streamer](https://github.com/slynn1324/BambuP1Streamer)** — MJPEG stream for P1 printers. / P1 的 MJPEG 串流。
- **[bambu-go2rtc](https://github.com/synman/bambu-go2rtc)** — go2rtc MJPEG streamer. / go2rtc 串流。
- **[BambuSource2Raw](https://github.com/hisptoot/BambuSource2Raw)** — Raw webcam stream from X1 / P1P. / X1／P1P 原始鏡頭串流。
- **[BambuCAM](https://github.com/BangerTech/BambuCAM)** — Web app for monitoring multiple printer cameras. / 多台鏡頭監看網頁。

## Dashboards, displays & apps / 儀表板、螢幕與 App

- **[BambuHelper](https://github.com/Keralots/BambuHelper)** — ESP32 desk monitor over MQTT. / ESP32 桌面監看器。
- **[PrintSphere](https://github.com/cptkirki/PrintSphere)** — Round ESP32-S3 status companion. / 圓形 ESP32-S3 狀態顯示。
- **[CYD-Klipper](https://github.com/suchmememanyskill/CYD-Klipper)** — Wireless status display (Klipper / Bambu / OctoPrint). / 無線狀態螢幕。
- **[BambUI](https://github.com/fidoriel/BambUI)** — Open UI for LAN mode. / 區網模式開源 UI。
- **[openbu](https://github.com/cygnusx-1-org/openbu)** — Android app for Developer Mode. / 開發者模式 Android App。
- **[panda-be-free](https://github.com/MiguelSchulz/panda-be-free)** — Open-source iOS printer dashboard. / 開源 iOS 儀表板。
- **[BambuBoard](https://github.com/t0nyz0/BambuBoard)** — Near real-time web dashboard. / 近即時網頁儀表板。
- **[Bambulabs-Exporter](https://github.com/Aetrius/Bambulabs-Exporter)** — Prometheus exporter. / Prometheus exporter。

## Bridges & AI agents / 橋接與 AI 代理

- **[OctoPrint-OctoEverywhere](https://github.com/QuinnDamerell/OctoPrint-OctoEverywhere)** — Remote access that also supports Bambu printers. / 支援 Bambu 的遠端存取。
- **[bambu-printer-mcp](https://github.com/DMontgomery40/bambu-printer-mcp)** — MCP server for Bambu printers. / Bambu 的 MCP server。
- **[bambu-mcp](https://github.com/griches/bambu-mcp)** — MCP server for multi-printer control. / 多機控制 MCP server。
- **[bambu](https://github.com/voska/bambu)** — Agent-friendly LAN CLI to slice, preflight, send and monitor prints. / 從終端機切片、預檢、送印與監看的區網 CLI，適合 AI 代理。
- **[Kiln](https://github.com/codeofaxel/Kiln)** — MCP server for AI agents to design, slice and print on Bambu Lab and other printers. / 讓 AI 代理設計、切片並在 Bambu 等印表機列印的 MCP server。

## Closed-source / commercial (for reference) / 閉源／商業（對照用）

- **[Bambu Handy](https://bambulab.com/en/download)** — Official mobile app. / 官方手機 App。
- **[MakerWorld](https://makerworld.com)** — Official model repository. / 官方模型平台。

## Related lists / 相關列表

- [neardws/awesome-bambu](https://github.com/neardws/awesome-bambu) — Earlier small list. / 較早的小型清單。
- [Awesome](https://github.com/sindresorhus/awesome)

## Contributing / 貢獻

Open a PR or issue. One line per entry, open-source and on-topic, link to the repo, no star counts. Closed-source/commercial only in the reference section.
歡迎開 PR 或 issue。每條一行、需開源且切題、直接連到倉庫、不放星數。閉源／商業只放對照區。

## License / 授權

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright to this work. / 在法律允許範圍內，貢獻者放棄本作品的所有著作權。
