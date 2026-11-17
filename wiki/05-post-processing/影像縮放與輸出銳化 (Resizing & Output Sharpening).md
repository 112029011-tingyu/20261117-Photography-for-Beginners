---
title: "影像縮放與輸出銳化 (Resizing & Output Sharpening)"
aliases: ["縮放與輸出銳化", "輸出銳化", "影像內插", "Resizing", "Output Sharpening", "Interpolation", "Moiré"]
tags:
  - photography
  - post-processing
  - export
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-digital-photo-editing-workflow.pdf"
---

# 影像縮放與輸出銳化 (Resizing & Output Sharpening)

## 一句話核心定義
這是後製流程的**最後第九與第十道終極工序**；根據終端用途（實體大圖輸出列印 vs 網路社群螢幕觀看）進行數位重採樣縮放，並客製化施加**輸出銳化 (Output Sharpening)**，以補償縮放與印刷介質帶來的物理軟化。

---

## 一、 影像縮放策略：放大 (Upsizing) vs 縮小 (Downsizing)

改變像素尺寸的數學過程稱為「數位影像內插 (Digital Image Interpolation)」：

### 1. 放大列印 (Upsize for Print)
* **黃金守則**：**永遠由攝影師自己在軟體中完成尺寸放大，切勿交給印表機驅動程式胡亂插值！** 印表機硬體內插容易出現生硬的馬賽克與鋸齒。
* 放大時使用「雙三次雙平滑 (Bicubic Smoother)」或 AI 超解析度演算法，能維持平滑的斜線邊緣。

### 2. 縮小發布 (Downsize for Web / Social Media)
* **避開摩爾紋 (Moiré Artifacts)**：縮圖演算法若過於粗暴，磚牆、百葉窗或密集西裝紋理會產生彩色的網紋干涉（摩爾紋）。
* 縮圖時採用「雙三次較銳利 (Bicubic Sharper)」，確保線條在手機螢幕上清晰緊湊。

---

## 二、 擷取銳化 vs 輸出銳化 (Capture vs Output Sharpening)

許多新手不知道，專業暗房中**銳化必須分開執行兩次**：

```text
[原始 RAW 檔] ──► 【第一道：擷取銳化 (Capture Sharpening)】──► 補償鏡頭與感光元件低通濾鏡造成的原始光學微軟化
      │
[中間編修、調色、降噪、裁切、尺寸縮放完成]
      │
      ▼
【第二道：輸出銳化 (Output Sharpening)】──► 依據「發布媒介」定制最後的微觀邊緣反差！
```

* **螢幕觀看輸出 (For Screen)**：適度強化微對比，抵抗社群平台（如 Instagram/Facebook）二次壓縮帶來的軟化。
* **相紙印刷輸出 (For Print)**：
  * **亮面相紙 (Glossy)**：需要中等強度的銳化。
  * **霧面/棉紙 (Matte Paper)**：墨水滲入紙張纖維時會自然向外毛細擴散，導致圖像邊緣變鈍。因此**霧面紙必須施加顯著更強的輸出銳化**，印出來才會剛好銳利如常！

---

## 相關概念與延伸閱讀
* [[數位後製標準十步工作流 (10-Step Workflow)]] - 十步工作流的完結階段
* [[降噪與銳化平衡 (Noise Reduction vs Sharpening)]] - 前期擷取銳化的控噪原則
* [[02-optics-and-gear/感光元件與片幅 (Sensor & Crop Factor)]] - 原始像素量與大圖輸出的關係
