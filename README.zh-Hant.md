# Nyan AI – 您的貓娘風格 Chrome 助理，支援對話式任務自動化 🐾

[中文說明](README.zh-Hant.md) | [English](README.md)

Nyan AI 是一款 **Chrome 擴充功能**，讓一位聰明可愛的 **貓娘 AI 助理** 進駐您的瀏覽器。不只是桌面寵物，Nyan AI 結合 **Live2D 動畫**、**自然語言對話** 與 **目標導向任務自動化**，幫助您完成網頁操作、搜尋資訊，甚至依照您的個人偏好進行智慧化推薦與回應。

![Nyan AI Banner](https://user-images.githubusercontent.com/your-username/your-repo/assets/placeholder_banner.png)

<!-- 建議您放上橫幅圖 -->

[![GitHub issues](https://img.shields.io/github/issues/your-username/ai-nyan-extension)](https://github.com/your-username/ai-nyan-extension/issues)
[![GitHub forks](https://img.shields.io/github/forks/your-username/ai-nyan-extension)](https://github.com/your-username/ai-nyan-extension/network)
[![GitHub stars](https://img.shields.io/github/stars/your-username/ai-nyan-extension)](https://github.com/your-username/ai-nyan-extension/stargazers)
[![License: Apache-2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

## ✨ 主要功能

* **Live2D 虛擬貓娘角色**：

  * 由大型語言模型即時驅動的情緒表情與動畫互動
  * 支援多角色自訂，每位貓娘都有獨立個性設定（見 `roles.json`）

* **語音控制與自然語言對話**：

  * 整合語音辨識（STT）與語音合成（TTS）服務
  * 與 AI 進行自然語言互動、對話理解準確
  * 自訂對嘴引擎讓動畫口型更生動

* **任務導向的智慧助理**：

  * 可理解如「找一間附近適合吃午餐的餐廳」這類自然語言任務
  * 支援多步驟規劃、自動化操作與即時決策

* **瀏覽器網頁互動能力**：

  * 自動點擊、捲動、切換頁籤、填寫表單等瀏覽器操作
  * 擷取與摘要網頁內容並進行語意理解

* **多模態 AI 能力**：

  * **OCR 圖像辨識** – 讀取圖片中的文字
  * **DOM 結構分析** – 以更快速準確的方式處理網頁資料

* **🧩 模組化擴充：喵卡系統**：

  * 透過 JSON 格式「喵卡」新增外觀、個性、任務行為
  * 自訂提示詞：

    * `modelPrompt` 外觀
    * `personalityPrompt` 個性
    * `missionPrompt` 任務

* **個人化推薦與側寫理解**：

  * 根據使用者偏好（如距離容忍度、預算、天氣習慣）進行智慧推薦
  * 結合即時天氣、時間與熱門度自動做出判斷

* **記憶與上下文理解**：

  * 記住使用者名稱、偏好
  * 多輪對話可回顧過往網頁內容與指令紀錄

* **高自訂性設定**：

  * 支援自由設定 LLM API 金鑰、TTS 選項、記憶開關與喵卡安裝

## 🎬 展示範例

*貓娘與使用者互動動畫*

![Nyan AI Demo](https://user-images.githubusercontent.com/your-username/your-repo/assets/demo.gif)

*設定介面畫面擷圖*

![Nyan AI Settings](https://user-images.githubusercontent.com/your-username/your-repo/assets/settings_popup.png)

## 🚀 安裝與使用說明

### 👤 一般使用者

1. 前往 [Chrome 線上應用程式商店]() 下載安裝
2. 點擊瀏覽器右上角 Nyan AI 圖示
3. 使用 Google 帳號登入
4. 設定您的 LLM API 金鑰（建議使用 OpenRouter）
5. 開啟「顯示/隱藏貓咪」開關，即可在任一頁面啟動互動
6. 可透過語音或輸入文字開始對話與操作

### 🧑‍💻 開發者

1. Clone 本專案：

```bash
git clone https://github.com/your-username/ai-nyan-extension.git
```

2. 開啟 `chrome://extensions`
3. 啟用「開發人員模式」
4. 點擊「載入未封裝的擴充功能」，選擇專案資料夾
5. 依照一般使用者步驟完成設定

### 🎤 如何互動

* 點選貓咪旁的麥克風圖示說話
* 在聊天框中輸入文字
* 從 [https://your-website-url.com](https://your-website-url.com) 拖曳「喵卡」至貓咪身上安裝

## 🛠️ 技術架構與使用技術

```
[ 使用者 ] <--> [ Content Script ] <--> [ Background Script ] <--> [ 外部 API（LLM, TTS, Firebase） ]
   (網頁互動)         (狀態管理)                   (語言模型/語音/驗證等)
```

* **語言**：JavaScript (ES6+)
* **Live2D 引擎**：PIXI.js + pixi-live2d-display
* **雲端後端服務**：Firebase
* **OCR 引擎**：Tesseract.js

## 🧩 喵卡系統簡介

「喵卡」是定義 Nyan AI 行為的 JSON 檔案，可以客製：

* 外觀模型（`modelPrompt`）
* 個性語氣（`personalityPrompt`）
* 任務邏輯（`missionPrompt`）

您可前往 [https://your-website-url.com](https://your-website-url.com) 瀏覽、創建並分享喵卡！

## 🤝 貢獻方式

1. Fork 本專案
2. 建立功能分支：`git checkout -b feature/AmazingFeature`
3. 提交變更：`git commit -m 'Add some AmazingFeature'`
4. Push 分支：`git push origin feature/AmazingFeature`
5. 提交 Pull Request！

## 📜 授權

本專案採用 [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0) 授權。

## ❤️ 特別感謝

* 所有 Live2D 模型創作者（皆已於 `roles.json` 中標註）
* PIXI.js 與 pixi-live2d-display 開發者
* Tesseract.js 團隊
* 開源社群的靈感與支持！
