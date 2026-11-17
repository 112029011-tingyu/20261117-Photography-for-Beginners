---
title: "曝光級數 (Exposure Stops)"
aliases: ["曝光檔位", "級數", "EV", "Stop", "Stops"]
tags:
  - photography
  - exposure
  - math
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-camera-exposure.pdf"
---

# 曝光級數 (Exposure Stops)

## 一句話核心定義
在攝影術語中，「級（Stop）」是衡量曝光量的**對數量化單位**：**增加 1 級曝光（+1 Stop）代表進光量翻倍（Double）；減少 1 級曝光（-1 Stop）代表進光量減半（Half）**。

---

## 核心原理：等效曝光與互易法則 (Reciprocity Law)

攝影的核心就是計算進光量。無論你調整的是光圈、快門還是 ISO，只要是以「級（Stop）」為單位，它們對畫面明暗的影響是**完全等價且可以相互補償的**。

> **黃金平衡法則**：
> 如果你把某一要素「降低了 1 級」，只要把另一要素「提高了 1 級」，最終照片的明暗度將維持**完全不變**！

### 範例：獲得相同曝光的三種組合
假設以下組合能達到完美的正常曝光：
1. **基準設定**：`f/4.0`、`1/125s`、`ISO 100`
2. **想虛化背景（開大 2 級光圈）**：
   * 光圈改為 `f/2.0`（+2 Stops，進光量變 4 倍）。
   * 補償：快門必須加快 2 級至 `1/500s`（-2 Stops，時間變 1/4）。
   * $\rightarrow$ 曝光維持不變，但獲得了淺景深。
3. **想凍結飛鳥（加快 3 級快門）**：
   * 快門改為 `1/1000s`（-3 Stops，時間變 1/8）。
   * 補償：ISO 提高 3 級至 `ISO 800`（+3 Stops，增益變 8 倍）。
   * $\rightarrow$ 曝光維持不變，但成功凝固動態。

---

## 三大要素的標準「全檔（Full Stop）」對照表

相機通常允許以 1/3 級為單位微調，但新手必須先牢記最核心的**全檔基準線**：

| 要素 | 減半進光 (-1 Stop) $\longleftarrow$ | **基準點** | $\longrightarrow$ 翻倍進光 (+1 Stop) |
| :--- | :--- | :---: | :--- |
| **[[光圈 (Aperture)]]** (面積翻倍=直徑x1.4) | ... $\leftarrow$ f/11 $\leftarrow$ f/8.0 | **f/5.6** | f/4.0 $\rightarrow$ f/2.8 $\rightarrow$ f/2.0 $\rightarrow$ f/1.4 $\rightarrow$ ... |
| **[[快門速度 (Shutter Speed)]]** (時間等比) | ... $\leftarrow$ 1/500s $\leftarrow$ 1/250s | **1/125s** | 1/60s $\rightarrow$ 1/30s $\rightarrow$ 1/15s $\rightarrow$ 1/8s $\rightarrow$ ... |
| **[[感光度 (ISO)]]** (訊號增益等比) | ... $\leftarrow$ (無) $\leftarrow$ (無) | **ISO 100** | ISO 200 $\rightarrow$ ISO 400 $\rightarrow$ ISO 800 $\rightarrow$ ISO 1600 $\rightarrow$ ... |

---

## 1/3 檔微調 (1/3 Stop Steps)

現代數位相機的轉盤每轉一格通常是 **1/3 級（0.3 EV）**，而不是直接跳 1 整級。這讓曝光調整更加精準細緻。
* **光圈 1/3 檔範例**：
  $$\mathbf{f/2.8} \rightarrow f/3.2 \rightarrow f/3.5 \rightarrow \mathbf{f/4.0} \rightarrow f/4.5 \rightarrow f/5.0 \rightarrow \mathbf{f/5.6}$$
* **快門 1/3 檔範例**：
  $$\mathbf{1/125s} \rightarrow 1/160s \rightarrow 1/200s \rightarrow \mathbf{1/250s} \rightarrow 1/320s \rightarrow 1/400s \rightarrow \mathbf{1/500s}$$

---

## 新手實戰技巧：攝影師口中的「加一檔 / 減一檔」

當老手在現場說「光線不夠，你加一檔光圈」或「曝光過曝了，快門減一檔」時，意思非常單純：
* **「加一檔（+1 Stop）」**：透過把光圈開大一格、快門放慢一倍、或 ISO 拉高一倍，讓進光量增加一倍。
* **「減一檔（-1 Stop）」**：透過把光圈縮小一格、快門加快一倍、或 ISO 減半，讓進光量減少一半。

在半自動模式下，你只需要直接撥動 **[[曝光補償 (Exposure Compensation)|曝光補償 (+/- EV)]]** 轉盤，轉向 `+1` 或 `-1`，相機就會自動替你加減一檔曝光。

---

## 相關概念與延伸閱讀
* [[曝光三要素 (Exposure Triangle)]] - 曝光的互易與協同系統
* [[光圈 (Aperture)]] - 非線性平方根級距的由來
* [[快門速度 (Shutter Speed)]] - 線性時間級距
* [[感光度 (ISO)]] - 線性增益級距
* [[相機拍攝模式 (Camera Modes)]] - 相機如何在不同模式下自動計算級數
