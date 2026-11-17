---
title: "高動態範圍與包圍曝光 (Bracketing & HDR)"
aliases: ["包圍曝光", "HDR", "高動態範圍", "Bracketing", "High Dynamic Range", "BKT"]
tags:
  - photography
  - techniques
  - exposure
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-camera-exposure.pdf"
  - "raw/fotobeginner-113-photography-terms.pdf"
---

# 高動態範圍與包圍曝光 (Bracketing & HDR)

## 一句話核心定義
**包圍曝光 (Auto-Exposure Bracketing / AEB)** 是指相機連續以不同曝光設定拍下「一暗、一準、一亮」的多張照片；而在電腦後製中將其融合成一張同時擁有深邃暗部與純淨亮部細節的技術，即稱為 **高動態範圍成像 (High Dynamic Range / HDR)**。

---

## 為什麼需要 HDR？（感光元件動態範圍的物理極限）

人類眼睛具有超過 20 級 (Stops) 的驚人動態範圍適應力，我們能同時看清晴朗大太陽下的白雲細節，又能看清背陰大樹下的苔蘚。
* 然而，現代頂級全片幅相機單次曝光的**動態範圍 (Dynamic Range)** 通常僅有 12~14 級。
* 面對強烈光差場景（例如：大白天從室內透過落地窗拍窗外風景、或是日出大逆光下的山巒）：
  * **照顧地面** $\rightarrow$ 天空慘白一片（高光死白，無細節）。
  * **照顧天空** $\rightarrow$ 地面漆黑一片（暗部死黑，滿是雜訊）。

---

## 解決方案：包圍曝光三部曲

```text
【相機自動包圍曝光 (BKT)】
  ├── 欠曝張 (-2 EV)：壓暗整體，專門記錄天空夕陽雲彩的完美層次 (防止死白)
  ├── 正常張 ( 0 EV)：記錄中間調地景
  └── 過曝張 (+2 EV)：暴力提亮，專門汲取陰影暗部岩石的細膩紋理 (防止死黑)
          │
          ▼ 在 Lightroom / Photoshop / 專用軟體中【合成 HDR (Photo Merge HDR)】
  【生成極致 HDR 相片】：同時呈現最純淨的夕陽天空，與層次豐富的暗部地景，無雜訊無死白！
```

---

## 新手實戰避坑法則

1. **必須保持畫面絕對靜止**：
   * 拍攝多張照片合成時，若相機震動或畫面中有行人走動、樹葉劇烈搖晃，合成時會產生嚴重的重影（鬼影 Ghosting）。**請務必架設穩固三腳架！**
2. **切忌「HDR 審美中毒」**：
   * 很多新手初學 HDR 後製時，喜歡把陰影拉到最亮、高光壓到最暗，讓畫面毫無陰影，反差全無，整張照片發灰發髒、邊緣泛起詭異的白色光暈（偽 HDR 風格）。
   * **最高境界的 HDR**：看起來自然真實，宛如親臨現場人眼所見的舒適明暗平衡！

---

## 相關概念與延伸閱讀
* [[01-exposure/測光系統與直方圖 (Metering & Histogram)]] - 檢測高光與陰影死黑死白的客觀工具
* [[03-lighting-and-accessories/攝影濾鏡 (Photography Filters)]] - 前期光學濾鏡 GND 與後期數位 HDR 的抗衡
* [[05-post-processing/數位後製標準十步工作流 (10-Step Workflow)]] - 數位暗房處理 HDR 的標準工序
