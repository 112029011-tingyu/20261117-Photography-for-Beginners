---
title: "鏡頭數位校正 (Lens Corrections)"
aliases: ["鏡頭校正", "色差校正", "暗角校正", "幾何畸變校正", "Lens Corrections", "Profile Corrections"]
tags:
  - photography
  - post-processing
  - optics
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-digital-photo-editing-workflow.pdf"
  - "raw/cambridge-understanding-camera-lenses.pdf"
---

# 鏡頭數位校正 (Lens Corrections)

## 一句話核心定義
**鏡頭數位校正 (Lens Corrections)** 是後製第四步的標準工序；它利用光學實驗室為各廠牌鏡頭量身打造的精確數學模型（Profile），在電腦中**一鍵自動消除色差紫邊、抹平四角暗角、並將幾何畸變拉直**。

---

## 鏡頭校正面板的三大核心修復項

```text
Lightroom / Camera RAW 鏡頭校正模組:
  ├── [✔] 移除色差 (Remove Chromatic Aberration) ──► 一鍵消除高反差紫邊/綠邊
  └── [✔] 啟用設定檔校正 (Enable Profile Corrections)
            ├── 變形修正 (Distortion Correction) ──► 廣角桶狀/望遠枕狀畸變拉正
            └── 暗角修正 (Vignetting Correction) ──► 邊緣與四個角落平滑提亮
```

### 1. 移除色差 (Remove Chromatic Aberration)
* **自動消除**：勾選後，演算法會自動沿著高反差邊緣偵測互補色波長偏差，直接吸除紫邊與綠邊。
* **手動去邊工具 (Defringe)**：若面對極端逆光樹枝依然殘留頑固紫邊，可開啟手動去邊面板，用滴管點擊紫邊顏色，精準擴大吸除寬度。

### 2. 幾何變形修正 (Distortion Correction)
* **廣角桶狀畸變拉直**：將原本向外凸起的地平線與建築物外牆線條一瞬間繃平拉正。
* **物理代價**：畸變校正的幾何本質是「四角拉伸與重採樣」，拉伸過程會極微幅犧牲邊角的原始解像度，且會微幅裁切掉畫面最外圍一圈邊緣。

### 3. 暗角消除 (Vignetting Correction)
* **平滑補償**：讀取鏡頭的光學暗角曲線，在中央亮度不變的前提下，精準地將四個變暗的角落補償提亮 +0.5 ~ +1.5 級。
* **代價注意**：因為提亮了四角，邊角的暗部雜訊可能會隨之微幅增加。

---

## 相關概念與延伸閱讀
* [[數位後製標準十步工作流 (10-Step Workflow)]] - 鏡頭校正在十步工作流中的地位
* [[02-optics-and-gear/光學像差與瑕疵 (Optical Aberrations)]] - 色差、暗角與畸變的光學物理源頭
* [[裁切構圖與色彩微調 (Framing & Color Refinements)]] - 校正畸變後的邊界裁切處理
