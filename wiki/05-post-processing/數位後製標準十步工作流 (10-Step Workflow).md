---
title: "數位後製標準十步工作流 (10-Step Workflow)"
aliases: ["數位暗房工作流", "後製順序", "Post-Processing Workflow", "10-Step Editing"]
tags:
  - photography
  - post-processing
  - workflow
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-digital-photo-editing-workflow.pdf"
---

# 數位後製標準十步工作流 (10-Step Workflow)

## 一句話核心定義
**後製是拍出好作品的最後一環**；遵循 Cambridge in Colour 規範的**全球經典十步後製工序**，能最大化榨取感光元件 RAW 檔的潛力，並防止因工序顛倒導致的噪點暴增、畫質劣化與色階斷裂。

---

## 為什麼後製工序的先後順序（Order）至關重要？

如果你先進行大幅銳化、拉高反差，最後才想要來修補白平衡與消除雜訊：
* 先前的銳化早已把細小的雜訊放大成不可逆的彩色光斑！
* 先前的極端反差拉扯早已把暗部細節壓碎為死黑，無法挽救。
* 因此，**全流程嚴格遵循「從底層全域校正，到局部微調，最後才是輸出定案」的科學順序**。

---

## 標準數位後製十步全景圖

```text
【階段一：全域物理與基礎校準】
  1. 白平衡 (White Balance) ──► 校正色溫 (K數) 與色調 (Tint)，還原純淨色彩基底
  2. 曝光與高光陰影 (Exposure) ─► 曝光補償、壓暗過曝高光、提亮死黑陰影
  3. 數位降噪 (Noise Reduction) ─► 在影像銳化前先抹平高 ISO 雜訊
  4. 鏡頭校正 (Lens Corrections) ─► 一鍵修正四角暗角、紫邊色差與幾何畸變
          │
          ▼
【階段二：反差、細節與藝術構圖】
  5. 擷取銳化與清晰度 (Capture Sharpening & Clarity) ─► 補償感光元件物理軟化
  6. 對比階調 (Contrast / Curves) ──► 黑白場定錨、S 型曲線營造立體 3D Pop 感
  7. 旋轉裁切 (Framing & Crop) ─────► 拉正地平線、精準裁切構圖 (3:2, 16:9, 1:1)
  8. 色彩與局部微調 (Refinements) ──► 污點移除、局部筆刷提亮、自然飽和度調整
          │
          ▼
【階段三：終端輸出準備】
  9. 尺寸縮放 (Resizing) ───────────► 依照發布目標 (網路社群 vs 實體輸出印刷) 重採樣
  10. 輸出銳化 (Output Sharpening) ──► 針對特定顯示螢幕或印刷紙質進行最後一道銳化
```

---

## RAW vs JPEG 的工序差異

* **拍攝 RAW 格式（強烈推薦）**：
  * RAW 檔的編輯是**非破壞性編輯 (Non-destructive)**。在 Lightroom / Adobe Camera RAW 中，各步驟的運算底層由軟體智慧排程，即使先調曲線再調白平衡，也不會破壞原始資料。
* **拍攝 JPEG 格式**：
  * JPEG 是 8-bit 破壞性壓縮檔案。**必須嚴格依照上述 1 到 10 步順序執行**，否則極端拉伸極易產生**色階斷裂 (Posterization)** 與嚴重雜訊！

---

## 相關概念與延伸閱讀
* [[白平衡與色溫校正 (White Balance & Color Temperature)]] - 第一步的色彩基石
* [[曝光微調與高光陰影還原 (Exposure & Dynamic Range Recovery)]] - 第二步的動態範圍重構
* [[降噪與銳化平衡 (Noise Reduction vs Sharpening)]] - 第三與第五步的博弈
* [[RAW vs JPEG 深度解析 (RAW vs JPEG Format)]] - 為什麼後製必須從 RAW 檔開始
