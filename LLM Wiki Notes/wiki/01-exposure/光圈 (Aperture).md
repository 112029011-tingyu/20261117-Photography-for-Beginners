---
title: "光圈 (Aperture)"
aliases: ["光圈值", "f-number", "f-stop", "Aperture"]
tags:
  - photography
  - exposure
  - optics
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-camera-exposure.pdf"
---

# 光圈 (Aperture)

## 一句話核心定義
光圈是鏡頭內部由多片光圈葉片組成的可調孔徑，負責控制光線穿過鏡頭進入感光元件的**進光面積**，並同時決定畫面的**[[02-optics-and-gear/景深與彌散圓|景深 (Depth of Field)]]**。

---

## 核心原理與數值表示 (f-stop)

光圈大小以 **f 值 (f-number / f-stop)** 來標示（如 f/1.4, f/2, f/2.8...）。初學者最常感到的直覺衝突在於：
* **f 數值越小 = 光圈開孔越大（大光圈 / Large Aperture）** $\rightarrow$ 進光量多、景深淺（背景虛化）。
* **f 數值越大 = 光圈開孔越小（小光圈 / Small Aperture）** $\rightarrow$ 進光量少、景深深（前後皆清晰）。

### 為什麼 f 數值是倒數比例？
f 值的物理定義為：
$$\text{f-stop} = \frac{\text{鏡頭焦距 (Focal Length)}}{\text{光圈有效孔徑直徑 (Entrance Pupil)}}$$

因此，當孔徑直徑越大時，分母越大，算出來的數值（f-stop）反而越小。

### 標準光圈級數（全檔光圈級距）
光圈面積每放大一倍（進光量翻倍，即增加 1 個 [[曝光級數 (Exposure Stops)|Stop]]），直徑需乘以 $\sqrt{2} \approx 1.414$。常見的標準全檔光圈序列如下：

$$\mathbf{f/1.0 \rightarrow f/1.4 \rightarrow f/2.0 \rightarrow f/2.8 \rightarrow f/4.0 \rightarrow f/5.6 \rightarrow f/8.0 \rightarrow f/11 \rightarrow f/16 \rightarrow f/22}$$

> **進光量對照範例**：
> 在相同快門與 ISO 下，**f/1.4 的進光量是 f/2.8 的 4 倍**（相差 2 級曝光 Stop），更是 **f/16 的 128 倍**！

---

## 視覺效果與實戰影響

1. **景深控制 (Depth of Field)**：
   * **大光圈 (如 f/1.4 ~ f/2.8)**：景深極淺，主體清晰而背景呈現柔和漂亮的**[[02-optics-and-gear/散景 (Bokeh)|散景 (Bokeh)]]**，極適合特寫、人像攝影。
   * **小光圈 (如 f/8 ~ f/16)**：景深極深，前景到遠景皆在清晰範圍內，常用於壯麗的風景攝影、建築攝影。
2. **快門速度解放（大光圈又稱「大光圈快速鏡頭 Fast Lens」）**：
   * 因為大光圈通光量大，在昏暗環境或室內，能讓相機使用更快的 **[[快門速度 (Shutter Speed)]]**，有效避免手震模糊與凍結動作。
3. **畫質甜區（最佳光圈 Sweet Spot）**：
   * 光圈全開時（如最大光圈 f/1.4），鏡頭像差往往較明顯，且四角容易出現**[[02-optics-and-gear/光學像差與瑕疵 (Optical Aberrations)|暗角 (Vignetting)]]**。
   * 縮小 1 到 2 檔光圈（例如 f/4 到 f/8），通常能達到鏡頭中央與邊緣銳利度最高的「畫質甜區」。
   * 過度縮小光圈（超過 f/16 或 f/22）會引發光學**繞射現象 (Diffraction)**，反而導致整個畫面解析度軟化下降。

---

## 新手常用設定建議

| 拍攝題材 | 推薦光圈範圍 | 核心考量 |
| :--- | :--- | :--- |
| **單人人像 / 特寫** | f/1.4 - f/2.8 | 虛化雜亂背景，突出人物眼神與主體 |
| **日常街拍 / 紀實** | f/4.0 - f/5.6 | 保證主體清晰，兼具適度環境脈絡與鏡頭銳利度 |
| **團體合照 (多排)** | f/5.6 - f/8.0 | 避免站在前後排的人臉因景深過淺而脫焦模糊 |
| **大景風景 / 建築** | f/8.0 - f/11 | 追求畫面從近到遠全景清晰與最高解像力 |
| **夜景星芒 (星芒效果)** | f/11 - f/16 | 利用小光圈讓強光源繞射出漂亮的光芒線條 |

---

## 相關概念與延伸閱讀
* [[曝光三要素 (Exposure Triangle)]] - 曝光系統的黃金三角
* [[曝光級數 (Exposure Stops)]] - 計算光圈檔位進光量的翻倍原則
* [[相機拍攝模式 (Camera Modes)]] - 新手最推薦的「光圈先決 (Av/A)」實戰
* [[02-optics-and-gear/景深與彌散圓]] - 深入剖析景深的物理本質
* [[02-optics-and-gear/定焦鏡與變焦鏡]] - 為什麼定焦鏡更容易做到大光圈
