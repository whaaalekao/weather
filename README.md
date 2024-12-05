# 天氣查詢應用程式

這是一個使用 Vue.js 製作的簡易天氣查詢應用，能根據使用者輸入的地點提供當前的天氣資訊。應用程式使用 OpenWeatherMap API 獲取即時天氣數據，並以簡潔設計進行展示。

## 功能特點

- **地點天氣查詢**：透過城市名稱查詢該地點的天氣資訊。
- **動態背景**：根據溫度變化背景顏色，溫度高於 16°C 時顯示暖色背景。
- **日期顯示**：以友好的格式顯示當前日期。

## 使用技術

- Vue.js
- JavaScript
- HTML 和 CSS
- OpenWeatherMap API

## 項目設置

1. 將此專案複製到本地端：
    ```bash
    git clone https://github.com/whaaalekao/weather
    ```

2. 進入專案目錄：
    ```bash
    cd weather
    ```
   ```bash
    cd vue-weather
    ```

4. 安裝相依套件：
    ```bash
    npm install
    ```

5. 啟動開發模式：
    ```bash
    npm run dev
    ```

## 使用方式

- **查詢天氣**：在搜尋欄位輸入城市名稱並按下 "Enter" 鍵，即可顯示該地點的天氣。
- **動態背景**：當溫度高於 16°C 時，背景自動轉為暖色調，否則顯示冷色背景。

## 代碼概述

### `App.vue`

- **Template（模板）**：包含應用的結構，包括搜尋欄和天氣資訊顯示區。
- **Script（腳本）**：使用 Vue.js 建立功能，包含調用 OpenWeatherMap API 取得天氣資料並顯示的方法。
- **Style（樣式）**：自訂 CSS 樣式，根據溫度變化動態切換背景。

### 主要方法

- **fetchWeather**：觸發 API 調用，根據使用者輸入的查詢地點獲取天氣數據。
- **setResults**：API 返回數據後更新天氣資訊的狀態。
- **dateBuilder**：一個輔助函數，用於顯示當前日期的格式化方式。

### API 整合

此應用使用 [OpenWeatherMap API](https://openweathermap.org/api) 來獲取天氣數據。請在 `App.vue` 中的 `data()` 內填入從 OpenWeatherMap 獲取的 API 金鑰。

## 授權

此專案為開源項目，並採用 [MIT License](LICENSE) 授權。
