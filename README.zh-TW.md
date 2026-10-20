# Awesome Bambu Lab [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

[English](README.md) | 繁體中文

> 精選 Bambu Lab 3D 印表機開源生態：區網控制、Home Assistant、韌體、切片、農場、線材與鏡頭。

**狀態：** 2026-10 整理，歡迎貢獻。

**免責聲明：** 非官方，與 Bambu Lab 無關。自製韌體與硬體改裝**可能使保固失效**並損壞機器；部分韌體專案有授權疑義，請自行查閱。風險自負。

---

## 從這裡開始

別人會轉發的是這幾個。下面是圍繞它們的地圖，不是產品目錄。

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — X1／X1 Carbon 社群自製韌體。
- **[bambuddy](https://github.com/maziggy/bambuddy)** — 自架、免雲端的 Bambu 印表機控制中心。
- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — Bambu Lab 的 Home Assistant 整合。
- **[OpenBambuAPI](https://github.com/Doridian/OpenBambuAPI)** — 社群整理的 Bambu API 文件。
- **[RFID-Tag-Guide](https://github.com/Bambu-Research-Group/RFID-Tag-Guide)** — 讀取 Bambu 線材 RFID 標籤的指南。

---

## 目錄

- [官方開源（bambulab）](#官方開源bambulab)
- [區網模式、API 與函式庫](#區網模式api-與函式庫)
- [Home Assistant 與自動化](#home-assistant-與自動化)
- [韌體與硬體改裝](#韌體與硬體改裝)
- [切片、設定檔與 G-code](#切片設定檔與-g-code)
- [列印農場與佇列](#列印農場與佇列)
- [線材、AMS 與 RFID](#線材ams-與-rfid)
- [鏡頭與縮時](#鏡頭與縮時)
- [儀表板、螢幕與 App](#儀表板螢幕與-app)
- [橋接與 AI 代理](#橋接與-ai-代理)
- [閉源／商業（對照用）](#閉源商業對照用)
- [相關列表](#相關列表)
- [貢獻](#貢獻)
- [授權](#授權)

---

## 官方開源（bambulab）

- **[BambuStudio](https://github.com/bambulab/BambuStudio)** — 官方切片軟體（開源）。

## 區網模式、API 與函式庫

- **[OpenBambuAPI](https://github.com/Doridian/OpenBambuAPI)** — API 文件。
- **[bambulabs_api](https://github.com/BambuTools/bambulabs_api)** — 非官方 Python API。
- **[bambulabs_api](https://github.com/torbenconto/bambulabs_api)** — 非官方 Go 綁定。
- **[bambulab](https://github.com/markhaehnel/bambulab)** — Rust API 客戶端。
- **[pybambu](https://github.com/greghesp/pybambu)** — HA 整合所用的 Python 函式庫。
- **[bambu-printer-manager](https://github.com/synman/bambu-printer-manager)** — 純 Python 印表機管理函式庫。
- **[bambu-connect](https://github.com/mattcar15/bambu-connect)** — 讀取狀態、控制與鏡頭。
- **[Bambu-Lab-Cloud-API](https://github.com/coelacant1/Bambu-Lab-Cloud-API)** — Bambu 雲端 API 分析。
- **[open-bamboo-networking](https://github.com/ClusterM/open-bamboo-networking)** — 取代 Bambu Studio 專有網路外掛的開源實作。
- **[bambu-farm](https://github.com/ellenhp/bambu-farm)** — 可自架的 Bambu Cloud 替代。
- **[open-bambu-networking-plugin](https://github.com/persano/open-bambu-networking-plugin)** — OrcaSlicer 開源網路外掛：雲端列印、遠端鏡頭、AMS 同步。
- **[bambu-proxy](https://github.com/disconn3ct/bambu-proxy)** — MQTT 代理，讓多個客戶端共用一台 Bambu 印表機連線。
- **[bambulab-virtual-printer](https://github.com/tbc0309/bambulab-virtual-printer)** — 本地 Bambu 印表機與 AMS MQTT 模擬器，附網頁管理介面，不需真機即可測試客戶端。

## Home Assistant 與自動化

- **[ha-bambulab](https://github.com/greghesp/ha-bambulab)** — HA 整合。
- **[ha-bambu-lab-p1-spaghetti-detection](https://github.com/nberktumer/ha-bambu-lab-p1-spaghetti-detection)** — 炒麵偵測整合。
- **[Bambu-HomeAssistant-Flows](https://github.com/WolfwithSword/Bambu-HomeAssistant-Flows)** — HA 儀表板與 Node-RED 流程。
- **[printwatch-card](https://github.com/drkpxl/printwatch-card)** — 監控印表機的 HA 卡片。
- **[SpoolmanSync](https://github.com/gibz104/SpoolmanSync)** — 透過 HA 自動同步 Spoolman。
- **[HA-Panda-PWR](https://github.com/62fixolab/HA-Panda-PWR)** — BIGTREETECH Panda PWR 智慧插座的 Home Assistant 整合。
- **[homeassistant-app-bambuddy](https://github.com/Spegeli/homeassistant-app-bambuddy)** — 把 BamBuddy 包成 Home Assistant App（Supervisor）。
- **[ha-bambulab-blueprints](https://github.com/pleasantone/ha-bambulab-blueprints)** — Home Assistant 藍圖：濾網耗損追蹤、自動斷電、腔室加熱安全與列印通知。
- **[universal-3d-cards](https://github.com/Rein033/universal-3d-cards)** — 支援 Bambu Lab 等印表機的 Home Assistant 儀表板卡片，有繪製的印表機、即時鏡頭與實際顏色的 AMS 線軸。
- **[3d-printdash](https://github.com/Freaky-Jay-22/3d-printdash)** — 以 Home Assistant App 或 Docker 執行的本地儀表板，並排管理 Bambu Lab 與 Klipper 印表機，內建線材管理、鏡頭與列印紀錄。

## 韌體與硬體改裝

- **[X1Plus](https://github.com/X1Plus/X1Plus)** — X1／X1C 自製韌體。
- **[Bambu-Lab-Klipper-Conversion](https://github.com/ChazLayyd/Bambu-Lab-Klipper-Conversion)** — 換掉主板改跑 Klipper。
- **[BMCU-C-PJARCZAK](https://github.com/jarczakpawel/BMCU-C-PJARCZAK)** — 給 A1／A1 mini／P1S 的 BMCU 韌體。
- **[Bambu-Bus](https://github.com/Bambu-Research-Group/Bambu-Bus)** — Bambu Bus 工具與文件。
- **[x1-expander](https://github.com/jwise/x1-expander)** — X1 Carbon 擴充板。
- **[OpenBL](https://github.com/opensourcemanufacturing/OpenBL)** — 印表機軟硬體探索。
- **[bambu-cuts](https://github.com/unrelatedlabs/bambu-cuts)** — A1 mini 切割與繪圖。
- **[BambuScribe](https://github.com/Animesh-Varma/BambuScribe)** — 把 Bambu 印表機安全變成筆式繪圖機，產生自訂 G-code。
- **[Bambu-Poop-Conveyor-ESP32](https://github.com/t0nyz0/Bambu-Poop-Conveyor-ESP32)** — ESP32 廢料輸送帶。
- **[PandaStatusOS](https://github.com/jeremykenedy/PandaStatusOS)** — BIGTREETECH Panda Status P2 燈條的 clean-room 開源韌體。
- **[ReBLLED](https://github.com/brossow/ReBLLED)** — BLLED ESP32 燈條控制器的替代韌體，自動點亮機箱並顯示列印狀態。

## 切片、設定檔與 G-code

- **[OrcaSlicer](https://github.com/OrcaSlicer/OrcaSlicer)** — 對 Bambu 支援完整的開源切片。
- **[OrcaSlicer-bambulab](https://github.com/FULU-Foundation/OrcaSlicer-bambulab)** — 聚焦 Bambu 的 OrcaSlicer 版本。
- **[OrcaStudio](https://github.com/jarczakpawel/OrcaStudio)** — 合入 OrcaSlicer 改動的 Bambu Studio 分支。
- **[bambulab-studio-orca-slicer-presets](https://github.com/DRIgnazGortngschirl/bambulab-studio-orca-slicer-presets)** — 社群設定檔集合。
- **[Bambu_CustomGCode](https://github.com/eukatree/Bambu_CustomGCode)** — 自訂 G-code。
- **[Filament_Calibration_Wizard](https://github.com/Django1982/Filament_Calibration_Wizard)** — 線材校正精靈。
- **[Bricklayers](https://github.com/TengerTechnologies/Bricklayers)** — 磚式層疊後處理腳本。
- **[StudioBridge](https://github.com/Rdiger-36/StudioBridge)** — 把其他帳號的印表機加入 Bambu Studio。
- **[docker-orcaslicer](https://github.com/linuxserver/docker-orcaslicer)** — 可用瀏覽器開的 OrcaSlicer 容器。
- **[docker-bambustudio](https://github.com/linuxserver/docker-bambustudio)** — 可用瀏覽器開的 Bambu Studio 容器。
- **[layer-rescue](https://github.com/EmirhanSyl/layer-rescue)** — 從任意層續印失敗作品的 Bambu Studio 後處理腳本。
- **[preset-porter](https://github.com/OMRITGM/preset-porter)** — 瀏覽器工具，修復換印表機後在 Bambu Studio 變成「不支援」的線材預設。
- **[shambu](https://github.com/Shavvimal/shambu)** — 建立、檢查與修補 Bambu Studio .3mf 專案並無頭切片的 CLI 與 Claude Code 外掛。
- **[PausePalette](https://github.com/DanaLeeTech/PausePalette)** — 規劃顏色順序並插入換線暫停，讓列印顏色數超過 AMS 槽位數。
- **[pandy-slicer](https://github.com/gccammelli/pandy-slicer)** — 把 Bambu Studio 命令列切片包成 Home Assistant add-on 或 Docker 容器，讓 Pandy App 在 LAN-only 模式列印 MakerWorld 模型。

## 列印農場與佇列

- **[bambuddy](https://github.com/maziggy/bambuddy)** — 自架控制中心。
- **[bambu-farm](https://github.com/TFyre/bambu-farm)** — 多台印表機網頁介面。
- **[fdm-monster](https://github.com/fdm-monster/fdm-monster)** — 印表機農場管理平台。
- **[print-farm-manager](https://github.com/joeltelling/print-farm-manager)** — 多品牌自架農場管理。
- **[bambu-gateway](https://github.com/leolobato/bambu-gateway)** — 自架區網網頁與 REST API，監看並送印 Bambu 印表機。
- **[fabrica](https://github.com/wsturner88/fabrica)** — 本地多品牌列印農場儀表板，含鏡頭、AMS 線材控制與給 AI 代理的 MCP 工具。

## 線材、AMS 與 RFID

- **[RFID-Tag-Guide](https://github.com/Bambu-Research-Group/RFID-Tag-Guide)** — 讀取線材標籤。
- **[Bambu-Lab-RFID-Library](https://github.com/queengooborg/Bambu-Lab-RFID-Library)** — 線材標籤掃描資料庫。
- **[OpenSpool](https://github.com/spuder/OpenSpool)** — 開源線材 RFID。
- **[openspoolman](https://github.com/drndos/openspoolman)** — 結合 Bambu NFC 的 Spoolman。
- **[bambu-spoolman](https://github.com/mrkirby153/bambu-spoolman)** — Spoolman 的 Bambu 整合。
- **[HaspelSync](https://github.com/Rdiger-36/HaspelSync)** — 追蹤線材用量。
- **[flipper-bambu](https://github.com/uzyn/flipper-bambu)** — Flipper Zero 線材 NFC 解析。
- **[bambu-spoolman-bridge](https://github.com/Yarasarda/bambu-spoolman-bridge)** — 不必切成純區網模式即可把第三方線材用量同步到 Spoolman。
- **[TigerTag-Studio-Manager](https://github.com/TigerTag-Project/TigerTag-Studio-Manager)** — TigerTag 開源 NFC 標準的桌面印表機與線材管理。
- **[TigerSpool-RFID](https://github.com/TigerTag-Project/TigerSpool-RFID)** — ESP32＋PN532 線材 RFID 掃描器，掃完對應到印表機槽位。
- **[bambu-ams-spool-sync](https://github.com/demonkazuya/bambu-ams-spool-sync)** — Home Assistant 整合，把 Spoolman Sync 的線材指派推送到 Bambu AMS 槽位。

## 鏡頭與縮時

- **[BambuP1Streamer](https://github.com/slynn1324/BambuP1Streamer)** — P1 的 MJPEG 串流。
- **[bambu-go2rtc](https://github.com/synman/bambu-go2rtc)** — go2rtc 串流。
- **[BambuSource2Raw](https://github.com/hisptoot/BambuSource2Raw)** — X1／P1P 原始鏡頭串流。
- **[BambuCAM](https://github.com/BangerTech/BambuCAM)** — 多台鏡頭監看網頁。

## 儀表板、螢幕與 App

- **[BambuHelper](https://github.com/Keralots/BambuHelper)** — ESP32 桌面監看器。
- **[PrintSphere](https://github.com/cptkirki/PrintSphere)** — 圓形 ESP32-S3 狀態顯示。
- **[CYD-Klipper](https://github.com/suchmememanyskill/CYD-Klipper)** — 無線狀態螢幕。
- **[BambUI](https://github.com/fidoriel/BambUI)** — 區網模式開源 UI。
- **[openbu](https://github.com/cygnusx-1-org/openbu)** — 開發者模式 Android App。
- **[panda-be-free](https://github.com/MiguelSchulz/panda-be-free)** — 開源 iOS 儀表板。
- **[BambuBoard](https://github.com/t0nyz0/BambuBoard)** — 近即時網頁儀表板。
- **[Bambulabs-Exporter](https://github.com/Aetrius/Bambulabs-Exporter)** — Prometheus exporter。
- **[xtouch](https://github.com/xperiments-in/xtouch)** — 控制與監看 Bambu Lab 印表機的 ESP32 觸控螢幕韌體。
- **[PrintGlance](https://github.com/talic/PrintGlance)** — Mac 選單列 App，區網顯示 Bambu 列印進度與暫停／失敗原因。
- **[toothpeek](https://github.com/loicbisiere/toothpeek)** — Mac 選單列 App，區網顯示 Bambu 印表機即時鏡頭、列印進度與通知。
- **[print-heatmap](https://github.com/artemnovichkov/print-heatmap)** — 把 Bambu 列印紀錄畫成 GitHub 風格熱度圖，放在個人 README 或釘選 gist。
- **[BambuBar](https://github.com/GuoDaiYi/BambuBar)** — 原生 macOS 選單列監看工具，透過 Bambu 雲端帳號顯示進度、層數、剩餘時間與溫度。

## 橋接與 AI 代理

- **[OctoPrint-OctoEverywhere](https://github.com/QuinnDamerell/OctoPrint-OctoEverywhere)** — 支援 Bambu 的遠端存取。
- **[OctoPrint-BambuPrinter](https://github.com/jneilliii/OctoPrint-BambuPrinter)** — 連接 Bambu Lab 印表機的 OctoPrint 外掛。
- **[bambu-printer-mcp](https://github.com/DMontgomery40/bambu-printer-mcp)** — Bambu 的 MCP server。
- **[bambu-mcp](https://github.com/griches/bambu-mcp)** — 多機控制 MCP server。
- **[bambu](https://github.com/voska/bambu)** — 從終端機切片、預檢、送印與監看的區網 CLI，適合 AI 代理。
- **[Kiln](https://github.com/codeofaxel/Kiln)** — 讓 AI 代理設計、切片並在 Bambu 等印表機列印的 MCP server。
- **[bamboozle](https://github.com/nxmxbbd/bamboozle)** — 僅用區網的 Apple Home 橋接，在 HomeKit 顯示 Bambu 印表機的進度、狀態與鏡頭，不需 Home Assistant 或 Homebridge。
- **[printshop-mcp](https://github.com/FireBall1725/printshop-mcp)** — Bambuddy 與 Spoolman 的 MCP 伺服器，讓 AI 代理查線材庫存、送出已切片 3MF 並追蹤列印。
- **[bambustudio-mcp](https://github.com/subhashdasyam/bambustudio-mcp)** — Bambu Studio 切片軟體的 MCP 伺服器，可從 Claude Code 或 Codex 檢視零件、設定已存的 3MF 專案並比較切片結果。

## 閉源／商業（對照用）

- **[Bambu Handy](https://bambulab.com/en/download)** — 官方手機 App。
- **[MakerWorld](https://makerworld.com)** — 官方模型平台。

## 相關列表

- [neardws/awesome-bambu](https://github.com/neardws/awesome-bambu) — 較早的小型清單。
- [Awesome](https://github.com/sindresorhus/awesome)

## 貢獻

歡迎開 PR 或 issue。每條一行、需開源且切題、直接連到倉庫、不放星數。閉源／商業只放對照區。

## 授權

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

在法律允許範圍內，貢獻者放棄本作品的所有著作權。
