# 金線圖樣產生器 Goldline Pattern Generator

以 WebGL 即時描繪的金線幾何動畫工具。每個版本都是單一 HTML 檔，不需要安裝或伺服器端程式，用瀏覽器開啟即可使用。

| 檔案 | 說明 |
|---|---|
| `goldline-generator.html` | 第一版：原圖、隨機產生、匯入 SVG |
| `goldline-generator-v2.html` | V2：隨機產生、匯入 SVG（不含原圖）、匯入畫面比例不限 |
| `index.html` | 入口頁，連到上面兩個版本 |

# 金線圖樣產生器-V2版 Goldline Pattern Generator-V2
https://maxxkao.github.io/goldline-generator/goldline-generator-v2.html

## 功能

- **金線描繪動畫**：多支筆同時描線，筆頭發光、火花粒子、餘光漸退；實心色塊以掃入方式填滿。
- **兩條獨立控制**：「線條出現」與「英文字出現」可分別拖曳到任意進度，另有時間軸。
- **隨機產生**：依黃金比例切割版面，圓弧只使用正圓的 1/4、1/2、3/4 與整圓，斜線一律 45°，端點都落在格線上。可切換聖誕、新年、裝飾藝術三套圖樣庫，並調整圖樣密度與填色密度。
- **匯入 SVG**：支援直線、曲線、圓、矩形、多邊形、群組變形與挖空形狀；可依圖層順序或由一點擴散描線。
- **文字**：打字機、逐字淡入、逐字上浮三種效果；可調字體大小、行距與位置。
- **顏色**：底圖與線條顏色皆可自訂。
- **輸出**：錄製 MP4（瀏覽器不支援時改為 WebM）、下載 SVG。

## 使用方式

直接用瀏覽器開啟 HTML 檔，或透過 GitHub Pages 開啟網址。

- 建議使用新版 Chrome、Edge、Safari 或 Firefox（需支援 WebGL2）。
- 手機要把影片存到相簿，網址必須是 HTTPS（GitHub Pages 預設即為 HTTPS）。
- 錄影時請保持畫面開啟，不要切換分頁或 App。

## 第三方元件

- [earcut](https://github.com/mapbox/earcut) 2.2.4 — ISC License, Copyright (c) 2016 Mapbox（已內嵌於 HTML 中，用於實心形狀三角化）
- [Inter](https://rsms.me/inter/) 字型 — SIL Open Font License 1.1（由 Google Fonts 載入，無法連線時改用 Arial）
