---
title: "白平衡與色溫校正 (White Balance & Color Temperature)"
aliases: ["白平衡", "色溫", "K數", "White Balance", "Color Temperature", "Tint"]
tags:
  - photography
  - post-processing
  - color
created: 2026-11-17
updated: 2026-11-17
sources:
  - "raw/cambridge-digital-photo-editing-workflow.pdf"
  - "raw/fotobeginner-113-photography-terms.pdf"
---

# 白平衡與色溫校正 (White Balance & Color Temperature)

## 一句話核心定義
**白平衡（White Balance / WB）** 是數位暗房工作流的第一步；它的目的是**消除環境光源引發的非真實色偏（Color Cast）**，確保在不同光線下，物理上的純白色物體在照片中依然呈現為精準的純白色。

---

## 一、 色溫雙軸控制模型：溫度 (Temperature) 與 色調 (Tint)

色彩校正由兩個互補的色軸共同控制：

```text
【軸一：色溫軸 (Temperature - 絕對溫標 Kelvin / K 數)】
   藍色 (冷調 / Cool) ◄────────────────────────► 黃色/橘色 (暖調 / Warm)
  (2000K 燭光/日出)        (5500K 正午日光基準)        (10000K 藍天陰影)

【軸二：色調軸 (Tint)】
   綠色 (Green) ◄──────────────────────────────► 洋紅色 (Magenta)
  (辦公室日光燈管補償)                                 (自然光 / LED 偏色補償)
```

---

## 二、 典型環境光源與 K 數對照表

| 環境光源 | 物理色溫 (K 數) | 未校正時的相片色偏傾向 | 相機需加入的補償顏色 |
| :--- | :---: | :--- | :--- |
| **燭光、昏暗煤油燈** | 1,800K - 2,200K | 極度濃重的橙紅色 | 加入大量冷藍色 |
| **室內鎢絲燈泡 (Tungsten)** | 2,800K - 3,200K | 刺眼的黃色色偏 | 加入冷藍色中和 |
| **室內冷光螢光燈管 (Fluorescent)**| 4,000K - 4,500K | 詭異的慘綠色色偏 | 加入洋紅色 (Tint Magenta) 中和 |
| **晴朗正午直射陽光 (Daylight)** | **5,200K - 5,500K** | **中性標準白光（黃金基準線）** | 幾乎無需補償 |
| **陰天多雲 (Cloudy)** | 6,500K - 7,000K | 偏冷藍色、發陰沉 | 加入暖黃色提溫 |
| **晴天背陰處、藍色時刻 (Shade)** | 8,000K - 10,000K | 強烈冷冰冰的湛藍色 | 加入濃郁金黃色 |

---

## 三、 數位暗房三種校正手法

1. **白平衡滴管工具 (White Balance Dropper)**：
   * 這是最高效的手法。用滴管工具在照片中**點擊任何理應是「18% 中性灰」或「非反光純白/淺灰」的物體**（如灰色石牆、白襯衫、或預先拍攝的 **[[03-lighting-and-accessories/實用輔助器材|18% 灰卡]]**），軟體會自動計算並一瞬間減去整個畫面的色彩偏移！
2. **手動微調滑桿**：
   * 配合眼睛觀察皮膚顏色（避免人像臉色發綠發青），左右推動色溫與色調滑桿。
3. **藝術性色彩偏置 (Creative Color Toning)**：
   * 白平衡不一定非得「物理絕對正確」！拍夕陽時適度拉高 K 數（偏暖）能強化壯麗溫暖氛圍；拍夜景時適度調低 K 數（偏冷）能營造未來科幻冷色調。

---

## 相關概念與延伸閱讀
* [[數位後製標準十步工作流 (10-Step Workflow)]] - 白平衡作為後製工序第一步
* [[03-lighting-and-accessories/實用輔助器材]] - 灰卡在白平衡校準中的用法
* [[03-lighting-and-accessories/自然光與光質]] - 藍色時刻與黃金時刻的色溫特質
