---
title: "感光元件與片幅 (Sensor & Crop Factor)"
aliases: ["片幅", "全片幅", "APS-C", "Crop Factor", "Sensor Size", "裁切係數"]
tags:
  - photography
  - gear
  - sensor
  - optics
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-understanding-camera-lenses.pdf"
  - "raw/fotobeginner-113-photography-terms.pdf"
---

# 感光元件與片幅 (Sensor & Crop Factor)

## 一句話核心定義
感光元件（Sensor）是數位相機捕捉光線成像的心臟，其**物理尺寸大小（片幅）** 直接決定了視野裁切比例（Crop Factor）、鏡頭等效焦距、高 ISO 雜訊表現與景深特性。

---

## 主流感光元件尺寸對比

現代攝影領域以傳統 35mm 底片規格作為黃金標準基準：

| 片幅名稱 | 實體感光元件尺寸 | 裁切係數 (Crop Factor) | 特點與市場定位 |
| :--- | :--- | :---: | :--- |
| **中片幅 (Medium Format)** | 43.8 x 32.9 mm 等 | 約 0.79x | 頂級商業廣告、極致畫質與超高解析度（數千萬至一億像素） |
| **全片幅 (Full-frame / FF)** | **36 x 24 mm** (基準) | **1.0x** | 專業攝影師與進階發燒友標準；無裁切、動態範圍廣、高感純淨 |
| **APS-C (裁切片幅)** | 約 23.6 x 15.6 mm | **1.5x (Sony/Nikon/Fuji)**<br>**1.6x (Canon)** | 體積、重量與畫質的極佳平衡；入門與中階相機主流 |
| **微單四分之三 (Micro Four Thirds / M4/3)** | 17.3 x 13.0 mm | **2.0x** | 機身與鏡頭極輕巧，遠攝望遠倍率高，微距與防手震表現優異 |
| **智慧型手機 / 1吋感光元件** | 約 13.2 x 8.8 mm 或更小 | 約 2.7x ~ 7x+ | 便攜性最高，但受限於物理進光量，需強烈仰賴運算攝影 |

---

## 什麼是「裁切係數 (Crop Factor)」與「等效焦距」？

當你把一支專為全片幅設計的 50mm 鏡頭接在 APS-C 相機上時：
* 鏡頭投射的光學圓形影像依然相同，但因 APS-C 的感光元件面積較小，它只錄取了中間區域，邊緣被裁切掉。
* 視野（Angle of View）變窄，看起來宛如在全片幅上使用更長焦段的鏡頭！

> **等效焦距計算公式**：
> $$\text{等效焦距 (35mm Equivalent)} = \text{實體鏡頭焦距} \times \text{裁切係數 (Crop Factor)}$$

### 經典計算範例：
* 一支 50mm 鏡頭裝在 Sony APS-C 機身（係數 1.5x）上：
  $$50\text{mm} \times 1.5 = \mathbf{75\text{mm 等效視野}}$$（從標準視角變成了人像中望遠視角！）
* 一支 18-55mm 典型套裝鏡頭裝在 Canon APS-C（係數 1.6x）上：
  $$18\text{mm} \sim 55\text{mm} \times 1.6 = \mathbf{28.8\text{mm} \sim 88\text{mm 等效視野}}$$。

---

## 片幅大小對拍攝質感的深遠影響

1. **高感光度純淨度（訊噪比 SNR）**：
   * 全片幅感光元件面積是 APS-C 的 2.25 倍以上。在相同像素下，全片幅的每個「單一像素感光單元（Pixel Pitch）」更大，能收集更多光子，因此在夜間高 ISO（如 ISO 6400）下雜訊遠少於裁切片幅。
2. **同等視角下的景深更淺**：
   * 要在全片幅和 APS-C 上拍出完全一樣視角與構圖的照片，全片幅需要更長的物理焦距或站得更近，這兩者都會讓全片幅拍出來的**[[景深與彌散圓|景深更淺、背景散景更虛化]]**。

---

## 相關概念與延伸閱讀
* [[單眼與無反 (DSLR vs Mirrorless)]] - 現代感光元件載體系統
* [[焦距與視角 (Focal Length & Angle of View)]] - 焦段與裁切視野的換算
* [[01-exposure/感光度 (ISO)]] - 感光元件面積與雜訊的底層關係
* [[景深與彌散圓 (Depth of Field & Circle of Confusion)]] - 彌散圓標準如何依片幅縮放
