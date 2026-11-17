---
title: "曝光微調與高光陰影還原 (Exposure & Dynamic Range Recovery)"
aliases: ["曝光還原", "高光陰影", "動態範圍救援", "Exposure Compensation", "Highlight Recovery", "Shadow Recovery"]
tags:
  - photography
  - post-processing
  - exposure
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-digital-photo-editing-workflow.pdf"
  - "raw/cambridge-camera-exposure.pdf"
---

# 曝光微調與高光陰影還原 (Exposure & Dynamic Range Recovery)

## 一句話核心定義
在數位暗房的第二步中，透過**曝光補償 (Exposure)、高光壓暗 (Highlights Recovery) 與陰影提亮 (Shadow Recovery)** 三重滑桿，客觀對照直方圖，挽救前期拍攝時險些丟失的極限明暗細節。

---

## 核心調整四重奏（Lightroom 核心四滑桿）

```text
直方圖分佈:
 [ 黑階 (Blacks) ] ── [ 陰影 (Shadows) ] ── [ 曝光 (Exposure/中間調) ] ── [ 高光 (Highlights) ] ── [ 白階 (Whites) ]
```

1. **總曝光 (Exposure)**：
   * 等效於在前期微調相機的曝光補償。它主要推動整個**中間調（Midtones）** 的明暗，決定整張照片的基調。
2. **高光壓暗 (Highlights Recovery)**：
   * 專門針對畫面中最明亮但尚未完全死白溢出的區域（如天空白雲、陽光反射邊緣、皮膚反光高光點）進行精準壓暗。
   * **成效**：將泛白的天空雲層紋理重新拉回，展現豐富的層次感。
3. **陰影提亮 (Shadow Recovery)**：
   * 專門針對畫面中背光、陰暗但尚未完全死黑的區域（如陰影中的岩石、樹葉、背光人像臉部）進行提升。
   * **代價注意**：大幅提亮陰影（例如 +80）會不可避免地暴露隱藏在暗部的電子雜訊，後續必須搭配 **[[降噪與銳化平衡|數位降噪]]**！
4. **白色剪裁與黑色剪裁 (Whites / Blacks)**：
   * 定位整張照片的最黑點（Black Point）與最白點（White Point），確保照片擁有扎實的對比基底，防止畫面發灰。

---

## 嚴格警惕：過度補償的畫質懲罰

* **過度提亮暗部（+100 暴力硬拉）**：
  * 暗部細節雖然浮現，但會伴隨濃重的彩色噪點，暗部色彩嚴重發灰、失去飽和度，整張照片看似洗水褪色。
* **高光死白不可逆**：
  * 若前期拍攝時直方圖最右側早已嚴重撞牆（高光三原色全部溢出為 255/255/255），此時將高光滑桿拉到最底，拉回來的只會是一團**死寂難看的灰白色斑塊**，因為感光元件在此處根本沒有記錄下任何數位資訊！

---

## 相關概念與延伸閱讀
* [[數位後製標準十步工作流 (10-Step Workflow)]] - 曝光還原的工序定位
* [[01-exposure/測光系統與直方圖 (Metering & Histogram)]] - 透過直方圖直觀監視高光與陰影溢出
* [[降噪與銳化平衡 (Noise Reduction vs Sharpening)]] - 提亮陰影後必須進行的噪點壓制
